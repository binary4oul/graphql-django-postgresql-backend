# Folder Structure:
1) `core`: contains all core functionalites ex (BaseModel, BaseMutation)
2) `users` contains user related mutation, models, types, queries
3) `articles` contains all article related models, mutation, types, queries
4) `tests` all test related stuff
5) `medium` contains all django urls, settings, and others.

# Getting started

1) Install dependancies
`poetry install`

2) create `.env` file with this content
`DEBUG=True ` 
`SECRET_KEY=test-secret-key`
 `DATABASE_URL=postgresql://postgres:password@localhost:5432/medium`
3) run migration
 `poetry run python manage.py migrate`
4) run server
`poetry  run python manage.py runserver 8000`
5) open graphql playground using http://localhost:8000/playground
6) to connect to it via API use http://localhost:8000/graphql


## Third Party Packages
1) `graphene-django`: Add Graphql to a django server
2) `python-decouple`: manage django settings using .env file
3) `django-graphql-jwt`: Add JWT authentication
4) `graphene-django-optimizer`: Optimize database queries to avoid N+1 problem
5) `graphene-file-upload`: Add mutlipart file upload mutations to graphene

## Testing
some tests were added to `tests` directory, packages used for testing:
1) `pytest`
2) `pytest-django`
3) `factory-boy`
****
