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

### See [Togglefiles](https://github.com/Network-For-Gamers/resourcepackoptsdocs/blob/main/ToggleFiles.md) to see the logic behind this

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

## Adding a slider
A slider is slightly more complicated as a minimum and a maximum need to be defined. Sliders also only support whole numbers.

### Example:
```json
{
    "id": "ExamplePack",
    "version": 4,
    "conf": {
        "SomeOption": {
            "min": 0,
            "default": 5,
            "max": 10
        }
    }
}
```
### Result:


## Select From a list
To allow users to select one entry from a list, you can use a json array with string entries. *Numbers/etc are not supported*

### Example:
```json
{
    "id": "ExamplePack",
    "version": 4,
    "conf": {
        "SomeOption": [
            "option_one",
            "option_two",
            "option_three"
        ]
    }
}
```
### Result:


## Make a category

### Example:
```json
{
    "id": "ExamplePack",
    "version": 4,
    "conf": {
        "SomeCategory": {
            "SomeBoleanOption": true,
            "SomeNumberOption": 5,
            "SomeSelectionOption": [
                "option_one",
                "option_two",
                "option_three"
           ],
            "SomeSliderOption": {
                "min": 0,
                "default": 5,
                "max": 10
            }
        },
        "SomeotherCategory": {
            "SomeOtherBoleanOption": true,
            "SomeOtherNumberOption": 5,
        }
    }
}
```
### Result:
