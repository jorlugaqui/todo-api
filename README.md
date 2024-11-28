# todo-api
DRF ToDo API

## Run the project (db)
`docker compose up -d db`

## Run the API
`docker compose up api`

## Run the test
`docker compose exec api python manage.py test --settings=todoapp.settings.ci`

## Coverage
```
docker compose exec api coverage run manage.py test --settings=todoapp.settings.ci && coverage report -m
```

## Run the linter
`docker compose exec api ruff check . --fix`

## Run the formatter
`docker compose exec api ruff format .`
