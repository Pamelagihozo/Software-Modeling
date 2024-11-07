Gishushu Traffic Lights System Specification

State: Green
Description: Allows vehicles to proceed through the intersection.
Duration: Usually 60 seconds.
Transition Condition: After 60 seconds, the system transitions to Yellow.
Pedestrian Mode Check: The system waits until the Green cycle completes and then moves to Red to allow pedestrians to cross.

State: Yellow
Description: Signals vehicles to prepare to stop.
Duration: 5 seconds.
Transition Condition: After 5 seconds, the system transitions to Red. 
The system will proceed to Red after Yellow ends.

State: Red
Description: All vehicles must stop at the intersection and pedestrians can cross the road
Duration: Usually 60 seconds.
Transition Condition: After 60 seconds, it transitions back to Green.

State: Pedestrian Mode
Description: This is where the lights to enter a pedestrian crossing mode.
Duration: Pedestrian crossing is active for 20 seconds.
Transition Condition: After 20 seconds, the system returns to its normal sequence by moving to Green if it was initiated from Green or resuming from where it left off if interrupted mid-cycle.

State: Emergency Mode
Description: Activates flashing yellow lights to indicate caution due to an emergency or a malfunction in the traffic light system.
Transition Condition: Maintains continuous flashing yellow until the emergency is cleared. Once cleared, the system returns to the Green state.
