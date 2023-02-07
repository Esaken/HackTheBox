```
Hello my name is Kennedy Esau
Below is the last question on web requests (Crud API)
Which focuses on the creation, Read, Update and delete features on API
```

# Remeber to edit the server ip and port as i do not expect them to match my instance server

1. First, try to update any city's name to be 'flag'. Then, delete any city. Once done, search for a city named 'flag' to get the flag.

### START
 
 > sudo apt install jq
 INSTALL this feature as it will help to view the database

 > view all cities-

```
curl http://134.209.17.36:31855/api.php/city/ | jq
```

> -update a city called london to  Arusha in Tanzania-

```
curl -X PUT http://134.209.17.36:31855/api.php/city/london -d '{"city_name":"Tanzania", "country_name":"Arusha"}' -H 'Content-Type: application/json'

```

> added Nairobi as well-(Create a city)
```
curl -X POST http://134.209.17.36:31855/api.php/city/ -d '{"country_name":"Kenya", "city_name":"Nairobi"}' -H 'Content-Type: application/json'
```

> update a city to be called flag

```
curl -X PUT http://134.209.17.36:31855/api.php/city/Baltimore -d '{"city_name":"flag", "country_name":"(US)"}' -H 'Content-Type: application/json'
```

> -view your hardwork-
```
curl http://134.209.17.36:31855/api.php/city/ | jq
```

> delete a city

```
curl -X DELETE http://134.209.17.36:31855/api.php/city/Memphis
```

> -search for memphis to ensure its deleted-
```
curl -X DELETE http://134.209.17.36:31855/api.php/city/Memphis
```

### *the [] means its blank

> Delete a city you added to view the flag
```
curl -X DELETE http://134.209.17.36:31855/api.php/city/Nairobi

```

> -view all the cities to see the flag
 ```
curl -s  http://134.209.17.36:31855/api.php/city/  | jq
 ```

 ### ANSWER


 ```
