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

## Note:
You can also use the Minified code version `mergeConfig.min.js`
 
## How download it:
In your terminal use the wget command
```
wget https://raw.githubusercontent.com/bugsounet/configMerge/master/configMerge.js
```
or for Minified version
```
wget https://raw.githubusercontent.com/bugsounet/configMerge/master/configMerge.min.js
```
