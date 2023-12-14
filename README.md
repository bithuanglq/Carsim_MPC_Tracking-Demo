## Demo_Carsim_MPC_Tracking
**One Carsim-Simulink Demo of self-driving car trajectory tracking based on MPC**，展示了如何联合CarSim和Simulink来实现无人车MPC跟踪圆形轨迹。

### 配置
软件版本：MATLAB R2020a, CarSim 2020.0[（安装并关联Simulink）](https://blog.csdn.net/Cynthia_2019/article/details/121953106), Windows 11  
路径配置：根目录D:\CarSim2020\Carsim_Files，子文件（MPCtest1.mdl, MY_MPCController3.m, my_quadprog.m），根目录可以自定义  

> CarSim 配置

CarSim新建Procedure为newSplit Mu， 新建Run Control with Simulink的Models为MPCtest1，最终Home页面如下：  
<div align="center">
  <img src="issue/Carsim_Home.png" alt="result" width="40%" height="40%" />
</div>
Procedure、Models配置如下：  
<div align="center">
  <img src="issue/Carsim_Procedure.png" alt="result" width="40%" height="40%" />
</div>
<div align="center">
  <img src="issue/Carsim_Models.png" alt="result" width="40%" height="40%" />
</div>
在Models中，新建输入MPCtest1 input，输出MPCtest1 output，配置如下： 
<div align="center">
  <img src="issue/Carsim_Models_Import.png" alt="result" width="40%" height="40%" />
</div>
 <div align="center">
  <img src="issue/Carsim_Models_Export.png" alt="result" width="40%" height="40%" />
</div>

> Simulink 配置

Simulink 文件打开如下：  
 <div align="center">
  <img src="issue/Simulink.png" alt="result" width="40%" height="40%" />
</div>

### 运行
1. 点击CarSim--Home中的Send to Simulink，自动打开Simulink后点击Run，等待运行完成，查看Simulink仿真结果
2. 如果需要改动CarSim中的参数如车辆参数、仿真工况，则需要先Run Now再Send to Simulink；如果改动Simulink的参数，只需要在Simulink中Run
3. 最后在CarSim--Home--Analyze Results (Post Processing)中点击Video+Plot，查看CarSim仿真结果


### 结果
Simulink中无人车的轨迹： 
 <div align="center">
  <img src="issue/Result_Simulink.png" alt="result" width="40%" height="40%" />
</div>
CarSim中无人车的轨迹：  
<video width="40%" height="40%" controls>
  <source src="issue/Result_CarSim.mp4" type="video/mp4">
</video>

### 改进
参考轨迹在MY_MPCController3.m中修改


### Acknowlegement
参考自龚建伟著《无人驾驶车辆模型预测控制》

