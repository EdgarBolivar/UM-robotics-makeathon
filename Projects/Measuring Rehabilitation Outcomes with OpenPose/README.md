# Measuring Rehabilitation Outcomes with OpenPose
For Prosthetists and Orthotists, it is important to measure objective rehabilitation outcomes to asses patient progress. These rehabilitation outcomes typically include specific metrics of the human lower-limb kinematics, such as step length, cadence, and Range of Motion (RoM) of the joints. These metrics are available using motion capture analysis, e.g., using [Vicon](https://www.vicon.com/) or [XSens](https://www.xsens.com/). However, the cost of these systems makes these kind of analyses prohibitive for most clinicians. **The objective of this project is to create an open-source tool to analyse human lower-limb kinematics from video recordings taken from a smartphone.** Fortunately, we can leverage the results from the [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) project to materialize this objective!
# The challenge
## Easy
* Estimate ROM of the knee and ankle joints from a video recording. Offline or real-time estimation is valid.
* Auto-generate a pdf file that reports the mean, median, maximum, and minimum ROM for each joint for the complete length of the video.
## Medium (includes objectives at easy level)
* Calculate the step length and cadence.
* Include the mean, median, maximum, and minimum step lengths and cadences in the pdf report.
* Include a plot of the joint angle vs. time for the knee and ankle joints. Select a time window that is easy for visualization and is representative of the data.
## Spicy (includes objectives at medium level)
* Fragment the joint angles of the knee and ankles in multiple time windows. Each time window should include exactly one gait cycle.
* Include a violin plot to report the statistics of the ROM, step length, and cadence.
* Create a real-time video that shows in parallel the motion of the patient with the skeleton from OpenPose, the joint angle vs. time for the knee and ankle, and the statistical information from the the data currently in display.

# Resources
1. Webcam 1080P HD.
1. RPi-4 (?)

# Constraints
1. Develop the tool for Windows 10/8. Our alpha test will be to deploy our tool at the UM-Orthotics and Prosthetic Center ([UMOPC](https://www.uofmhealth.org/our-locations/south-industrial-op)).  The UMOPC will have access only to Windows machines. (Optional, it may be possible to use a debian-based system. Ask your mentor about the possibility of implementation in RPi-4.)
