# Simulation of Ransomware Encryption and Prevention Strategies

## Overview

This project simulates a **ransomware encryption** system, designed to demonstrate how ransomware operates and to explore effective prevention strategies. The system uses advanced cryptographic techniques, including **Diffie-Hellman key exchange**, **ChaCha20 encryption**, and **AES encryption**, to simulate the encryption of files and folders on a victim's machine. The project also includes a **Graphical User Interface (GUI)** for both the attacker (controller) and the victim, allowing for a realistic simulation of ransomware behavior.

The primary goal of this project is to provide a platform for understanding ransomware attacks, testing prevention mechanisms, and developing strategies to mitigate such threats.
Here is code https://github.com/Sadatali9/Simulation-of-Ransomware-Encryption-and-Prevention-Strategies/releases/tag/v1.0.0
---

## Features

### Cryptographic Core
- **Diffie-Hellman Key Exchange**: Establishes a secure shared secret between the attacker and victim without transmitting the key directly.
- **ChaCha20 Encryption**: Provides high-speed encryption for secure communication between the attacker and victim.
- **AES Encryption**: Encrypts the victim's files and folders, simulating a real-world ransomware attack.

### Server Implementation (Victim Side)
- Manages multiple client connections using threading.
- Performs secure key exchange and encrypts/decrypts incoming and outgoing messages.
- Simulates ransomware behavior by encrypting files and folders on the victim's machine.

### Client Implementation (Attacker Side)
- **SecureCommunicationClient Class**: Handles secure communication setup, encryption, and decryption.
- **GUI Interface**: Built with **Tkinter** and **ThemedTk**, providing a user-friendly interface for the attacker to control the ransomware simulation.
  - Connection management (connect/disconnect).
  - Secure communication status display (keys and encryption mode).
  - File storage for received data and message logs.

### Data Targeting
- The ransomware can target specific files, folders, or entire drives for encryption, simulating a real-world attack scenario.
- The attacker can control the encryption process remotely, making the simulation more efficient and realistic.

---

## Technologies Used

- **Python**: The project is implemented in Python, leveraging its simplicity and extensive libraries for cryptography and GUI development.
- **Cryptography Libraries**:
  - **PyCryptodome**: Used for AES encryption and decryption.
  - **ChaCha20**: Provides high-speed encryption for secure communication.
  - **Diffie-Hellman**: Ensures secure key exchange between the attacker and victim.
- **Tkinter**: Used to build the GUI for both the attacker and victim interfaces.
- **Threading**: Enables concurrent handling of multiple client connections and tasks.

---

## Getting Started

### Prerequisites

- **Python 3.x**: Ensure you have Python 3.x installed on your machine. You can download it from [Python's official website](https://www.python.org/downloads/).
- **Required Libraries**: Install the necessary Python libraries using pip:
  ```bash
  pip install pycryptodome tkinter ttkthemes
  ```

### Running the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/ransomware-simulation.git
   cd ransomware-simulation
   ```

2. **Run the Server (Victim Side)**:
   - The server simulates the victim's machine and handles encryption/decryption tasks.
   - Run the server script:
     ```bash
     python server.py
     ```

3. **Run the Client (Attacker Side)**:
   - The client provides the attacker with a GUI to control the ransomware simulation.
   - Run the client script:
     ```bash
     python client.py
     ```

4. **Connect and Simulate**:
   - Use the client GUI to connect to the server (victim).
   - Perform actions such as file encryption, folder encryption, and drive encryption.
   - Monitor the encryption process and view the results in real-time.

---

## Project Structure

### Key Components

- **Server (Victim Side)**:
  - `server.py`: Manages the victim's machine, handles encryption/decryption, and communicates with the attacker.
  - `AESFileEncryption.py`: Implements AES encryption and decryption for files and folders.
  - `ChaCha20Encryptor.py`: Handles ChaCha20 encryption for secure communication.
  - `DiffieHelman.py`: Implements the Diffie-Hellman key exchange protocol.

- **Client (Attacker Side)**:
  - `client.py`: Provides the attacker with a GUI to control the ransomware simulation.
  - `SecureCommunicationClient.py`: Handles secure communication between the attacker and victim.
  - `RansomScreen.py`: Simulates the ransomware screen on the victim's machine.

---


## Future Enhancements

1. **Advanced Features**:
   - Implement two-factor authentication for added security.
   - Add support for file transfers with encryption.
   - Introduce a logging module for monitoring communication events.

2. **Scalability**:
   - Transition to a distributed architecture to handle multiple concurrent clients.

3. **Enhanced GUI**:
   - Integrate real-time message visualization tools.
   - Add themes and customization options for better user experience.

4. **AI Integration**:
   - Use AI for anomaly detection in communication patterns to identify potential security breaches.

5. **Cross-Platform Support**:
   - Develop mobile and web-based versions of the client application for broader accessibility.

---

## Protection Measures Against Ransomware

To safeguard systems and data from ransomware attacks, the following measures are essential:
- **Maintain System Security**: Ensure that built-in security features such as firewalls and real-time protection are enabled.
- **Adopt a Strict No-Trust Policy**: Avoid running unauthorized or cracked applications.
- **Ensure Regular Updates**: Keep your operating system, applications, and security tools up-to-date.
- **Implement Data Backups**: Regularly back up critical data to secure, offline, or cloud-based storage solutions.

---

## Conclusion

This project provides a comprehensive simulation of ransomware encryption and prevention strategies. By leveraging advanced cryptographic techniques and a user-friendly GUI, it offers a realistic platform for understanding and mitigating ransomware threats. Future enhancements can further improve the system's scalability, security, and usability.

---

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
