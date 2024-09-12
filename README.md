# LinguaFranca-to-Rebeca
Welcome to the Lingua Franca to Rebeca Verification Repository! This repository is dedicated to showcasing and verifying the equivalence of models written in Lingua Franca (LF) and their corresponding counterparts in Rebeca. By providing side-by-side examples of LF code and its Rebeca translation, we aim to facilitate the understanding of how reactive systems can be modeled in these two languages. Feel free to explore the code examples, compare their functionalities, and use them as a reference for your own projects. Contributions and feedback are welcome to enhance the repository further.

## Trigger-Activated Sequential Composition
![Trigger_Activated_Sequential_Composition](https://github.com/user-attachments/assets/bac0d89f-a5c7-46d8-bceb-ac8c2f06b951)

## Periodic Sequential Composition
![Periodic_Sequential_Composition](https://github.com/user-attachments/assets/a3c72dd0-1059-40d0-9436-214834044a37)

## Periodic Circular Composition

## Trigger Activated Circular Composition
![Trigger_Activated_Circular_Composition](https://github.com/user-attachments/assets/04b46704-a2b7-47cb-a9e4-32cec3811614)

## Trigger-Activated Ping Pong
![Trigger_Activated_PingPong](https://github.com/user-attachments/assets/89be335c-95f1-44dd-baac-73d6eaf3db1b)

## Periodic Ping Pong
![Periodic_PingPong](https://github.com/user-attachments/assets/c8ce8ef2-6e77-402f-81fe-658c87c1c04c)

## Periodic Fork Composition
![Periodic_Fork_Composition](https://github.com/user-attachments/assets/73cf1e8f-050d-4579-83b4-d594f78187f9)

## Periodic Join Composition
![Periodic_Join_Composition](https://github.com/user-attachments/assets/66279e94-8d19-4a57-ac7c-d3fc78d7f9a6)

## Car Brake
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a simplified automatic braking system in a car. The system comprises four main components: a Camera, Braking Assistant, Brake Pedal, and Brake. The Camera generates frames at regular intervals, which are processed by the Braking Assistant. Every tenth frame, the Braking Assistant triggers an automatic brake signal. Meanwhile, the Brake Pedal periodically simulates manual braking by sending a brake signal every second. Both automatic and manual brake signals are directed to the Brake component, which logs the activation and checks for deadlines to ensure timely responses. These models showcase how similar reactive systems can be modeled in Rebeca and Lingua Franca, facilitating a clear comparison and understanding of reactive programming concepts. The main reactors establish connections between components, ensuring coordinated operation of the braking system.

<img width="787" alt="Screenshot 2024-07-12 at 10 56 33 PM" src="https://github.com/user-attachments/assets/f78ce34d-b185-430a-9535-7cf1968b4c9d">
