Install:
ros-indigo-usb-cam
ros-indigo-ar-track-alvar

Calibrate camera and save yaml to
~/.ros/camera_info/head_camera.yaml

Publish
rosrun tf static_transform_publisher 0 0 0 0 0 0 odom usb_cam

Run
roslaunch usb_cam usb_cam-test.launch
roslaunch ar_cam.launch

View
rostopic echo /visualization_marker
