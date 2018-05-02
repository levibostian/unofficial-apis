# Pollen.com

From the [terms of use](https://www.pollen.com/help/tou), you can only use Pollen.com's content for personal use only. No commercial use allowed. 

# How to access API

## 5 day forecast 

```
GET https://www.pollen.com/api/forecast/extended/pollen/{zip-code}

Headers:
Content-Type: application/json; charset=utf-8
Host: www.pollen.com
Connection: keep-alive
Accept-Language: en-US,en;q=0.8
Accept-Encoding: gzip, deflate, sdch, br
Accept: application/json, text/plain, */*
Referer: https://www.pollen.com/forecast/extended/pollen/{zip-code}
```

Options:
```
{zip-code} replace with your zip code for the location you want to show. 
```

## Yesterday, today, tomorrow more detailed forecast 

Same as the `5 day forecast` except you replace `extended` in the endpoint URL and the `Referer` header URL with `current`. 

### Credits 

Thanks [JakeRuss/sneezr](https://github.com/JakeRuss/sneezr) for showing how to access the pollen.com's API.
