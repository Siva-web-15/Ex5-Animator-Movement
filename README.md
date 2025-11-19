# Ex5-Animator-Movement

## Aim:
To develop a animator movement for a player using unity.

## Algorithm:
### Step 1:
Import necessary models.

### Step 2:
Right-click -> Create -> Animator Controller.

### Step 3:
Open Animator window, define states (Idle, Run, Jump, etc.).

### Step 4:
Use keyframes or Unity's Animation tools to animate transitions between states.

### Step 5:
Drag Animator Controller to the GameObject in the Inspector.


## Program:
**Developed by:** `Sivabalan M`<BR>
**Register Num:** `212224230269`

### Movement.cs
```csharp
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputX", InputX);
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputY", InputY);
    }
}
```



## Output:

<img width="1038" height="606" alt="image" src="https://github.com/user-attachments/assets/a9b85cfb-4cfe-40f5-994e-9721e6738ea0" />

## Result:

An animator movement for a player using unity is developed successfully.
