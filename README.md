# Real-time-Chatting-application

# Project Overview:
The project I developed is a desktop-based chatting application created using Java. The primary goal of this project is to provide a simple yet effective means of communication between two clients, much like the desktop version of WhatsApp. The application leverages Java Swing for its graphical user interface (GUI) and Java Socket programming to manage the communication between the clients.

===============================================================================================================================

# User Interface Design:
For the graphical user interface, I used Java Swing. This involved creating a main application window using JFrame, where I set up the frame size using the setSize method and made it visible with setVisible(true). I also positioned the frame on the screen using setLocation. To enhance the user experience, I customized the background color of the frame with setBackground and used a JPanel to organize various UI components, such as text fields for message input, and buttons for sending messages, making calls, and starting video chats. Icons were added to these buttons to provide a familiar and user-friendly interface.

=================================================================================================================================

# Socket Programming:
The core functionality of the application relies on Java Socket programming. I implemented two main classes: the server class and the client class. The server class uses a ServerSocket to listen for incoming client connections. Once a connection is accepted using skt.accept(), the server can communicate with the client using DataInputStream to receive messages and DataOutputStream to send messages. The client class is responsible for connecting to the server, also using socket programming, and handles the sending and receiving of messages in a similar manner.
Message Handling:In the server class, I employed an infinite loop (while(true)) to continuously listen for and accept new client connections. This loop ensures that the server can handle multiple messages in real time. The messages received by the server are displayed on the left side of the chat window, while the messages sent from the client appear on the right side. To handle user actions such as clicking the send button, I implemented action listeners that capture the user's input and trigger the appropriate response.

================================================================================================================================


# Challenges and Learning Outcomes:
Throughout the development of this project, I encountered several challenges, particularly in synchronizing messages between the server and clients and ensuring the GUI updates in real time. These challenges provided valuable learning opportunities, enhancing my understanding of both Java Swing for GUI development and Java Socket programming for network communication. This project helped me gain practical experience in building a real-time communication application and improved my problem-solving skills.
