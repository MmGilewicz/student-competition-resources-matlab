# How to Run the Self Driving Stack 🪧 <!-- omit in toc -->

## Description <!-- omit in toc -->

Please use the following guide to run the Self Driving Stack after completing the [Virtual Software Setup Guide](./Virtual_MATLAB_Software_Setup.md) or the
[Manual Software Setup Guide](./Virtual_MATLAB_Manual_Software_Setup.md):

- [Running the Self-Driving Stack Resources](#running-the-self-driving-stack-resources)
- [MATLAB Setup Real Scenario](#matlab-setup-real-scenario)
- [Learning the Self-Driving Stack](#learning-the-self-driving-stack)

## Running the Self-Driving Stack Resources

Follow the below instructions to make sure everything is set up correctly and learn how to use the provided resources:

1. Using MATLAB navigate to the `/student-competition-resources-matlab/Virtual_MATLAB_Resources/self_driving_stack_resources` (make sure you double -click on folders and don't expand them)

2. Open QLabs and navigate to `Self-Driving Car Studio` => `Plane`

    ![qlabs plane](../Pictures/plane_world_qlabs.png)

3. Run the `Setup_Competition_Map.m` script

    - Make sure the `spawn_location` variable is `1` (top of the script)

    It should look like this after running the script:

    ![competition map](../Pictures/qlabs_setup_competition_map.png)

4. Open `QCar2_Virtual_calibrate.slx`

5. Use 'Monitor & Tune' to run the model

    ![competition map](../Pictures/monitor_and_tune.png)

6. Change `spawn_location` to `2` in the `Setup_Competition_Map.m` script

7. Run `Setup_Competition_Map.m` to spawn the QCar in the taxi hub area

8. Run `Setup_QCar2_Params.m`

9. Open `VIRTUAL_self_driving_stack_v2.slx`

10. Use 'Monitor & Tune' to run the model

    ![competition map](../Pictures/monitor_and_tune.png)

You should see the QCar begin to complete a lap of the outside-most lane as shown below (sped up):

![1 lap self drivning stack](../Pictures/1_lap_self_driving_stack.gif)

If something is not working correctly, please double-check that you have gone through the steps correctly. If the issue persists, you may raise an issue in the [Issues tab](https://github.com/quanser/student-competition-resources-matlab/issues)

## MATLAB Setup Real Scenario

A more realistic traffic scenario is provided through the [`Setup_Real_Scenario.m`](../Virtual_MATLAB_Resources/self_driving_stack_resources/Setup_Real_Scenario.m) file. This script spawns signage and traffic lights. This script runs CONTINUOUSLY in a loop to control the traffic lights, so it will need to be run in a separate MATLAB session from the `VIRTUAL_self_driving_stack_v2.slx`. To open another session of matlab, you will need to right-click on the MATLAB icon and select your version of MATLAB again.

## Learning the Self-Driving Stack

Once everything is confirmed and working, you can take a look at the [development guide](./Virtual_MATLAB_Development_Guide.md).
