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
[
  {
    "city_name": "Tanzania",
    "country_name": "Arusha"
  },
  {
    "city_name": "Birmingham",
    "country_name": "(UK)"
  },
  {
    "city_name": "Leeds",
    "country_name": "(UK)"
  },
  {
    "city_name": "Glasgow",
    "country_name": "(UK)"
  },
  {
    "city_name": "Sheffield",
    "country_name": "(UK)"
  },
  {
    "city_name": "Bradford",
    "country_name": "(UK)"
  },
  {
    "city_name": "Liverpool",
    "country_name": "(UK)"
  },
  {
    "city_name": "Edinburgh",
    "country_name": "(UK)"
  },
  {
    "city_name": "Manchester",
    "country_name": "(UK)"
  },
  {
    "city_name": "Bristol",
    "country_name": "(UK)"
  },
  {
    "city_name": "Wakefield",
    "country_name": "(UK)"
  },
  {
    "city_name": "Cardiff",
    "country_name": "(UK)"
  },
  {
    "city_name": "Dudley",
    "country_name": "(UK)"
  },
  {
    "city_name": "Wigan",
    "country_name": "(UK)"
  },
  {
    "city_name": "Coventry",
    "country_name": "(UK)"
  },
  {
    "city_name": "Belfast",
    "country_name": "(UK)"
  },
  {
    "city_name": "Leicester",
    "country_name": "(UK)"
  },
  {
    "city_name": "Sunderland",
    "country_name": "(UK)"
  },
  {
    "city_name": "Doncaster",
    "country_name": "(UK)"
  },
  {
    "city_name": "Stockport",
    "country_name": "(UK)"
  },
  {
    "city_name": "Nottingham",
    "country_name": "(UK)"
  },
  {
    "city_name": "Newcastle",
    "country_name": "(UK)"
  },
  {
    "city_name": "Kingston",
    "country_name": "(UK)"
  },
  {
    "city_name": "Bolton",
    "country_name": "(UK)"
  },
  {
    "city_name": "Walsall",
    "country_name": "(UK)"
  },
  {
    "city_name": "Plymouth",
    "country_name": "(UK)"
  },
  {
    "city_name": "Rotherham",
    "country_name": "(UK)"
  },
  {
    "city_name": "Stoke",
    "country_name": "(UK)"
  },
  {
    "city_name": "Wolverhampton",
    "country_name": "(UK)"
  },
  {
    "city_name": "South",
    "country_name": "(UK)"
  },
  {
    "city_name": "Derby",
    "country_name": "(UK)"
  },
  {
    "city_name": "Swansea",
    "country_name": "(UK)"
  },
  {
    "city_name": "Salford",
    "country_name": "(UK)"
  },
  {
    "city_name": "New York",
    "country_name": "(US)"
  },
  {
    "city_name": "Los Angeles",
    "country_name": "(US)"
  },
  {
    "city_name": "Chicago",
    "country_name": "(US)"
  },
  {
    "city_name": "Houston",
    "country_name": "(US)"
  },
  {
    "city_name": "Phoenix",
    "country_name": "(US)"
  },
  {
    "city_name": "Philadelphia",
    "country_name": "(US)"
  },
  {
    "city_name": "San Antonio",
    "country_name": "(US)"
  },
  {
    "city_name": "San Diego",
    "country_name": "(US)"
  },
  {
    "city_name": "Dallas",
    "country_name": "(US)"
  },
  {
    "city_name": "San Jose",
    "country_name": "(US)"
  },
  {
    "city_name": "Austin",
    "country_name": "(US)"
  },
  {
    "city_name": "Jacksonville",
    "country_name": "(US)"
  },
  {
    "city_name": "Fort Worth",
    "country_name": "(US)"
  },
  {
    "city_name": "Columbus",
    "country_name": "(US)"
  },
  {
    "city_name": "Indianapolis",
    "country_name": "(US)"
  },
  {
    "city_name": "Charlotte",
    "country_name": "(US)"
  },
  {
    "city_name": "San Francisco",
    "country_name": "(US)"
  },
  {
    "city_name": "Seattle",
    "country_name": "(US)"
  },
  {
    "city_name": "Denver",
    "country_name": "(US)"
  },
  {
    "city_name": "Washington",
    "country_name": "(US)"
  },
  {
    "city_name": "Nashville-Davidson",
    "country_name": "(US)"
  },
  {
    "city_name": "Oklahoma City",
    "country_name": "(US)"
  },
  {
    "city_name": "El Paso",
    "country_name": "(US)"
  },
  {
    "city_name": "Boston",
    "country_name": "(US)"
  },
  {
    "city_name": "Portland",
    "country_name": "(US)"
  },
  {
    "city_name": "Las Vegas",
    "country_name": "(US)"
  },
  {
    "city_name": "Detroit",
    "country_name": "(US)"
  },
  {
    "city_name": "flag",
    "country_name": "HTB{crud_4p!_m4n!pul4t0r}"
  }
]

 ```
