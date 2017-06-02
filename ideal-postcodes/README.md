ideal-postcodes (https://ideal-postcodes.co.uk/documentation)

Search address by post code
```
curl --header 'Authorization: IDEALPOSTCODES api_key="my-key"' --proxy localhost:8500 https://api.ideal-postcodes.co.uk/v1/postcodes/SE10NZ
```

Postcode search that returns rate limited error
```
curl --header 'Authorization: IDEALPOSTCODES api_key="my-key"' --proxy localhost:8500 https://api.ideal-postcodes.co.uk/v1/postcodes/ID1CHOP
```

Postcode search that returns invalid postcode error
```
curl --header 'Authorization: IDEALPOSTCODES api_key="my-key"' --proxy localhost:8500 https://api.ideal-postcodes.co.uk/v1/postcodes/ID1
```

Search address
```
curl --header 'Authorization: IDEALPOSTCODES api_key="my-key"' --proxy localhost:8500 https://api.ideal-postcodes.co.uk/v1/addresses --data-urlencode "q=10 Downing Street London" -G
```

Get address autocomplete suggestion
```
curl --header 'Authorization: IDEALPOSTCODES api_key="my-key"' --proxy localhost:8500 https://api.ideal-postcodes.co.uk/v1/autocomplete/addresses --data-urlencode "q=10 Downing Str" -G
```

Get postcodes by coordinates
```
curl --header 'Authorization: IDEALPOSTCODES api_key="my-key"' --proxy localhost:8500 https://api.ideal-postcodes.co.uk/v1/postcodes --data-urlencode "lonlat=-0.20864,51.48994" -G
```
