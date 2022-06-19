# Challenge DevOps

# Build da aplicação
```
docker build --tag aluraflix .
```

# Primeira execução
- Executar migration do banco
```
python manage.py migrate
```
- Criar usuário
```
python manage.py createsuperuser
```

# Utilização com docker compose
- Executar
```
docker compose up -d
```
- Executar migration no container
```
 docker exec -it aluraflix python manage.py migrate
```
- Executar criação de usuário
```
 docker exec -it aluraflix python manage.py createsuperuser
```

# Referências
- https://github.com/docker/awesome-compose/tree/master/django