# Working-with-the-devices-API

The beginning of an awesome article...

```python
import requests

url = "http://localhost:3000/api/devices/one"

querystring = {"API Key":"0123654789"}

payload = "{\"deviceID\":\"string\",\"deviceName\":\"string\",\"dateCreated\":\"2017-07-21T17:32:28Z\",\"dateUpdated\":\"2017-07-21T17:32:28Z\",\"user\":{\"userID\":\"string\",\"userName\":\"string\",\"email\":\"string\"},\"account\":{\"accountID\":\"string\",\"accountName\":\"string\",\"userCount\":0,\"deviceCount\":0},\"location\":{\"lat\":0,\"long\":0,\"geoTracking\":true}}"
headers = {'deviceName': 'newDevice'}

response = requests.request("POST", url, data=payload, headers=headers, params=querystring)

print(response.text)
```