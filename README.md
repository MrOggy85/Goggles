# Goggles

* Official docs: https://github.com/brave/goggles-quickstart
* Syntax: https://github.com/brave/goggles-quickstart/blob/main/goggles/quickstart.goggle

## Options

`$site` - limit a instruction to a specific website
```
$site=brave.com
/blog/$site=brave.com
```

`$boost` - customize the ranking of results to your liking
```
/r/brave_browser/
/r/brave_browser/$boost
/r/brave_browser/$boost=2
/r/brave_browser/$boost=3
```

`$discard` - discard results completely:
```
$discard,site=idontwanttobepartoftheresults.com
/this/is/spam/$discard
```

# How can I exclude any result not matched by my Goggle?
You can change the “default action” by adding a generic `$discard` rule
```
$discard
[...]
```
