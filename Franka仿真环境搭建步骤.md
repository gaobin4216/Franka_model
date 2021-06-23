#1. 在ros环境下将panda_arm.urdf.xacro转化为urdf文件
    rosrun xacro xacro panda_arm.urdf.xacro> FRANKA.urdf --inorder
#2. 用blender建模软件将Franka的三维描述文件转换为stl格式，因为matlab只能调stl格式
#3. 将stl文件导入solidworks并实体化，可以装配得到机器人的三维模型
        
----------

#使用方法:
###simulink
    smimport('FRANKA_simu.urdf')
###Robotics Toolbox
    robot=importrobot('FRANKA_tool.urdf')
    show(robot)

