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
docker run -p 5000:5000 -w /app -v ${PWD}:/app flask-api sh -c "flask run --host 0.0.0.0"

# db
flask db init
flask db migrate
flask db upgrade
```