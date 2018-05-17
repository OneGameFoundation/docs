---
layout: single
sidebar:
  nav: "docs"
---

### Asset Bundle
-----------------------------

The One Game Asset Bundle is a unit of asset that contains specific dependencies such as image, audio clip, texture, model).  An asset bundle manifest file describes all the dependencies of an asset bundle.

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
