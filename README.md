# robotics-icub
CW1 Robotics class at HW university for 2019. 
Important commands for Yarp and iCub simulator. 
- Run Yarp Server: 
yarpserver 
- Run iCub Simulator: 
iCub_SIM 
- Run motorgui for iCub: 
yarpmotorgui 
- View output from left camera: 
yarpview --name /view/left 
- Connect view port with camera on iCub: 
yarp connect /icubSim/cam/left /view/left 
- Show a video on the screen: 
yarpdev --device test_grabber --name /test/video --mode ball 
- Show a cam feed on the screen: 
yarpdev --device opencv_grabber --name /test/video 
- Connect a video to the screen: 
yarp connect /test/video /icubSim/texture/screen 
- Control the head joints: 
yarp rpc /icubSim/head/rpc:i
- Modify Head Joints Position: 
set pos 0 -60 

