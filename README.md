# AlertNap
 Drowsiness Detection &amp; Alert System: Using advanced AI methodologies, this project developed in collaboration with IBM utilizes driver drowsiness detection techniques. Leveraging IBM Cloud for data loading and storage, and Node-RED for integration, the system detects driver drowsiness and promptly alerts them via voice and text messages.
## Inspiration
Automotive population is increasing exponentially in the country. The biggest problem regarding the increased traffic is raising number of road accidents. Driver sleepiness, alcoholism and carelessness are key players in accident scenario. Taking into account of these factors the driver behaviour state is major challenge for designing advanced driver assistants systems. Driver drowsiness detection is a car safety technology which prevents accidents when driver is getting drowsy. Driver in attention is might be the result of lack of alertness when driving due to drowsiness and distraction. The system alerts driver through alarm in real time.Driver when losing his focus while driving by feeling drowsy, yawning or taking his eyes off the road, is said to be distracted and it can prove to be chaotic to any passengers, pedestrians and the goods on the vehicle. As a result, one of the reasons behind vehicle accidents is due to the negligence

## What it does
1 Problem Statement (Problem to be solved):
Drowsiness detection is a safety technology that can prevent accidents that are caused by drivers. Driver's inattention might be the result of a lack of alertness when driving due to driver drowsiness and distraction. Driver distraction occurs when an object or event draws a person's attention away from the driving task.
 2 Idea / Solution description:
 Many of the road accidents will occur due to drowsiness of the driver. Drowsiness can be detected by monitoring the driver through continuous video stream with a camera. The general objective is to create a model thatwill indicate whether a person is feeling drowsy or not. The model takes image for every second and check for eye blinking and calculate the time for eye closed . If the blinking is high and eye is closed for certain amount of time then it will indicate driver through a sound. 
3 Novelty / Uniqueness:
 In case if the driver met with an accident, it automatically notifies their family members and also contact nearby hospitals. 
4 Social Impact / Customer Satisfaction :
Number of accidents can be reduced. As the person can contact the hospitals soon so there is high possibility of chances that person can be saved. 
5 Business Model (Revenue Model):
 The government can take initiative to implement this system mandatorily in every vehicle 
6 Scalability of the Solution :
This solution has a high scalability as it doesn’t have any work load and work well in all situations.

## How we built it
The drowsiness detection and alert system was built using computer vision techniques and deep learning libraries. We utilized OpenCV and specifically the Dlib library for facial recognition and processing of images captured by Raspberry Pi cameras. The captured data was processed on the Raspberry Pi acting as an edge device. We integrated IBM Watson IoT cloud, storing the processed data in a Cloudant database through Node-RED, a programming tool provided by IBM. Notifications were sent via the Telegram messaging application using a Node-RED bot.
*State: Not Drowsy (Eyes opened)*
![image](https://github.com/shruthi2608/AlertNap/assets/99944438/1abe76e8-17fb-4d51-a41a-265d4020895b)
*State: Drowsy (Eyes closed)*
![image](https://github.com/shruthi2608/AlertNap/assets/99944438/a9575e46-1a5d-4545-92ba-4ef10b478e50)
*IBM Watson IOT Configuration*
![image](https://github.com/shruthi2608/AlertNap/assets/99944438/10cc34d2-f32c-4c45-a176-2565262541a5)
*Node Red Dashboard output for drowsiness(Status = 1)*
![image](https://github.com/shruthi2608/AlertNap/assets/99944438/fc8b7f5c-8562-4a6f-b7cd-29288744dc43)
*Node Red Dashboard output for awake(Status = 0)*
![image](https://github.com/shruthi2608/AlertNap/assets/99944438/ace74c7f-e7f4-4cd9-9ce9-52a5f493f25b)
*NodeRed Flow*
![image](https://github.com/shruthi2608/AlertNap/assets/99944438/722527fb-12f3-40a5-953b-f1478704bd33)

## Challenges we ran into
During the development process, we encountered challenges such as selecting the most accurate and efficient library for facial recognition, which led us to choose Dlib. Additionally, optimizing the processing on the Raspberry Pi to achieve real-time performance was a challenge. Integrating the hardware with the IBM Cloud and ensuring seamless communication between the edge device and the cloud services also required careful attention.

## Accomplishments that we're proud of
We are proud of successfully integrating the IBM Cloud into our project and leveraging its capabilities for data storage and real-time monitoring. Collaborating with an esteemed company like IBM provided valuable resources and expertise, enhancing the project's overall quality and reliability. The implementation of the drowsiness detection and alert system, which combines advanced AI methodologies with edge computing, showcases our ability to address critical safety concerns in real-world scenarios.

## What we learned
Through this project, we gained practical experience in computer vision, deep learning, and edge computing technologies. We learned to leverage OpenCV libraries effectively for facial recognition and image processing. The integration with IBM Cloud, specifically the Watson IoT Platform and Node-RED, expanded our knowledge of cloud-based services and their seamless integration with edge devices. We also developed skills in real-time monitoring, data storage, and event logging, contributing to our understanding of building end-to-end AI applications for driving safety.

## What's next for AlertNap
The future scope for AlertNap is promising, as there is a growing need for effective solutions to combat drowsy driving andprevent accidents caused by driver fatigue. Future systems can leverage emerging sensor technologies, such as infrared cameras, eye-tracking devices, and biosensors, to enhance drowsiness detection accuracy. These sensors can monitor various physiological and behavioral indicators of drowsiness, including eye movements, blink patterns, facial expressions, heart rate, and brain activity.Future systems can provide real-time monitoring and feedback to the driver. For example, they can use audio or visual cues to alert the driver when drowsiness is detected, encouraging them to take a break or engage in activities that promote alertness, such as opening the windows or playing stimulating music.

## YouTube link
https://youtu.be/yadyrNbW3EA
