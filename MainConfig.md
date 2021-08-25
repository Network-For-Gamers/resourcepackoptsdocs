# ResourcePackOpts Config.

### Location (ResourcePacks).
> `/assets/respackopts/conf.json`

### Location (DataPacks).
> `/data/respackopts/conf.json`

## What needs to be here.
```json
{
    "id": "<PackID>",
    "version": 4,
    "conf": {
        // Your config options here
    }
}
```

## Adding a Toggle/Boolean

To add a boolean entry, add code like this: `"entryName": <Default Option (true/false)>` 

### Example:
```json
{
    "id": "ExamplePack",
    "version": 4,
    "conf": {
        "SomeTexture": true,
        "SomeOtherTexture": false
    }
}
```
### Result:
![configExampleBolean](https://github.com/Network-For-Gamers/resourcepackoptsdocs/blob/main/img/ExamplePackBoolean.PNG?raw=true "ConfigExampleBolean")



## Adding a Free Number Box
A number box follows the same principle as a boolean: `"entryName": DefaultNumber`
*please note any value can be put in here with no limit*

### Example:
```json
{
    "id": "ExamplePack",
    "version": 4,
    "conf": {
        "SomeOption": 10
    }
}
```
### Result:
![configExampleNumber](https://github.com/Network-For-Gamers/resourcepackoptsdocs/blob/main/img/ExamplePackNumber.PNG?raw=true "ConfigExampleNumber")
