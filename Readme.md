# Rotating the Gaming Object

## Aim
To develop a 3D application for rotating the gaming objects in Unity.

## Algorithm

**Step 1:** Start  

**Step 2:** Click File → Scene → Select the scene → Save as → New folder (Scenes) → File name (Expno1)  

**Step 3:** Click Hierarchy → 3DObject → Cylinder, Hierarchy → 3DObject → Capsule, Hierarchy → 3DObject → Text, Hierarchy → 
Effects → Particle system  

**Step 4:** Create a folder in Project and name it `Materials`.  
- `Materials` folder → Create → Material (Name: Cylinder) → Inspector → Surface Inputs → BaseMap (Choose color) → Drag the Cylinder to the plane.  
- `Materials` folder → Create → Material (Name: Capsule) → Inspector → Surface Inputs → BaseMap (Choose color) → Drag the Capsule to the plane.  

**Step 5:** Click Hierarchy → Directional Light → Inspector → Change the color to white (255, 255, 255).  

**Step 6:** Create a folder named `Coding` and add a C# file to it.  

**Step 7:** To add our C# Script file to our selected object, drag the script to the objects in the Hierarchy window and run the application.  

**Step 8:** Stop  

## Program

```csharp
using UnityEngine;

public class NewMonoBehaviourScript : MonoBehaviour
{
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        transform.RotateAround(Vector3.left, Vector3.up, 40 * Time.deltaTime);
    }
}

```
## Output

Assets/Screenshot 2025-08-19 091822.png

## Result

Hence, the 3D application for rotating the gaming objects in Unity is developed.


