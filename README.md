# LinguaFranca-to-Rebeca
Welcome to the Lingua Franca to Rebeca Verification Repository! This repository is dedicated to showcasing and verifying the equivalence of models written in Lingua Franca (LF) and their corresponding counterparts in Rebeca. By providing side-by-side examples of LF code and its Rebeca translation, we aim to facilitate the understanding of how reactive systems can be modeled in these two languages. Feel free to explore the code examples, compare their functionalities, and use them as a reference for your own projects. Contributions and feedback are welcome to enhance the repository further.

## Trigger-Activated Sequential Composition
![Trigger_Activated_Sequential_Composition](https://github.com/user-attachments/assets/bac0d89f-a5c7-46d8-bceb-ac8c2f06b951)

## Periodic Sequential Composition

![Periodic_Sequential_Composition](https://github.com/user-attachments/assets/a3c72dd0-1059-40d0-9436-214834044a37)

## Periodic Circular Composition

<img width="962" alt="image" src="https://github.com/user-attachments/assets/c0ece28e-47c9-4dfe-9cad-b1f1192d7563">

## Trigger Activated Circular Composition


<img width="1051" alt="image" src="https://github.com/user-attachments/assets/f3d8d2b6-89ad-4991-8dea-6ee3e48501db">

## Trigger-Activated Ping Pong


<img width="778" alt="image" src="https://github.com/user-attachments/assets/24f63060-2eb3-46a2-85ed-0534b51c54e7">

## Periodic Ping Pong


<img width="786" alt="image" src="https://github.com/user-attachments/assets/a17a3939-1084-4f73-8a75-60b669f2c48f">

## Periodic Fork Composition

<img width="620" alt="image" src="https://github.com/user-attachments/assets/c9588cf0-cc08-4171-b84d-99751f13e70b">

## Periodic Join Composition


<img width="467" alt="image" src="https://github.com/user-attachments/assets/f7a1da4e-91bc-457b-85e6-f6daeff46ce6">

## Car Brake
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a simplified automatic braking system in a car. The system comprises four main components: a Camera, Braking Assistant, Brake Pedal, and Brake. The Camera generates frames at regular intervals, which are processed by the Braking Assistant. Every tenth frame, the Braking Assistant triggers an automatic brake signal. Meanwhile, the Brake Pedal periodically simulates manual braking by sending a brake signal every second. Both automatic and manual brake signals are directed to the Brake component, which logs the activation and checks for deadlines to ensure timely responses. These models showcase how similar reactive systems can be modeled in Rebeca and Lingua Franca, facilitating a clear comparison and understanding of reactive programming concepts. The main reactors establish connections between components, ensuring coordinated operation of the braking system.

<img width="787" alt="Screenshot 2024-07-12 at 10 56 33 PM" src="https://github.com/user-attachments/assets/f78ce34d-b185-430a-9535-7cf1968b4c9d">
