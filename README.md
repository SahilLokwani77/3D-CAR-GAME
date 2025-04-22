# 🚗 Unity Car Controller

A simple and realistic physics-based Car Controller made in Unity using `Rigidbody`. This script handles acceleration, braking, turning, and grounded checks using raycasting, making it a great foundation for racing or driving games.

## 🛠 Features

- Rigidbody-based movement
- Acceleration & reverse
- Realistic gravity when airborne
- Turning limited to when grounded
- Ground detection via raycast
- Speed cap
- Adjustable parameters for tuning

<pre> ## 📂 Project Structure <code> ProjectRoot/ ├── Assets/ │ ├── Scripts/ │ │ └── CarController.cs # The main car control script │ ├── Prefabs/ │ │ └── Car.prefab # (Optional) Car prefab with Rigidbody & script │ ├── Scenes/ │ │ └── SampleScene.unity # (Optional) Demo scene with car placed │ └── Materials/ # (Optional) Any custom materials used ├── ProjectSettings/ # Unity project settings ├── Packages/ # Unity package dependencies └── README.md # This readme file </code> </pre>


## 🚀 Getting Started

### Prerequisites

- Unity (2021.3 LTS or later recommended)
- Rigidbody component on your car object
- Input setup using Unity's default `Horizontal` and `Vertical` axes

### Setup

1. Create a GameObject for your car.
2. Add a `Rigidbody` component.
3. Attach the `CarController.cs` script.
4. Create an empty child GameObject (for ground detection) and assign it to `groundRayPoint`.
5. Assign the correct `LayerMask` to `whatIsGround`.

### Input

- `W` / `Up Arrow`: Accelerate
- `S` / `Down Arrow`: Reverse/Brake
- `A` / `Left Arrow`: Turn Left
- `D` / `Right Arrow`: Turn Right

## ⚙️ Public Parameters

| Variable         | Description                              |
|------------------|------------------------------------------|
| forwardAccel     | Forward acceleration force               |
| reverseAccel     | Reverse acceleration force               |
| maxSpeed         | Maximum speed of the car                 |
| turnStrength     | How fast the car turns                   |
| gravityForce     | Additional gravity applied when airborne |
| dragOnGround     | Drag applied when on the ground          |
| groundRayLength  | Length of ray to detect ground           |
| whatIsGround     | Layer mask to define what is ground      |
| groundRayPoint   | Point from which the ray is cast         |

## 📸 Preview

![image](https://github.com/user-attachments/assets/c9209435-a4c3-4c0b-bba8-595b6ca60121)


## 🧠 Ideas for Extension

- Add drift mechanics
- Add handbrake and tire skid effects
- Add camera follow script
- Multiplayer car racing
- Surface-based grip changes (e.g., ice, sand, asphalt)

## 📄 License

This project is open source and free to use under the MIT License.

---



