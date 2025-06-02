# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
### Echo-server.py
```
import socket


HOST = "127.0.0.1"  
PORT = 65432  


with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
    s.connect((HOST, PORT))
    s.sendall(b"Hello, world")
    data = s.recv(1024)


print(f"Received {data!r}")
```

### Echo-client.py
```
import socket


HOST = "127.0.0.1"  
PORT = 65432  


with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
    s.connect((HOST, PORT))
    s.sendall(b"Hello, world")
    data = s.recv(1024)


print(f"Received {data!r}")
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/7a60e010-6e01-464f-b78f-6a54c5f6867b)

## RESULT:
The program is executed successfully
