***Local development commands:***

```shell
# install
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install flask
flask run
pip install -r requirements.txt

# run
docker build -t flask-api .
docker run -p 5000:80 flask-api
docker run -w /app flask-api sh -c "rq worker -u $REDIS_URL"

# db
flask db init
flask db migrate
flask db upgrade
```