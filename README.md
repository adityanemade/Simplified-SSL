# Simplified SSL

Simplified SSL creates a connection between the client and server to exchange encrypted messages using RSA algorithm.

### Prerequisites

You need to have Java 8+ in your system. If not then you can download it from
[https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

### Installation

Clone the repository. Then open command prompt and create class files for the java files.

    javac RSA.java
    javac Client.java
    javac Server.java
Then in the same command prompt run the Server.

    java Server
Open another command prompt run the Client.

    java Client
Now test using sample messages whether everything is running perfectly.

### Testing

After completing the installation and the Server and Client are running.
Send a message from the command prompt of the client and check whether you receive it on the Server end and vice versa.

### Deployment

For deployment you need to follow same steps as for installation. Compile Server and RSA in one computer. Start the Server on that computer. Take another computer and before compiling Client and RSA on that just make one change i.e. add the Server's ip address and port number accordingly in the void main of Client.java.

    Client client = new Client("127.0.0.1", 3445);
Then compile Client and RSA and run Client.
