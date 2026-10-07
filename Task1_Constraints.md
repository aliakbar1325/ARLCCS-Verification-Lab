ARLCCS – Software Verification Lab
Automated Railway Level-Crossing Control System
Task 1 – Constraints
ID
Constraint (simple English)
Reason
C1
The barrier must not be open while a train is present in the crossing.
Open barriers would let road traffic enter the path of the train.
C2
Warning lights and alarm must be active whenever a train is approaching or present.
Road users need visual and audible warning before and during the passage.
C3
The barrier must be closed whenever a train is present in the crossing.
Physically blocks the road for the entire train passage.
C4
The barrier may open only after the train is confirmed to have completely cleared the crossing.
Prevents opening while the tail of the train is still in the crossing.
C5
The road traffic signal must be red whenever the barrier is not fully open.
Keeps drivers from entering a closing/closed crossing.
C6
Warning lights and alarm must be on before the barrier starts closing.
Gives vehicles time to clear and avoids trapping them.
C7
If a sensor fault is detected, the system must enter fail-safe mode.
A blind system cannot know whether a train is coming; it must assume danger.
C8
If a barrier fault is detected, the control center must be alerted and road signal must be red.
Operators must dispatch help or warn the train driver; drivers must be told to stop.
C9
If communication is lost, the system must enter fail-safe mode and must not open the barrier.
Without communication, train status cannot be trusted.
C10
If an emergency is declared, barriers must close (or stay closed) and the alarm must be on.
Emergencies require the safest, most restrictive state.
C11
The barrier must not close on a vehicle that is inside the crossing (it must be held/raised safely or an alert raised).
Avoid trapping or crushing a vehicle in the crossing.
C12
A train must not be reported as cleared while Train_Present is still true.
Contradictory state data would cause premature opening.
C13
The warning signals must not turn off while the barrier is not fully open.
Drivers may assume the crossing is safe when it is not.
