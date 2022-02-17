# webcrawling

if a site is forbidden to do web crawling, with error code 403. then option is to use Request, with agent.

from urllib.request import urlopen
from bs4 import BeautifulSoup
html=urlopen('https://www.pythonscraping.com/pages/page3.html')
bs=BeautifulSoup(html, 'html.parser')

# Normally we can do that above. but when a website is blocking its source to be crawled, we need to pass browser information

This example is exactly does this. Learning from doing..
