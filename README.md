import requests

url = "http://sasbap.demo.sas.com:80/SASFederationData/fedsrv/servers/Federation%20Server%20sasbap/dataSources/BASE/catalogs/SECUREVIEWS/schemas/T000001/tables/CASUALTY"

payload = ""
headers = {
    'Authorization': "Basic c2FzOk9yaW9uMTIz",
    'cache-control': "no-cache",
    'Postman-Token': "06e0aa61-64a2-4989-b713-9e7947bad68d"
    }

response = requests.request("GET", url, data=payload, headers=headers)

print(response.text)
