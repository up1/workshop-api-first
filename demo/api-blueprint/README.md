# Workshop with [API Blueprint](https://apiblueprint.org/)


## Generate API Document with [Aglio](https://www.npmjs.com/package/aglio)
```
$npm i -g aglio
$aglio -i example-api.apib -o output.html
```

## Create Mock API with [Drakov](https://www.npmjs.com/package/drakov)
```
$npm i -g drakov
$drakov -f example-api.apib --watch --public -p 3000
```