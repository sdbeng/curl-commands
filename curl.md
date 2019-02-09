## curl, command line
```
# curl, command line
curl "http://api.giphy.com/v1/gifs/search?q=ryan+gosling&api_key=YOUR_API_KEY&limit=5"
```

# python
import urllib,json
data = json.loads(urllib.urlopen("http://api.giphy.com/v1/gifs/search?q=ryan+gosling&api_key=YOUR_API_KEY&limit=5").read())
print json.dumps(data, sort_keys=True, indent=4)

//javascript, jQuery
var xhr = $.get("http://api.giphy.com/v1/gifs/search?q=ryan+gosling&api_key=YOUR_API_KEY&limit=5");
xhr.done(function(data) { console.log("success got data", data); });
