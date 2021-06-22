# Pickup Machine Error Detection

Source: https://www.kaggle.com/emilblixthansen/aicd-dataset
  
The machine is a pick-and-place machine, capable of handling many different shapes, sizes, and weights.  
The data are taken every 10 ms, most from the PLC tags.  
Because of the real industrial nature of the dataset, the information names are anonymised.  
  
Input and output data: about 96 features  
  
Input: sensor measurement(not considered), operational setting  
  
Operational setting input data:  
8) 'Sequence.SoftTouchActuator'(X)  
9) 'Sequence.WantedSoleHeight'  
17) 'BellowSoftTouch.AdjustStep'(X)  
18) 'BellowSoftTouch.iWantedDest'(X)  
28) 'IO.VacuumValveON'  
29) 'IO.VacuumValveOFF'(X)  
30) 'IO.BellowPressure'  
31) 'IO.SpeedVacuumMotor'(X)  
32) 'IO.SoleVacuum'(X)  
35) 'Status.ElementStatus’(X)  
36) 'Status.MachineStatus'(X)  
37) 'Statistics.SequenceNr'(X)  
38) 'VacuumBlower.CMD.SpeedHz'  
39) 'Vacuum.Stat.ActSpeedHz'  
41) 'Actuator.Speed'  
42) 'Actuator.CurrentSpeed'  
43) 'Actuator.CurrentForce'  
44) 'Actuator.CurrentPos'(X)  
45) 'Actuator.TargetPos'(X)  
46) 'Actuator.WantedBellowPressure’(X)  
48) 'IO.RakeForcedVacuumON'  
49) 'IO.RakeForcedVacuumOFF'(X)  
50) 'IO.ChangeOverValveON'  
51) 'IO.ChangeOverValveOFF'(X)  
52) 'IO.LiftHeadSensor1NC’ (X: same values)  
53) 'IO.LiftHeadSensor2NC' (X: same values)  
54) 'Operation.Setting.0'(X)  
76) 'Operation.Setting.15'(X)  
77) 'Operation.Setting.16'(X)  
78) 'Operation.Setting.17'(X)  
  
**[Note] (Selected input data characteristic: nominal data type (e.g., small = little amount, large = a lot of amount), not class type (e.g., class 1, class 2, …)**
  
Output data:  
66) sensor measurement: 'Alarm.ItemDroppedError’  
(When the machine drops an item (variable 'Alarm.ItemDroppedError’ = 1), it is considered that an error occurs.)  

Analysis points:  
- Find priority of input factors  
- Summarizing the range of input variable values for normal and error cases (plot them), then find general differences, if possible.  
- Suppose that the machine is calibrated with new operational settings (we could create some noise/change in the operational input factors, we try to observe whether the machine will operate in normal or error state.
