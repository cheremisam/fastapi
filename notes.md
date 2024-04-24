pip install fastapi[all]
pip install sqlalchemy alembic psycopg2-binary
alembic init migrations
alembic revision --autogenerate -m "Database creation"
alembic upgrade cc7b6356eeae

uvicorn main:app --reload
