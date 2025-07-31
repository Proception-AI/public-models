# Hand Viewer

A simple MuJoCo viewer for ProHand models with joint control.

## Usage

The hand viewer accepts command line arguments to select which scene to load:

```bash
# View left hand only
python hand_viewer.py left

# View right hand only  
python hand_viewer.py right

# View both hands
python hand_viewer.py both
```

## Features

- **Scene Selection**: Choose between left hand, right hand, or both hands
- **Ground Plane**: Each scene includes a textured ground plane for better visualization
- **Joint Control**: Use the MuJoCo viewer's Control tab to manipulate joints
- **Stable Physics**: Gravity is disabled so hands stay stable unless controlled
- **Proper Camera**: Each scene has optimized camera positioning

## Scenes

### `left_hand_scene.xml`
- Loads the ProHand V17 left hand model
- Positioned above a ground plane
- Optimized camera angle for single hand viewing

### `right_hand_scene.xml`  
- Loads the ProHand V18R right hand model
- Positioned above a ground plane
- Optimized camera angle for single hand viewing

### `both_hands_scene.xml`
- Loads both left and right hand models
- Hands positioned side by side above ground
- Wider camera angle to view both hands

## Controls

1. Run the script with your desired scene
2. In the MuJoCo viewer, switch to the "Control" tab
3. Use the sliders to control joint positions
4. Press ESC to exit

## Requirements

- Python 3.7+
- MuJoCo 3.3.0+
- GLFW
- PyOpenGL
- NumPy

Install dependencies with:
```bash
pip install -r requirements.txt
``` 