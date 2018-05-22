---
layout: single
sidebar:
  nav: "docs"
---

### Step by Step Basic Tutorial for Creating Laughing Panda Asset Bundle
-------------------------------------------------------------------------

Step 1: [Download Unity](https://unity3d.com/get-unity/download)


Step 2: Download the Panda files from Google Poly [here](https://poly.google.com/view/2T6A0o4Kq2h) or get the Panda from this git repository [here](https://github.com/OneGameFoundation/docs/tree/master/assets/Mesh_Panda).

Step 3: Import the Panda files into Unity by dragging the Panda Mesha file and Panda obj into unity - step 1 photo.
Into the project window in Unity.

![Drag Panda Files into Unity](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step1.png)


Step 4. Unity add panda voice (sound clip). 
Step 2 photo with a sound file panda-laugh 
![Add sound file panda-laugh](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step2.png)





Step 5. Drag mesh panda to the Hierarchy window and confirm that the Panda is now showing on the scene. 

Step 6. Add texture to the Panda. Right cck in Asset Folder and create Material and call Panda. Attach texture to the material. Screen shot 3 with texture applied. 

![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step3.png)


Step 7. Drag the material on the the panda mesh. Now we see that the panda has material applied. Screenshot 4.
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step4.png)



Step 8. Attach the sound file to the Mesh Panda. Screenshot 5. Add the sound to the laugh. 
![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step5.png)


Step 9. Create prefab for the. Drag Mesh_pange into the Prefabs folder and it will create Prefabs. Screenshot 6. 

![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step6.png)


Step 10. Assign Aset Bundle prefa  b is in. Change the Asset Bundle. Adding title Laugh Panda to the Asset Bundle. Screenshot 7.

![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step7.png)


Step 11. Open the Asset Bundle Browser. We clic on Laught pand we have tis Mesh Panda and has all dependencies in it. A manifest file is automatically created. You should see the following manifest file. 

Step 12. Manifest file is automatically generated and it should be same as below. The manifest file for the Panda Asset Bundle needs to be create manually via template.

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

Step 13. We click build and define the output path for laughing panda. 

![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step8.png)


Step 14. Build and unity will build the laughing panda for us.

Step 15. Find the exported launghing panda at the build folder. 

![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step9.png)


![Panda](https://raw.githubusercontent.com/OneGameFoundation/docs/master/assets/screenshots-laughing-panda/screenshot-step10.png)



Step 16. One Game client storage, put the laughing panda here.

Step 17. Open One Game and push to server.  You can also use the Asset bundle right away locally in One Game.



