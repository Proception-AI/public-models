# ProHand Models

This repository contains the models files for the ProHand model (MJCF format). The repository includes both left and right hand variants with convex and capsule collision models.

## Example Usage

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd public-models
   ```

2. Install the required dependencies:
   ```bash
   cd test
   pip install -r requirements.txt
   ```

3. View the ProHand models in MuJoCo:
   ```bash
   # View left hand
   python hand_viewer.py left
   
   # View right hand
   python hand_viewer.py right
   
   # View both hands
   python hand_viewer.py both
   ```

## Model Variants

### Left Hand (ProHand_L)
- **Convex Model**: `models/left/ProHand_L_convex.xml`
- **Capsule Model**: `models/left/ProHand_L_capsule.xml`

### Right Hand (ProHand_R)
- **Convex Model**: `models/right/ProHand_R_convex.xml`
- **Capsule Model**: `models/right/ProHand_R_capsule.xml`

## Note on Meshes

Visual meshes contain optimized geometry for realistic rendering:
- **Finger segments**: High-detail optimized meshes
- **Palm and wrist**: Detailed surface geometry
- **Thumb assembly**: Specialized thumb kinematics

Collision meshes contain simplified geometry for fast physics:
- **Convex models**: Convex hull approximations
- **Capsule models**: Simplified capsule-based geometry
- **Optimized for**: Real-time collision detection

## Scene Configuration

The `test/scenes/` directory contains pre-configured scene files:
- `common_scene.xml` - Shared elements (ground, lighting, camera)
- `left_hand_scene.xml` - Left hand with ground plane
- `right_hand_scene.xml` - Right hand with ground plane
- `both_hands_scene.xml` - Both hands positioned side by side

## License

This project contains ProHand models and associated assets. Please refer to the original model licenses for usage terms.

## Contact

For questions or support, please contact the maintainers of this repository.
