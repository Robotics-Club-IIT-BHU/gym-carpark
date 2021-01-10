# AUTONOMOUS CAR PARKING

Autonomous parking management through Multi-Agent Reinforcement Learning.

<p align="center">
 <img  width="400" height="250" src="https://github.com/Robotics-Club-IIT-BHU/gym-carpark/blob/main/media/parking.gif">
 <img  width="400" height="250" src="https://github.com/Robotics-Club-IIT-BHU/gym-carpark/blob/main/media/full-parking.png"><br>
</p>

## Installation Guidelines

Before installing this arena, you need to download certain modules on which it is dependent. We **strongly** recommend using a distribution of **Linux** as your operating system for this event. Windows installations tend to be a hassle and require, in some instances, quite a bit of time and effort to complete.

0. Although not compulsory, we strongly recommend creating a virtual environment specific to this project. This will help in package management and for decluttering your workspace. A simple way to create a virtual environment is as follows:

   ~~~bash
   python3 -m venv <Env_Name>
   ~~~

   Activation and deactivation of your virtual environment, will be done as specified [here](https://docs.python.org/3/library/venv.html). Scroll down to the table where the activation method for various operating systems is provided. Deactivation, in most cases, can be done by simply typing deactivate while being in in the virtual environment.

1. Once you activate your virtual environment, you will have to install the various dependencies of this project. We have simplified this process for you. Just follow the following steps:
   * Download/Clone this repository on to your local machine.
   * Navigate to the root folder of this repository through your terminal.
   * Execute the following command in your terminal.

      ~~~bash
      pip install -e carpark-arena
      ~~~

In case there are problems with the PyBullet installation, you can refer to this [guide](https://github.com/Robotics-Club-IIT-BHU/Robo-Summer-Camp-20/blob/master/Part1/Subpart%201/README.md).

## Using the Arena

0. You will have to import the package vision_arena, which will be available only if you've completed step 1 in the Installation Guidelines. The arena can be initialized by using:

   ~~~python
   env = gym.make("carpark_arena-v0")
   ~~~

   gym.make() itself takes some arguments, which will be elaborated upon further.

1. Then, you will have to create the working loop, as is normally done in pybullet (using `stepSimulation()`).

2. The functions of the environment, available to you for various purposes, are as follows. Please go through the functions themselves in this [file](https://github.com/Robotics-Club-IIT-BHU/gym-carpark/blob/main/carpark-arena/carpark_arena/envs/simpleDrivingEnv.py), if you wish to know their arguments and/or return values.

3. You can also run the file **helper.py** to see the documentation of the different various functions.

4. An example of how the arena works is given in the file **manual_control.py**, which contains the mechanism for controlling the car manually, for testing purposes.
