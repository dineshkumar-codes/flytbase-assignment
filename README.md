# FlytBase Assignment: Square and Triangle Trajectory

This repository contains Python applications that control a drone to follow square and triangle trajectories. The applications/python script utilizes the FlytBase platform to interface with the drone and send commands for navigation.

## Prerequisites
Before running the application, ensure that you have the following:
- Laptop with Ubuntu 14.04 or above (You can also use a VM)
- [FlytSim Docker setup](https://github.com/flytbase/flytsim-docker/releases/)
- Basic knowledge of Python and Linux commands

## Installation
1. Clone this repository to your local machine or download the source code as a ZIP file and extract it.
2. Setup FlytSim by following this [guide](https://github.com/flytbase/flytdocs/blob/master/flytsim/flytsim-docker/setup.md).
3. Activate the license (Refer to this [instructions](https://github.com/flytbase/flytdocs/blob/master/flytsim/flytsim-docker/activation.md)).
4. Open a terminal inside the downloaded folder and run the following commands to copy the Python apps to the FlytSim docker container:
   ```shell
   docker cp square.py flytsim:/flyt/flytapps/
   docker cp triangle.py flytsim:/flyt/flytapps/
   ```

5. Now, get terminal access to FlytSim Docker by executing the `openshell.sh` script.

6. Once you are inside the FlytSim Docker, navigate to the `flytapps` directory and provide executable permissions for the Python scripts:
    ```shell
    chmod +x square.py
    chmod +x triangle.py
    ```   
7. Now run the following command to execute the Python script:
    ```shell
    python square.py
    python triangle.py
    ```

## Customization
If you wish to customize the application or add additional features, you can modify the square.py and triangle.py files as per your requirements. Here are a few possible modifications you can make:
- Adjust the side length or altitude values for the square or triangle trajectory.
- Implement other types of trajectories, such as circles or polygons.
- Integrate additional commands or behaviors for the drone during the trajectory.
