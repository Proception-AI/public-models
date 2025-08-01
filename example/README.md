# Hand Viewer

A simple MuJoCo viewer for ProHand models.

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
## Scenes

`left_hand_scene.xml`
- Loads the ProHand V17 left hand model

`right_hand_scene.xml`  
- Loads the ProHand V18R right hand model

`both_hands_scene.xml`
- Loads both left and right hand models

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