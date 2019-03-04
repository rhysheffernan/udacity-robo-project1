# udacity-robo-project1

## How to run things...

### make 
```
$ cd ./build
$ cmake ../
$ make # You might get errors if your system is not up to date!
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/myrobot/build
```

### open world file and attach plugin

open the world file (in ./world)

Copy this code

```<plugin name="hello" filename="libhello.so"/>```
and paste it under

```<world name="default">```

### launch gazebo with the plugin

```cd /home/workspace/myrobot/world
gazebo myworld --verbose```

