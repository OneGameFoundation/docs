---
layout: single
sidebar:
  nav: "docs"
---

### Step by Step Basic Tutorial for Creating Laughing Panda Asset Bundle
-------------------------------------------------------------------------

Step 1: [Download Unity](https://unity3d.com/get-unity/download) and open Unity.


Step 2: Download the Panda files from this git repository [here](https://github.com/OneGameFoundation/docs/tree/master/assets/Mesh_Panda).

Step 3: Import the Panda files, `Mesh_Panda.obj` (the object), `Tex_Panda.png` (the texture), and the `panda-laugh` (the sound clip), into Unity by dragging the Panda Mesha file and Panda object file into the Project Window in Unity, under Assets > Models.
![Drag Panda Files into Unity](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step2.png)


Step 4. Drag mesh panda to the Hierarchy window and confirm that the Panda is now showing on the scene as seen below.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step3.png)


Step 5. Add texture to the Panda. Right click in Assets Folder and create Material. Let's simply name the Material `Panda`. Then, right click Maerial to attach texture to the Material. In the right panel Inspector, you can see that the the texture is now applied to the left of Albedo. 


Step 6. Drag the Material on the the Panda Mesh in the scene. Now we see that the panda has material applied. This panda now has the skin of a panda.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step4.png)


Step 7. Attach the sound file to the Mesh Panda. Screenshot 5. Add the sound file to the Panda. In the right panel Inspector, you can see that the Mesh Panda model now has a Audio Source of panda laugh.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step5.png)


Step 8. Now let's create a prefab for the Mesh Panda. Drag Mesh_Panda into the Prefabs folder and Unity will create Prefabs.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step6.png)


Step 9. Assign Asset Bundle prefab is in. Change the Asset Bundle. See in the lower right cordern, add title `laughing panda` to the Asset Bundle.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step7.png)


Step 10. We click on laughing panda we have the Mesh Panda and has all dependencies in it. A manifest file is automatically created. You should see the following manifest file. Manifest file is automatically generated and it should be same as below. The manifest file for the Panda Asset Bundle needs to be create manually via template. Opening in the manifest file in a text editor should show the below json.

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

Step 12. In the Asset Bundles tab, click on Build button and define the Output Path for laughing panda. You can leave Advanced Settings as defaults.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step8.png)


Step 13. When you've defined the Output Path and ready to Build, click on horizonatal Build button, and Unity will build the laughing panda.

Step 14. Find the exported launghing panda at the Output Path. We are done creating an asset bundle called laughing panda. This panda looks like a panda and can laugh as we attached a sound file as an Audio Source.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step9.png)


Step 16. In One Game client storage, put the laughing panda here. Open One Game and push to asset server. We will allow you to be able to sell or distribute your Asset Bundle in our Asset Store in the future where you can make money and sell or distribute your creations.

Step 17. You can also use the Asset Bundle, `laughing panda` right away locally in One Game. Below, we see the panda now in a scene in One Game.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step10.png)



