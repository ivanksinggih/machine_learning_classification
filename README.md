# Pickup Machine Error Detection

Source: https://www.kaggle.com/emilblixthansen/aicd-dataset
  
The machine is a pick-and-place machine, capable of handling many different shapes, sizes, and weights.  
The data are taken every 10 ms, most from the PLC tags.  
Because of the real industrial nature of the dataset, the information names are anonymised.  
  
Input and output data: about 96 features  
  
Input (some):  
5) sensor measurement: 'IO.ToolTemperature'  
8) operational setting: 'Sequence.SoftTouchActuator'  
28) operational setting: 'IO.VacuumValveON'  
31) operational setting: 'IO.SpeedVacuumMotor'  
38) operational setting: 'VacuumBlower.CMD.SpeedHz'  
39) operational setting: 'Vacuum.Stat.ActSpeedHz’  
41) operational setting: 'Actuator.Speed'  
42) operational setting: 'Actuator.CurrentSpeed'  
43) operational setting: 'Actuator.CurrentForce'  
47) sensor measurement: 'VibrationValue'  
52) operational setting: 'IO.LiftHeadSensor1NC'  
  
Output data:  
66) sensor measurement: 'Alarm.ItemDroppedError’  
(When the machine drops an item (variable 'Alarm.ItemDroppedError’ = 1), it is considered that an error occurs.)  

Analysis points:  
- Find priority of input factors  
- Summarizing the range of input variable values for normal and error cases (plot them), then find general differences, if possible.  
- Suppose that the machine is calibrated with new operational settings (we could create some noise/change in the operational input factors, we try to observe whether the machine will operate in normal or error state.
