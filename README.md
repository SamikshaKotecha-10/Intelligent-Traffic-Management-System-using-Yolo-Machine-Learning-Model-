# Intelligent-Traffic-Management-System-using-Yolo-Machine-Learning-Model-
   **Need of smart control of traffic signals** 
1. The condition of urban traffic is becoming one of the critical issues with increasing population and automobiles in cities
2. Traffic jams not only causes extra delay and stress for the drivers but also increase fuel consumption, add transportation cost and increase carbon dioxide air pollution.
3. There can be different causes of congestion in traffic like insufficient capacity unrestrained demand large red light delays etc,. 
4. The traffic lights are one of the critical factors affecting traffic flow.
   
   **Drawbacks of conventional systems**
1. The manual controlling system requires a large number of manpower.
2. Conventional traffic lights uses a timer for every phase which is fixed and does not adapt according to the real time traffic on that road.
3. Electronic sensors i.e. proximity sensors or loop detectors, the accuracy and coverage are often in conflict because the collection of high quality information is usually based on sophisticated and expensive technologies and thus limited budget will reduce the number of facilities.

   **Proposed system**
 The traffic flow has no specific pattern that is followed, and the static signal timers pose a huge problem to the already critical problem of congestion.
   Therefore, implementing a system which aims to reduce chances of such scenarios by automatically computing the optimal green signal time based on the current traffic at the signal will ensure that the direction with more traffic is allotted a green signal for longer duration of time as compared to the direction with lesser traffic.
   This system can override the older system of hard coded lights, which causeway unwanted delays, reducing congestion and waiting time, which will reduce the number of accidents and fuel consumption which in turn will help in controlling air pollution.

   **Main objective of the project**
 The main objective of this project is to design a traffic light controller based on computer vision that can adapt to the current traffic situation. Our proposed system aims to use live video feed from cctv camera at traffic junctions for real time traffic density calculation by detecting the vehicles at the signal and set the green signal time accordingly. The vehicles are classified as car, bike, bus or truck or rickshaw to obtain a more accurate estimate of the green signal time.

   **Advantages of proposed system**
1.Real time traffic signals switching according to current traffic density.
2.Virtually no new hardware to be installed.
3.Less expensive than sensors.
4.Autonomous, no need of manpower.

  **Proposed system model**
Our proposed system will pass a snapshot from the CCTV cameras at traffic junctions for realtime traffic density calculation using image processing and computer vision. 
We are using customized YOLO (you only look once) model for object detection in order to detect vehicles.
The scheduling algorithm will use this traffic density and appropriately set the optimal green signal time for each signal and update the red signal times of the other signals.

  **Some of the factors considered in the signal switching algorithm.**
1. The processing time of the algorithm to calculate traffic density.
2. The number of lanes.
3. Lag each vehicle suffers during startup.
4. The nonlinear increase in lag suffered by the vehicles which are at the back.
5. The maximum and minimum green signal time that can be set. This is done to prevent starvation of the lane with less traffic.
