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
