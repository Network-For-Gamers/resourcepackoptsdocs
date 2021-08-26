# ResPackOpts Toggle Files With A Fallback Option (Alternate Files)

This is a simple `IF` satment simply returning true/false to if the texture/file should be loaded into the pack. (Pick one file over another). You will need the `PackID` and `EntryName` from your `/assets/respackopts/conf.json` that you created earlier if you have not see [Main Config](https://github.com/Network-For-Gamers/resourcepackoptsdocs/blob/main/MainConfig.md) on how to do so.
<br>

You will need to navigate to the file you would like to toggle inside your resource, and create a `.rpo` file for it in the same folder(directory).
<br>

### Examples:
`texture.png` would be `texture.png.rpo`<br>
`SomeRecipe.json` would be `SomeRecipe.json.rpo`
<br>

### Layout:
```json
{
    "conditions": [
        "<your pack id>:<your entry>"
    ],
    "fallbacks": ["location/of/the/file"]
}
```
### Example:
```json
{
    "conditions": [
        "ExamplePack:Texture"
    ],
    "fallbacks": ["assets/respackopts/examplealternatefiles/SomeTexture.json"]
}
```
---

### See [Toggle Files ](https://github.com/Network-For-Gamers/resourcepackoptsdocs/blob/main/ToggleFiles.md) to see how to just disable files.
