## This is a summary of the data we need: ##


### AER STANDARD: ###

    general parameters:
        [km/h]  car speed
        [kgpm3] air density at the track 
        [mm]    ride heights min and ride height max, front/rear

    aero parame:
        [mm]    drag arm height min and max TODO: verify what data program expects
        [N]     front and rear downforce (X,Y,Z)
        [N]     front and rear ride height drag (X,Y,Z)

### AER ADVANCED: ###

    general parameters:
        [kgpm3] air density at the track
        [mm^2]  car frontal area TODO: verify unit  (mm^2 or m^2)
        [mm]    drag arm height min and max TODO: verify what data exactly the program expects

    offset parameters:
        [km/h]  velocity threshold 
        [km/h]  velocity offset reference
        CZ
        BALANCE_Z TODO: verify what data program expects
        CX body/front/rear

    aero and dynamics parameters (body/front/rear and angles):
        yaw
        pitch
        roll 
        steering angle 
        front and rear ride height 
        wind effect (angle [deg] and speed[v


### EXAMPLES ###

    from: [FRONT_DOWNFORCE](XY_DATA))

        {front_ride_height downforce }
        10.0 400.0 400.0 400.0 400.0 400.0 400.0
        40.0 400.0 400.0 400.0 400.0 400.0 400.0
        80.0 400.0 400.0 400.0 400.0 400.0 400.0
        120.0 400.0 400.0 400.0 400.0 400.0 400.0
        140.0 400.0 400.0 400.0 400.0 400.0 400.0
        160.0 400.0 400.0 400.0 400.0 400.0 400.0

        (                                                       )
        | 10, 40, 80, 120, 140, 160   ----->  front_ride_height |
        | 400, 400, 400, ........     ----->  downforce         |
        (                                                       )