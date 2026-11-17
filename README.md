LAN File Drop

Project Overview

LAN File Drop is a file transfer application developed using C programming and TCP socket programming.

It allows a sender application to transfer multiple files to a receiver application over a network.

Features

- TCP socket communication.
- Sender and receiver applications.
- Multiple file transfer.
- File name and file size transmission.
- Error handling.
- File validation.
- File transfer using Winsock2.

Technologies Used

- Programming Language: C
- Networking: TCP Socket Programming
- Network Library: Winsock2
- Compiler: GCC
- IDE: Visual Studio Code
- Operating System: Windows 11

Project Structure

LAN_File_Drop/
│
├── sender/
│   ├── sender_file.c
│   ├── sender.c
│   ├── sample.txt
│   ├── notes.txt
│   └── document.txt
│
├── receiver/
│   ├── receiver_file.c
│   └── receiver.c
│
├── received_files/
│
├── .gitignore
└── README.md

Compilation

Compile the receiver:

gcc .\receiver\receiver_file.c -o receiver_file.exe -lws2_32

Compile the sender:

gcc .\sender\sender_file.c -o sender_file.exe -lws2_32

How to Run

1. Start the receiver application first:

.\receiver_file.exe

2. Open another terminal and start the sender:

.\sender_file.exe

3. The sender transfers the files to the receiver.
4. The received files are saved inside the "received_files" folder.

Sample Output

Sender:

Connected to Receiver!
File sent: sample.txt
File sent: notes.txt
File sent: document.txt
All files sent successfully!

Receiver:

Receiver is waiting for file...
Sender connected!
Number of files to receive: 3
File received: sample.txt
File received: notes.txt
File received: document.txt
All files received successfully!

Learning Outcomes

Through this project, I practiced:

- C programming.
- TCP socket communication.
- Client-server architecture.
- File handling using C.
- Sending and receiving data.
- Error handling and input validation.

Author
Ashwitha punna

Developed as a C programming and networking project.