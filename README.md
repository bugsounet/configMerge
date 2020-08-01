# configMerge

Merging MagicMirror (or other) default/config script
merge 2 objects

## Using:

this.config = configMerge({}, this.defaults, this.config)

|Arg Number| Function
|---|---
|Arg 1| Initial objet
|Arg 2| Config model
|Arg 3| Config to merge

## Load the script in MagicMirror

You have to load the script on the main core of your module

```
getScripts: function () {
  return [
    "configMerge.js"
  ]
},
```

## Why using it ?
Object.assign() function don't to all job

it don't merge all thing in depth

 -> object in object and array is not merging

