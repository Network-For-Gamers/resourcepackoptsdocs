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
### Result
![configExample](https://github.com/Network-For-Gamers/resourcepackoptsdocs/blob/main/img/ExamplePackBoolean.PNG?raw=true "ConfigExample")



## Adding a Free Number Box

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
