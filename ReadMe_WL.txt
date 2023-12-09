dustynv/ros:humble-desktop-l4t-r35.4.1 this docker image support jetson inference and ros humble desktop:

./docker/run.sh --container dustynv/ros:humble-desktop-l4t-r35.4.1 --volume /home/orin/study/ros/docker_ws:/home/ros_ws
docker build -f Dockerfile.ros.humble -t dustynv/ros:humble-desktop-python3-venv-l4t-r35.4.1 .
docker build --no-cache -f Dockerfile.ros.humble2 -t dustynv/ros:humble-desktop-python3-venv-l4t-r35.4.1 .
./docker/run.sh --container dustynv/ros:humble-desktop-python3-venv-l4t-r35.4.1 --volume /home/orin/study/ros/docker_ws:/home/ros_ws

docker build --no-cache -f Dockerfile-desktop -t jeguzzi/robomaster_ros:humble-desktop .

docker build --no-cache -f Dockerfile.ros.humble2 -t jeguzzi/robomaster_ros:humble-desktop .

./docker/run.sh --container jeguzzi/robomaster_ros:humble-desktop --volume /home/orin/study/ros/docker_ws:/home/ros_ws

ubuntu22.04:humble-desktop
./docker/run.sh --container ubuntu22.04:humble-desktop --volume /home/orin/study/ros/docker_ws:/home/ros_ws


docker build -f Dockerfile.ros.humble4 -t ubuntu:humble-desktop-slam-ign-gazebo .


./docker/run.sh --container ubuntu22.04:humble-desktop-slam-ign --volume /home/orin/study/ros/docker_ws:/home/ros_ws
