## Demo_Carsim_MPC_Tracking
**One Carsim-Simulink Demo of self-driving car trajectory tracking based on MPC**，展示了如何联合CarSim和Simulink来实现无人车MPC跟踪圆形轨迹。

### 配置
软件版本：MATLAB R2020a, CarSim 2020.0[（安装并关联Simulink）](https://blog.csdn.net/Cynthia_2019/article/details/121953106), Windows 11  
路径配置：根目录D:\CarSim2020\Carsim_Files，子文件（MPCtest1.mdl, MY_MPCController3.m, my_quadprog.m），根目录可以自定义  

> CarSim 配置

CarSim新建Procedure为newSplit Mu， 新建Run Control with Simulink的Models为MPCtest1，最终Home页面以及Procedure、Models配置如下：  
CarSim_Home.png  
CarSim_Procedure.png  
CarSim_Models.png  
在Models中，新建输入MPCtest1 input，输出MPCtest1 output，配置如下：  
CarSim_Models_Import.png  
CarSim_Models_Export.png  


> Simulink 配置

Simulink 文件打开如下：  
Simulink.png  


### 运行
1. 点击CarSim--Home中的Send to Simulink，自动打开Simulink后点击Run，等待运行完成，查看Simulink仿真结果
2. 如果需要改动CarSim中的参数如车辆参数、仿真工况，则需要先Run Now再Send to Simulink；如果改动Simulink的参数，只需要在Simulink中Run
3. 最后在CarSim--Home--Analyze Results (Post Processing)中点击Video+Plot，查看CarSim仿真结果


### 结果
Simulink中无人车的轨迹：  
Result_Simulink.png  
CarSim中无人车的轨迹：  
Result_CarSim.mp4  


