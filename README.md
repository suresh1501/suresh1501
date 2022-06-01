import requests
from bs4 import Beautifulsoup

url = 'https://www.google.com'

req = requests.get(url)

soup = Beautifulsoup(req.text, 'html.parser')

print(soup)
