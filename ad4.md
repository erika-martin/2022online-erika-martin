<<engine='python', engine.path='python3'>>=
req = requests.get("https://resultados.elpais.com")
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')

