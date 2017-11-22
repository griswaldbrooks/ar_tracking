Install:
ros-kinetic-usb-cam
ros-kinetic-ar-track-alvar

Calibrate camera and save yaml to
~/.ros/camera_info/head_camera.yaml

Publish
rosrun tf static_transform_publisher 0 0 0 0 0 0 odom usb_cam

Run
roslaunch ar_cam.launch

View
rostopic echo /visualization_marker
