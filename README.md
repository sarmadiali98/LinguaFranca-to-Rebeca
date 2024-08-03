# LinguaFranca-to-Rebeca
Welcome to the Lingua Franca to Rebeca Verification Repository! This repository is dedicated to showcasing and verifying the equivalence of models written in Lingua Franca (LF) and their corresponding counterparts in Rebeca. By providing side-by-side examples of LF code and its Rebeca translation, we aim to facilitate the understanding of how reactive systems can be modeled in these two languages. Feel free to explore the code examples, compare their functionalities, and use them as a reference for your own projects. Contributions and feedback are welcome to enhance the repository further.

## Sequential Composition
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a reactive system composed of nodes that communicate in a sequence. Each node in the system can send and receive messages, with the first node initiating communication with a predefined message. As messages are received, they are processed and forwarded to the next node. In the Rebeca model, when the last node in the sequence receives a message, it sends the same message to itself perpetually to avoid deadlock. This continuous self-message passing is necessary to maintain the flow, but it's not allowed in Lingua Franca since one output can't connect to more than one input.

<img width="143" alt="image" src="https://github.com/user-attachments/assets/ea06c69b-e8c6-49d0-b936-b9d30f7eaff4">
<img width="852" alt="image" src="https://github.com/user-attachments/assets/7d89d168-4af6-4fa9-a32b-9e5c8d33c1f9">

## Circular Network
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a reactive system where nodes periodically send a fixed message to the next node in a loop. Each node is configured with a specific period for sending messages and a network delay for message delivery. The first node initiates the communication cycle by sending a message with a predefined value. As each node receives a message, it simply records the received value and continues to send the same fixed message at its defined interval. The models illustrate how this periodic messaging system can be implemented in both Rebeca and Lingua Franca, providing a basis for verifying and understanding reactive system behaviors in different programming paradigms. The main reactor in both languages sets up a loop of nodes, ensuring continuous and periodic message passing.
<img width="795" alt="image" src="https://github.com/user-attachments/assets/a811352c-da6b-411a-b0d4-cdf5c5783955">


## Peer To Peer
This repository contains two models illustrating reactive systems in Rebeca and Lingua Franca. The first model demonstrates a simple reactive system where nodes communicate by sending and receiving messages that are doubled at each step. The first node initiates the communication with a value of 5, and each node sends the doubled message to the next node upon receiving it. The second model showcases a periodic message-passing system, where nodes send a fixed message at regular intervals defined by their period. Each node receives the message and continues the cycle. These models highlight how similar reactive systems can be expressed in Rebeca and Lingua Franca, providing a basis for comparison, verification, and educational purposes. The main reactors in both languages establish the connections between nodes, ensuring continuous communication in the network.
<img width="780" alt="Screenshot 2024-07-12 at 10 55 55 PM" src="https://github.com/user-attachments/assets/c1463bc9-fe53-4f9a-b796-9114f106f4e1">


## Car Brake
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a simplified automatic braking system in a car. The system comprises four main components: a Camera, Braking Assistant, Brake Pedal, and Brake. The Camera generates frames at regular intervals, which are processed by the Braking Assistant. Every tenth frame, the Braking Assistant triggers an automatic brake signal. Meanwhile, the Brake Pedal periodically simulates manual braking by sending a brake signal every second. Both automatic and manual brake signals are directed to the Brake component, which logs the activation and checks for deadlines to ensure timely responses. These models showcase how similar reactive systems can be modeled in Rebeca and Lingua Franca, facilitating a clear comparison and understanding of reactive programming concepts. The main reactors establish connections between components, ensuring coordinated operation of the braking system.
<img width="787" alt="Screenshot 2024-07-12 at 10 56 33 PM" src="https://github.com/user-attachments/assets/f78ce34d-b185-430a-9535-7cf1968b4c9d">

## Fork Network
This repository contains a Rebeca model and its equivalent in Lingua Franca, illustrating a simple communication system where a sender periodically transmits messages to two receivers. The sender, configured with a specific period, sends a message with a fixed value to both receivers after a defined network delay. Each receiver captures and stores the received message. These models demonstrate how a similar reactive system can be described in both Rebeca and Lingua Franca, providing a basis for verification and educational purposes. The main reactors in both languages establish the connections between the sender and receivers, ensuring the continuous and periodic message passing in the network.

<img width="746" alt="Screenshot 2024-07-15 at 6 08 41 PM" src="https://github.com/user-attachments/assets/bced78eb-8a94-464d-891d-8fcf0de3bf2a">

## Join Network
This repository contains a Rebeca model and its equivalent in Lingua Franca, demonstrating a simple communication system where two senders periodically transmit messages to a single receiver. In Rebeca, the Sender components send a message with a fixed value to the Reciever component after a defined network delay and period. The Reciever captures and stores the received message.

In Lingua Franca, due to the limitation that prevents connecting multiple inputs to the same port, the Reciever component is designed with two separate input ports. Each Sender component sends its message to a distinct port on the Reciever. This adjustment ensures that the system behaves as intended, with both senders successfully communicating with the single receiver. These models demonstrate how similar reactive systems can be implemented in both Rebeca and Lingua Franca, providing a basis for comparison and understanding of reactive programming concepts.

<img width="746" alt="Screenshot 2024-07-15 at 6 13 23 PM" src="https://github.com/user-attachments/assets/e437150e-1b74-4392-a9b0-324ed487a53b">


