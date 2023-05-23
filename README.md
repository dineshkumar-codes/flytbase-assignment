# FlytBase Assignment: Square and Triangle Trajectory

This repository contains Python applications that control a drone to follow square and triangle trajectories. The applications/python script utilize the FlytBase platform to interface with the drone and send commands for navigation.

## Prerequisites
Before running the application, ensure that you have the following:
- Laptop with Ubuntu 14.04 or above (You can also use a VM)
- [FlytSim Docker setup](https://github.com/flytbase/flytsim-docker/releases/)
- Basic knowledge of Python and Linux commands

## Installation
1. Clone this repository to your local machine or download the source code as a ZIP file and extract it.

2. Make sure FlytSim is up and running (Refer to this setup [guide](https://docs.flytbase.com/flytsim/flytsim-docker/setup)).

3. Open a terminal inside the downloaded folder and run the following commands to copy the Python apps to the FlytSim docker container:
   ```shell
   docker cp square.py flytsim:/flyt/flytapps/
   docker cp triangle.py flytsim:/flyt/flytapps/
   ```

4. Now, get terminal access to FlytSim Docker by executing the `openshell.sh` script.

5. Once you are inside the FlytSim Docker, navigate to the `flytapps` directory and provide executable permissions for the Python scripts:
    ```shell
    chmod +x square.py
    chmod +x triangle.py
    ```   
6. Now run the following command to execute the Python script:
    ```shell
    python square.py
    python triangle.py
    ```

## Customization
If you wish to customize the application or add additional features, you can modify the square.py and triangle.py files as per your requirements. Here are a few possible modifications you can make:
- Adjust the side length or altitude values for the square or triangle trajectory.
- Implement other types of trajectories, such as circles or polygons.
- Integrate additional commands or behaviors for the drone during the trajectory.

## Contributing
If you'd like to contribute to this project, you can follow these steps:
- Fork the repository on GitHub.
- Create a new branch with a descriptive name for your feature or bug fix.
- Make the necessary changes in your branch.
- Commit your changes with clear and concise commit messages.
- Push your branch to your forked repository.
- Submit a pull request detailing your changes and describing their purpose.

## Disclaimer
Please note that operating a drone requires expertise and adherence to local regulations. Ensure that you have the necessary knowledge and permissions to operate a drone safely and legally in your area. The authors of this repository are not responsible for any misuse or illegal activities involving drones.
