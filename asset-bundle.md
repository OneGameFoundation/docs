---
layout: single
sidebar:
  nav: "docs"
---

### Asset Bundle
-----------------------------

The One Game Asset Bundle is a unit of assets that contains specific dependencies such as image, audio clip, texture, model.  

An asset bundle manifest file describes all the dependencies of an asset bundle. A manifest file is a text file that you can open with any text editor.  Below, we have a manifest file that describes the dependencies of Basic Buildings, the name of the Asset Bundle. The name is the name of the asset bundle. The path is the location of asset bundle on the server. The assets is a flat array containing the specific assets of this bundle. In this simple exmaple, the assets contain three png files.

```javascript
[
    {
        "id" : 1,
        "name" : "Basic Buildings",
        "path" : "/bundles/experimental/buildings",
        "assets" : [
            {
                "id" : 0,
                "name" : "Building 1",
                "prefab" : "Tall building",
                "type" : 0,
                "thumbnail-path" : "/images/building1.png"
            },
            {
                "id" : 1,
                "name" : "Building 2",
                "prefab" : "Tall Building",
                "type" : 0,
                "thumbnail-path" : "/images/building2.png"
            },
            {
                "id" : 2,
                "name" : "Building 3",
                "prefab" : "Tall Block",
                "type" : 0,
                "thumbnail-path" : "/images/building3.png"
            }
        ]
    }
]
```

Each asset in the bundle should have the following fields:
* id = The unique id of the asset
* name = The custom name of the asset
* prefab = The name of the prefab in the asset bundle
* type = The type of asset (TBD, but this is an integer for now)
* thumbnail-path = The relative path of the thumbnail on the server e.g. /images/building1.png

Asset Bundles can contain any arbitrary number of dependencies, but each requires a manifest file. We will provide a tutorial walking through how to create an Asset Bundle.
