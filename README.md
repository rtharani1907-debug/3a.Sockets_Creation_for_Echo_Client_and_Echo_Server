# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
```
DEVELOPED BY: THARANI RAMESHBABU           REG NO: 212225240170
```
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
```
client side:

import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
  msg=input("Client > ") 
  s.send(msg.encode()) 
  print("Server > ",s.recv(1024).decode())

server side:

import socket 
s=socket.socket() 
s.bind(('localhost',8000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
  ClientMessage=c.recv(1024).decode() 
  c.send(ClientMessage.encode())
```
## OUPUT
<img width="1920" height="1080" alt="Screenshot (560)" src="https://github.com/user-attachments/assets/b51a211c-0bbf-4547-bdcb-6dde0c3deefc" />
<img width="1920" height="1080" alt="Screenshot (561)" src="https://github.com/user-attachments/assets/8ac29ef6-9376-447a-b13d-19e13a2e07c3" />

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
