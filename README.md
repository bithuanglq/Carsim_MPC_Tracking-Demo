## Language

- [En](README.md)
- [中](README_cn.md)

---

## Demo_Carsim_MPC_Tracking
A Carsim-Simulink demonstration of Model Predictive Control (MPC) for autonomous vehicle trajectory tracking showcases the integration of CarSim and Simulink to achieve MPC-based circular trajectory tracking for self-driving cars.

### Prerequisites
Version: MATLAB R2020a, CarSim 2020.0 [(install and link Simulink)](https://blog.csdn.net/Cynthia_2019/article/details/121953106), Windows 11  
Directory: root directory is _D:\CarSim2020\Carsim_Files_, include（_MPCtest1.mdl_, _MY_MPCController3.m_, _my_quadprog.m_），the root directory can be customized 
Please refer to the detailed [configuration process](issue/Readme.md).


### Run
1. Click 'Send to Simulink' in CarSim—Home, then automatically open Simulink. Click 'Run' in Simulink, wait for the completion of the simulation, and check the simulation results in Simulink
2. If you need to modify parameters in CarSim, such as vehicle parameters or simulation conditions, you should first 'Run Now' and then 'Send to Simulink.' If you are modifying parameters in Simulink, you only need to 'Run' within Simulink
3. Finally, in CarSim—Home—Analyze Results (Post Processing), click on 'Video+Plot' to view the CarSim simulation results.


### Results
Trajectory of the autonomous vehicle in Simulink:
<br>
 <div align="center">
  <img src="issue/Result_Simulink.png" alt="result" width="50%" height="50%" />
</div>
<br>
<br>
The trajectory of the autonomous vehicle in CarSim:
<br>

https://github.com/bithuanglq/Demo_Carsim_MPC_Tracking/assets/46642752/b69457a2-bf0a-4fab-8b71-9c14a14dddc8



### Where to modify
Modify the reference trajectory in MY_MPCController3.m for reference.


### Acknowlegement
Thanks to the book 'Model Predictive Control for Autonomous Vehicles' by Jianwei Gong for guidance.



