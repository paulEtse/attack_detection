# Attack detection model
Attack detection tool in the two-tank benchmark
## requirements
> Matlab 2019<br>
> Simulink

## Execution
```
 open the project folder in matlab
 run the file run.m
 configure the simulation with the value of T1 leak rate, T2 leak rate etc.
 run the simulation by clicking on the lauch button
```
You can see the outputs in a scope the bloc residual circuits of the benchmark

## Description of the system
### Interface
The interface is used to simulate attacks. The user the select inputs and run the scenario.
- The leak rates are used to simulate a leak in each tank.
- The overflow rate affects the inlet flow in tank 1.
- The valve switch is used to open (on 1) or close the valve (on 0). The valve is stuck in a particular position when the stuck box is checked. 
- The pump, controller and sensor switches are used to simulate one of these components off. The default value is 1, which indicates that a component is working normally.
- The machine learning algo can be choose too.
The simulation time is 250s. The values are affected during the time interval attack_start and attack_end.
### Benchmark
The benchmark is the simulink app that is going to run simulation. it is designed by [[1]](#1). We modified it to get someting suitable to our system.
### Machine learning
The machine learning block must analyse system's behaviour to detect if there is an attack.

## Contact 
For any question you can contact :
* Emna Dhouib [dhouib@etud.insa-toulouse.fr](mailto:dhouib@etud.insa-toulouse.fr)
* Assa Diarra [diarra@etud.insa-toulouse.fr](mailto:diarra@etud.insa-toulouse.fr)
* Paul Etse [etse@etud.insa-toulouse.fr](mailto:etse@etud.insa-toulouse.fr)
* Richard Nedu [nedu@etud.insa-toulouse.fr](mailto:nedu@etud.insa-toulouse.fr)
*  Quentin Mouret [qmouret@etud.insa-toulouse.fr](mailto:qmouret@etud.insa-toulouse.fr)

## References
<a id="1">[1]</a> 
E. Chanthery, A. Subias (2020)
Diagnosis approaches for detection and isolation of
cyber attacks and faults on a two-tank system
[online](https://hal.laas.fr/hal-02439489/document)
