category: control  
signature: vexcodeInit();  
description: Initializes devices added using the Robot Configuration tool.

# vexcodeInit();

`vexcodeInit();` is used to setup and initialization devices configured in the Robot Configuration tool. 

`The vexcodeInit();` should always run at the start of your "int main" function to ensure that your devices are configured before running any other commands.

Removing or commenting `vexcodeInit();` out can result in devices not working properly and/or unexpected behaviors when you run your project.

<advanced>
</advanced>