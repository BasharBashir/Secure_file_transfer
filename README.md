# Fast Secure File Transfer
This project presents the development of a new file transfer application that uses the TCP protocol with sliding window technology. The application is designed for client-server communication and aims to provide a fast, reliable, and secure way to transfer files. The project is divided into two parts. In the first part, a client requests a file from other connected clients and establishes peer-to-peer connections with those clients to retrieve the file. The client also determines the bandwidth available for file transfer and requests the file in chunks based on this information. The connected clients encrypt and send the requested chunks to the client, who then verifies the integrity of the received file. In the second part of the project, a client sends a file to all connected clients using peer-to-peer connections. The file is first compressed to reduce its size, and then processed and encrypted before being sent to the clients. Each client receives a different chunk of the file and immediately sends it to the other clients, while also processing and decrypting the received chunk. The sender and receiver clients verify the transferred file using a secure hashing algorithm. Overall, this project aims to provide a reliable and efficient way to transfer files in a client-server environment, utilizing the benefits of peer-to-peer communication.

# How to run 
1)To run the application, you will need to download the JavaFX library and add it to the build path of your clients and server. Start by obtaining the JavaFX library from the official Oracle website or a suitable repository.
 After downloading JavaFX, extract the contents of the library to a preferred location on your computer. Next, open the Eclipse IDE 2020 and create a new Java project for your application.
 
2)Configure the build path by right-clicking on the project in the Project Explorer, selecting "Build Path," and then "Configure Build Path." In the Libraries tab of the Configure Build Path window, click on "Add External JARs" or "Add Library" (depending on your Eclipse version).
 Navigate to the location where you extracted the JavaFX library, select the appropriate JAR files, and add them to the build path of your project. Additionally, you will need to set up the JavaFX runtime in Eclipse.

3)Go to the Run Configurations of your Eclipse project  Access the Arguments tab. In the VM arguments section ,add the following line, replacing the path with the actual location of the JavaFX runtime on your system:
                    --module-path /path/to/javafx-sdk-VERSION/lib --add-modules javafx.controls,javafx.fxml


