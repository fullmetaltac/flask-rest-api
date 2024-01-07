
***Useful commands:***

```
python -m venv .venv
pip install flask
flask run
pip install -r requirements.txt
docker build -t flask-smorest-api .
docker run -dp 5000:5000 -w /app -v ${PWD}:/app flask-smorest-api
```