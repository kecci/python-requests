# python-requests

## Install python and pipenv
```
$ brew install python
$ brew install pipenv
```

## install dependency requests
```
$ pipenv install requests
```

## Application
create `main.py`
```
import requests

response = requests.get('https://httpbin.org/ip')

print('Your IP is {0}'.format(response.json()['origin']))
```

## Run application
```
pipenv run python main.py
```

output:
```
Your IP is 8.8.8.8
```
