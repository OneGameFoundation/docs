---
layout: single
sidebar:
  nav: "docs"
---

### One Game Asset Bundle
-----------------------------

This article covers the fundamentals to understand how to efficiently load assets to create asset bundles. Proper Asset creation is crucial step effective development on the One Game platform. 

## Asset Bundles

An asset textures, 3D models, or audio clips are common types of Assets. From the One Game Asset Store, you can download default bundles or you can go to open source resources such as Google Poly to find asset models with textures. Some assets contain data in formats native to Unity, such as materials. Other Assets need to be processed into native formats, such as FBX files. 

From those assets, we can create asset bundles which can be used as part of your game in One Game. You can also look for asset bundles that we will be able to offer in One Game Asset Store.

In One Game, we have several types of bundle that are predefined with a default format and a generalized manifest. When we have more asset bundles from the community, we will add the following support tags to allow easy categorization of asset bundles. The supported tags are as follows:

* Human characters
* Animal
* Building
* Plant
* Static item
* Weapon

Each type of bundle has its own manifest example format. With each bundle type, we have a default or base manifest for each bundle type. You can also come to Developer Docs here to check out default manifest for each type of asset bundles and use these as references when you build your own asset bundles.


## Manifest of an Asset Bundle


The One Game Asset Bundle is a unit of assets that contains specific dependencies such as image, audio clip, texture, model.  

An asset bundle manifest file describes all the dependencies of an asset bundle and contains metadata for a group of files that are used in an Asset Bundle. A manifest file is a text file that you can open with any text editor.  Below, we have a manifest file `manifest.json` that describes the dependencies of Basic Buildings, the name of the Asset Bundle. The name is the name of the asset bundle. The path is the location of asset bundle on the server. The assets is a flat array containing the specific assets of this bundle. In this simple exmaple, the assets contain three png files.

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
* thumbnail-path = The relative path of the thumbnail on the server, such as `/images/building1.png`





## Creating Asset Bundles
Asset Bundles are Unity-related containers that store custom assets in a compact way. 
They can be easily created in any Unity Project using the *AssetBundleBrowser* tool. 
[Refer to this link on how to create asset bundles.](https://unity3d.com/learn/tutorials/topics/scripting/assetbundles-and-assetbundle-manager)

Requirements for pushing asset bundles:
* Unity 2018.1
* AssetBundleBrowser 1.5 or above (accessible via PackageManager)
* Update the bundle manifest file manually to publish changes (see below). 
* Do note that the assets must be referenced in `bundle-asset-manifest.json` and/or 
`script-manifest.json` for the game to recognize any new assets. 




### Updating AssetBundle Manifest Files
All bundles (for now) should be an element in the `bundle-asset-manifest.json` file
Each bundle should have the following fields:
  * **id** = The unique id of the bundle 
  * **name** = The custom name for the bundle
  * **path** = The relative path of the bundle in the server e.g. */bundles/a-random-bundle*
  * **assets** = An array of assets that this bundle will provide

Each asset in the bundle should have the following fields:
 * **id** = The unique id of the asset
 * **name** = The custom name of the asset
 * **prefab** = The name of the prefab in the asset bundle
 * **type** = The type of asset *(TBD, but this is an integer for now)*
 * **thumbnail-path** = The relative path of the thumbnail on the server e.g. */images/prop5.jpg*

Here is an example of a bundle:
```json
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
```

### Updating Script Manifest Files
Script manifests are much simpler to update.  Each element must have the following fields:

* **id** = The unique id of the script template
* **name**  = The custom name of the script
* **asset-path** = The relative path of the script on the server e.g. *scripts/spawner.lua*

Here's an example of a script in the manifest file:

```json
{
    "id" : 5,
    "name" : "Zombie AI",
    "asset-path" : "/scripts/zombie-ai.lua"
}
```
