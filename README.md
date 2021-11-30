# MoRe Modena Racing - Aeromap for VI-Grade simulation

This repository is made to create an aeromap file for VI-Grade and make an accurate simulation of a FSAE vehicle.
There are two tipes of scripts, AER Standard and AER Advanced. The main difference between the two is that AER Advanced scripts require more input than AER Standard, and thus outputs more precise data.


## AER Standard

The Standard AER file contains aero maps as functions of front and rear ride heights:

    - front downforce
    - rear downforce
    - drag force

The maps resolution and extension is customizable, but it is strongly recommended that the maps are defined for
all the ride heights combination allowed by the ride height saturation boundaries. Standard and user defined units could be used to define the maps.
NOTE: the user-defined unit tags are not supported within tables. They are accepted for single value parameters only.

## AER Advanced

The Advanced AER file contains:

    - front and rear downforce
    - front and rear side force
    - drag force
    - rolling torque
    - pitch torque

The maps resolution and extension is customizable, but it is strongly recommended that the maps are defined for all the ride heights combination allowed by the ride height saturation boundaries. Standard and user defined units could be used to define the maps.
NOTE: the user-defined unit tags are not supported within tables. They are accepted for single value parameters only.

ATTENTION: the 1.0 file format is now deprecated, you need to use the 2.0 version or convert your 1.0 file to 2.0 file