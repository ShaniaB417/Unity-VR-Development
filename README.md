# VR Room Project

<img width="1128" alt="Screenshot 2024-08-13 at 4 54 48 PM" src="https://github.com/user-attachments/assets/ec89a8ef-53d6-443d-b2fe-248d5da1d956">
<img width="1120" alt="Screenshot 2024-08-13 at 4 55 12 PM" src="https://github.com/user-attachments/assets/e2f712ad-53d5-4660-952a-f61484de1441">
<img width="1008" alt="Screenshot 2024-08-13 at 5 16 52 PM" src="https://github.com/user-attachments/assets/cd851ff9-723c-426a-9ad4-b492c2f606f1">

## Overview

This project is part of the Unity VR Developer Pathway. The VR Room Project focuses on creating an immersive, fully interactive virtual reality experience using Unity and C#. The room features detailed 3D models, user interactions, and a thoughtfully designed environment that allows users to navigate and interact within the VR space.

## Features

- **Interactive Environment:** Users can interact with various objects in the room, such as opening doors, picking up items, and manipulating objects.
- **Immersive Design:** The room is designed with realistic lighting, textures, and sound effects to create an immersive experience.
- **Intuitive Navigation:** The project includes teleportation-based navigation to enhance user comfort and reduce motion sickness.
- **Cross-Platform Support:** The project is optimized for various VR platforms, including Oculus and HTC Vive.

## VR Principles Utilized

- **Spatial Audio:** Implemented 3D sound to enhance the sense of presence and immersion.
- **Interaction Design:** Used natural interactions such as grabbing, pushing, and pulling to create a more intuitive user experience.
- **Comfort & Usability:** Integrated teleportation to minimize VR motion sickness, ensuring a comfortable experience for the user.
- **Optimization Techniques:** Applied various optimization strategies such as level of detail (LOD) management and batching to ensure smooth performance.

## Performance Analysis

### Preface
In this section, I analyze the current performance metrics of the VR Room Project to evaluate its efficiency and responsiveness at this point in the project. The data was gathered during runtime, capturing CPU and GPU utilization, display performance, and CPU core distribution. These insights help identify areas where optimization is effective and where further improvements could be made.


<img width="974" alt="Screenshot 2024-08-13 at 4 56 31 PM" src="https://github.com/user-attachments/assets/e90ae1cb-4720-4415-be88-4f7dc624a878">

### 1. CPU & GPU Utilization

#### Graph Description
The top graph displays the percentage utilization of both the CPU and GPU over time.

#### Observations
- **CPU Utilization:** The CPU usage hovers between 40% and 60%, showing that the VR application is moderately demanding on the CPU. There is a small peak, likely due to a specific operation or scene in the application that required more processing power.
- **GPU Utilization:** The GPU utilization remains consistent, ranging from 20% to 50%, indicating that the VR application is not overly demanding on the GPU.

#### Impact
- **Performance Balance:** The relatively low GPU utilization suggests that the application is well-optimized for graphics, and there is likely room for more complex visual effects or higher resolution without significantly impacting performance.
- **CPU Load:** The moderate CPU usage indicates that the application can handle additional CPU-intensive tasks, but there is a need to monitor and optimize to avoid potential bottlenecks, especially in more complex scenes.

### 2. Display Performance


#### Graph Description
The middle graph shows display metrics including the display refresh rate, average frame rate, early frame count, stale frame count, and minimum vsyncs.

#### Observations
- **Display Refresh Rate:** The refresh rate is consistently at 72 Hz, which is typical for VR headsets, ensuring smooth visuals.
- **Average Frame Rate:** The average frame rate is consistently at 73 FPS, which is slightly above the refresh rate, indicating that the application maintains a stable and smooth frame rate, which is crucial for VR comfort.
- **Early & Stale Frames:** There are no early or stale frames recorded, indicating that frames are being rendered and displayed in a timely manner without delays or drops.
- **Minimum Vsyncs:** The minimum vsyncs count remains at 1, showing that the application successfully synchronizes with the display refresh rate, preventing screen tearing.

#### Impact
- **Smooth Experience:** The consistent frame rate and lack of frame drops or delays ensure a comfortable and immersive VR experience, reducing the risk of motion sickness.
- **Performance Efficiency:** The synchronization with the display refresh rate indicates that the application is efficiently utilizing the available hardware, providing a balanced and optimized experience.

### 3. CPU Core Utilization

#### Graph Description
The bottom graph displays the utilization percentage across different CPU cores over time.

#### Observations
- **Core Distribution:** The workload is distributed across multiple cores, with core utilization ranging from 20% to 70%. The graph shows that some cores are more heavily utilized than others, with occasional peaks in certain cores.
- **Load Balancing:** There is variability in core utilization, which may indicate that certain tasks are more parallelizable than others, or that some operations are more CPU-bound.

#### Impact
- **Parallel Processing:** The application appears to take advantage of multi-threading, spreading tasks across several cores, which helps in maintaining performance stability and responsiveness.
- **Potential Optimization:** The varying core utilization suggests that there could be opportunities to further optimize load balancing, ensuring that no single core becomes a bottleneck during more demanding tasks.

### Overall Performance Analysis
- **Optimization:** The application is well-optimized, maintaining a stable and smooth frame rate while effectively utilizing both CPU and GPU resources. The balanced load across CPU cores and the efficient use of GPU suggest that the application has been designed with performance in mind.
- **User Experience:** With consistent frame rates and a lack of frame drops or screen tearing, the VR experience is likely to be comfortable and immersive, minimizing the risk of discomfort for users.
- **Future Considerations:** While the current performance is strong, further optimizations could focus on enhancing load balancing across CPU cores and exploring more advanced visual effects to fully utilize GPU capacity.
