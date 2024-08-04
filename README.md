# LinguaFranca-to-Rebeca
Welcome to the Lingua Franca to Rebeca Verification Repository! This repository is dedicated to showcasing and verifying the equivalence of models written in Lingua Franca (LF) and their corresponding counterparts in Rebeca. By providing side-by-side examples of LF code and its Rebeca translation, we aim to facilitate the understanding of how reactive systems can be modeled in these two languages. Feel free to explore the code examples, compare their functionalities, and use them as a reference for your own projects. Contributions and feedback are welcome to enhance the repository further.

## Trigger-Activated Sequential Composition
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a reactive system composed of nodes that communicate in a sequence. Each node in the system can send and receive messages, with the first node initiating communication with a predefined message. As messages are received, they are processed and forwarded to the next node. In the Rebeca model, when the last node in the sequence receives a message, it sends the same message to itself perpetually to avoid deadlock. This continuous self-message passing is necessary to maintain the flow, but it's not allowed in Lingua Franca since one output can't connect to more than one input.

<img width="852" alt="image" src="https://github.com/user-attachments/assets/7d89d168-4af6-4fa9-a32b-9e5c8d33c1f9">

## Periodic Sequential Composition
This is the same as trigger-activated sequential composition, except that the action of sending a message is not triggered by receiving a message from the previous node, but rather by a timer every second.

<img width="929" alt="image" src="https://github.com/user-attachments/assets/1d2f7a10-92db-4cce-81ae-91acfa4b80c8">

## Periodic Circular Composition
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a reactive system where nodes periodically send a fixed message to the next node in a loop. Each node is configured with a specific period for sending messages and a network delay for message delivery. The first node initiates the communication cycle by sending a message with a predefined value. As each node receives a message, it simply records the received value and continues to send the same fixed message at its defined interval. The models illustrate how this periodic messaging system can be implemented in both Rebeca and Lingua Franca, providing a basis for verifying and understanding reactive system behaviors in different programming paradigms. The main reactor in both languages sets up a loop of nodes, ensuring continuous and periodic message passing.

<img width="962" alt="image" src="https://github.com/user-attachments/assets/c0ece28e-47c9-4dfe-9cad-b1f1192d7563">

## Trigger Activated Circular Composition

This is the same as periodic circular composition, except that the action of sending a message is triggered by receiving a message from the previous node, instead of a timer every second.

<img width="1051" alt="image" src="https://github.com/user-attachments/assets/f3d8d2b6-89ad-4991-8dea-6ee3e48501db">

## Trigger-Activated Ping Pong

This repository contains two models illustrating reactive systems in Rebeca and Lingua Franca. The first model demonstrates a simple reactive system where nodes communicate by sending and receiving messages. The first node initiates the communication with a value of 1, and each node sends the same message to the next node upon receiving it. The second model showcases the same message-passing system, where nodes send a fixed message upong being triggered. Each node receives the message and continues the cycle. These models highlight how similar reactive systems can be expressed in Rebeca and Lingua Franca, providing a basis for comparison, verification, and educational purposes. The main reactors in both languages establish the connections between nodes, ensuring continuous communication in the network.

<img width="778" alt="image" src="https://github.com/user-attachments/assets/24f63060-2eb3-46a2-85ed-0534b51c54e7">

## Periodic Ping Pong

This is the same as trigger-activated Ping Pong, except that the action of sending a message is not triggered by receiving a message from the previous node, but rather by a timer every second.

<img width="786" alt="image" src="https://github.com/user-attachments/assets/a17a3939-1084-4f73-8a75-60b669f2c48f">

## Periodic Fork Composition
This repository contains a Rebeca model and its equivalent in Lingua Franca, illustrating a simple communication system where a sender periodically transmits messages to two receivers. The sender, configured with a specific period, sends a message with a fixed value to both receivers after a defined network delay. Each receiver captures and stores the received message. These models demonstrate how a similar reactive system can be described in both Rebeca and Lingua Franca. The main reactors in both languages establish the connections between the sender and receivers, ensuring the continuous and periodic message passing in the network.

<img width="620" alt="image" src="https://github.com/user-attachments/assets/c9588cf0-cc08-4171-b84d-99751f13e70b">

## Periodic Join Composition
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a simple communication system where senders periodically transmit messages to a single receiver. In Rebeca, the Sender components send a message with a fixed value to the Reciever component after a defined network delay and period. The Reciever captures and stores the received message.

In Lingua Franca, due to the limitation that prevents connecting multiple inputs to the same port, the Reciever component is designed with two separate input ports. Each Sender component sends its message to a distinct port on the Reciever. This adjustment ensures that the system behaves as intended, with both senders successfully communicating with the single receiver. These models demonstrate how similar reactive systems can be implemented in both Rebeca and Lingua Franca, providing a basis for comparison and understanding of reactive programming concepts.

<img width="467" alt="image" src="https://github.com/user-attachments/assets/f7a1da4e-91bc-457b-85e6-f6daeff46ce6">

## Car Brake
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a simplified automatic braking system in a car. The system comprises four main components: a Camera, Braking Assistant, Brake Pedal, and Brake. The Camera generates frames at regular intervals, which are processed by the Braking Assistant. Every tenth frame, the Braking Assistant triggers an automatic brake signal. Meanwhile, the Brake Pedal periodically simulates manual braking by sending a brake signal every second. Both automatic and manual brake signals are directed to the Brake component, which logs the activation and checks for deadlines to ensure timely responses. These models showcase how similar reactive systems can be modeled in Rebeca and Lingua Franca, facilitating a clear comparison and understanding of reactive programming concepts. The main reactors establish connections between components, ensuring coordinated operation of the braking system.

<img width="787" alt="Screenshot 2024-07-12 at 10 56 33 PM" src="https://github.com/user-attachments/assets/f78ce34d-b185-430a-9535-7cf1968b4c9d">
