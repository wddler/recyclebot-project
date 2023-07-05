# recyclebot-project

## Expected Deliverables

1. **Dataset** containing:
    - RGB images with plastic packaging items as classes (such as bottles, bags, trays, pots, and tubs).
    - Hyperspectral images with seven plastic types as classes: PET, PE-HD, PVC, PE-LD, PP, PS, O.
2. **Demonstration setup**. Consists of:
    - Sensors.
        - RGB camera.
        - Hyperspectral camera.
    - Manipulator.
        - Delta, articulated, or SCARA.
    - Gripper.
        - Vacuum suction (single cup or an array with level compensation).
    - Conveyor belt

## Demonstrator

Expected functional flow:

- A bulk of plastic waste moves on the conveyor belt passing hyperspectral and RGB cameras towards the robot.
- The object detection model detects individual plastic items.
- The classification model classifies each plastic item.
- The command server creates a pick-and-place task for the robot based on the detection and classification models' outcomes.
- The robot executes the pick and place task and moves plastic items from the belt to relevant bins.

![Recyclebot Demonstrator](/img/demo-setup.jpg)
