---
layout: single
sidebar:
  nav: "docs"
---

### Step-by-Step Basic Tutorial for Creating an Asset Bundle: Laughing Panda
-----------------------------------------------------------------------------

We are excited that you're getting ready to dive in and create Asset Bundles. You can upload and distribute the Asset Bundles nto our Asset Store in the future and make real money.

**Step 1**: Download Unity [here](https://unity3d.com/get-unity/download) and open Unity.


**Step 2**: Download the Panda files from this git repository [here](https://github.com/OneGameFoundation/docs/tree/master/assets/Mesh_Panda).

**Step 3**: Import the Panda files, `Mesh_Panda.obj` (the object), `Tex_Panda.png` (the texture), and the `panda-laugh` (the sound clip), into Unity by dragging the Panda object `Mesh_Panda.obj`, Panda texture `Tex_Panda.png`, and Panda sound clip `panda-laugh` into the Unity Project window, under Assets > Models.

![Drag Panda Files into Unity](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step2.png)


**Step 4**: Drag Mesh_Panda into the Hierarchy window and confirm that the Panda model is now visibly being displayed in the Scene window as seen below.

![Panda Model Displaying](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step3.png)


**Step 5**: Add texture to the Panda. Right click in Assets Folder and create Material. Let's simply name the Material `Panda`. Then, right click Material to attach texture `Tex_Panda` to the Material. In the right panel Inspector, you can see that the the texture is now applied (see Albedo) on the Material. 

![Panda Texture Applied](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step3.png)


**Step 6**: Drag the Material on the the Panda Mesh object in the Scene. Now we see that now the panda has material applied and this panda has the panda skin applied.

![Panda Mesh Added](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step4.png)


**Step 7**: Attach the sound file, `panda-laugh`, to the Mesh Panda. Add the sound file to the Panda as an Audio Source. In the right panel Inspector, you can see that the Mesh Panda model now has an Audio Source.

![Panda Sound File Added](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step5.png)


**Step 8**: Now let's create a Prefab for the Mesh Panda. The prefab asset allows you to store an asset with all its properties inside the prefab. Simply, drag Mesh_Panda into the Prefabs folder and Unity will create Prefabs automatically.

![Panda Prefab Created](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step6.png)


**Step 9**: Now let's create the Asset Bundle. Let's make the Asset Bundle to `laughing panda. See in the lower right corner, and add title `laughing panda` as the title to the Asset Bundle.
![Panda Asset Bundle Created](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step7.png)


**Step 10**: We click on `laughing panda`, we have the Mesh Panda and has all dependencies in it. A manifest file is automatically generated and it should be the same as below. Opening in the manifest file in a text editor should show the following json.

```javascript
{
    "id" : 5,
    "name" : "Laughing Panda",
    "path" : "/bundles/experimental/laughing panda",
    "assets" : [
        {
            "id" : 21,
            "name" : "Laughing Panda",
            "prefab" : "Mesh_Panda",
            "type" : 3,
            "thumbnail-path" : "/images/panda.png"
        }
    ]
}
```

**Step 12**: In the Asset Bundles tab, click on Build tab on the top and define the Output Path for `laughing panda`. You can leave Advanced Settings as defaulted.

![Panda Output Path](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step8.png)


**Step 13**: When you've defined the Output Path and ready to Build, click on the horizontal flat Build button, and Unity will build the laughing panda Asset Bundle.

**Step 14**: Find the exported `laughing panda` at the Output Path. We are done creating an asset bundle called `laughing panda`. Congratulations!

![Panda Exported](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step9.png)


**Step 16**: In One Game client storage, you can put in the laughing panda build here. Open One Game and push to asset server. In the future, you will be able to sell and to distribute your Asset Bundles in our Asset Store in the future where you can make money. Your imagination is the limit.

**Step 17**: You can also use the Asset Bundle, `laughing panda` locally in One Game. Below, we now see the panda in a scene in One Game.

![Panda in One Game](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step10.png)

If you have any questions, connect with our developers on social channels. We will be offering more tutorials for our developers.



