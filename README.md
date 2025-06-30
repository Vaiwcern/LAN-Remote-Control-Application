# LAN Remote Control Application

A university project for the *Computer Network* course (Semester 4, HCMUS).

This application allows a client machine to remotely control a server machine within the same LAN network. It is implemented in **C++** using the **MFC** framework and communicates via **sockets** using the **TCP protocol** at the transport layer.

<table>
  <tr>
    <td align="center">
      <img src="assets/ui-6-buttons-enabled.png" alt="Main UI" width="300"/><br/>
      <em>Main UI</em>
    </td>
    <td align="center">
      <img src="assets/diagram-client.png" alt="Client Diagram" width="300"/><br/>
      <em>Client Diagram</em>
    </td>
    <td align="center">
      <img src="assets/diagram-server.png" alt="Server Diagram" width="300"/><br/>
      <em>Server Diagram</em>
    </td>
  </tr>
</table>

## ✨ Features

- Connect to the server using an IP address and port.
- Display information about processes running on the server.
- Display information about active applications.
- Capture and view the screen of the server machine.
- Log key presses on the server machine.
- Browse the directory tree of the server machine.
- 
## 🔌 Connect Server and Client

To connect the client to the server, users must enter the correct **IP address** and **port number** in the connection dialog. Below are example screenshots of the connection process:

<table>
  <tr>
    <td align="center">
      <img src="assets/ui-dialog-connect.png" alt="Connect Dialog" width="280"/><br/>
      <em>Connect Dialog</em>
    </td>
    <td align="center">
      <img src="assets/ui-dialog-connect-failed.png" alt="Connect Failed" width="280"/><br/>
      <em>Connection Failed</em>
    </td>
    <td align="center">
      <img src="assets/ui-dialog-connect-successful.png" alt="Connect Successful" width="280"/><br/>
      <em>Connection Successful</em>
    </td>
  </tr>
</table>

When connecting between **two different machines on the same local network**, the client must know the **IP address of the server**. This address can be obtained by running the `ipconfig` command in **Command Prompt** on the server machine. The default port number is **6666**, as pre-defined in the source code.

If both the client and server are running on the **same machine**, users can either use the actual IP address or simply enter the **loopback address `127.0.0.1`**. This special IP refers to the local machine itself, allowing internal communication without going through a physical network.


## 🎥 Demo Video

<a href="https://youtu.be/bAyCufM2_0o" target="_blank">
  <img src="https://img.youtube.com/vi/bAyCufM2_0o/hqdefault.jpg" alt="Watch the video" width="480">
</a>

## 🚀 Usage

To run the application, download and run the following files:

- `Server/x64/Debug/Server.exe`
- `Client/x64/Debug/Client.exe`

Make sure both client and server are on the same local network.
