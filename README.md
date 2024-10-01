# Wireless Video and Audio Broadcasting System on Ultra96-V2 FPGA

This project focuses on designing and implementing hardware for the **wireless transmission of video and audio data** using the **Ultra96-V2 FPGA board**. The core objective is to create a system capable of **capturing, compressing, and transmitting** multimedia data, with future scalability towards integrating the design as an **ASIC (Application-Specific Integrated Circuit)** for use in wearable devices and other real-world applications.

## Project Structure

### 1. Data Capture and Compression
The system will use **commercial off-the-shelf sensors** to capture **video and audio data**, such as:
- MIPI camera modules (for video)
- Microphones (for audio)

The **FPGA fabric** will be responsible for **compressing the video and audio data** in real-time, ensuring efficient transmission. A **speaker** will serve as the **audio output device**, which will receive and play back sound that is processed and returned from the server-based AI system.

### 2. Wireless Communication
- Initially, the **on-chip Arm Cortex-A53 processor** will handle the necessary **communication protocols** (such as **Wi-Fi** and **cellular communication**) for data transmission over the internet.
- As development progresses, the communication protocols will be **migrated to the FPGA fabric**, allowing the FPGA to fully manage wireless data transfer. Additional sensors, such as **Wi-Fi** and **cellular modules**, will be utilized to facilitate communication.

### 3. System Output and AI Communication
The system will interact with a **cloud-based AI** to process the video and audio data:
- **Captured video and audio data** will be transmitted wirelessly to a server for processing by a **customized AI**.
- The AI will return relevant data, which will be sent back to the system.
- The **speaker** will play the AI’s audio output, enabling **real-time feedback and interaction**.

### 4. Future Vision: AI-Driven Smart Wearables
While the current focus is on developing a hardware solution using the **Ultra96-V2 FPGA**, the long-term goal is to transition the design into a **custom IC (Integrated Circuit)**. This will enable lower-cost production and integration into **smart wearable devices** and **smart home utilities**.

The complete hardware design—encompassing video/audio capture, compression, and wireless communication—will ultimately reside within the **FPGA fabric**, with only essential sensors (e.g., Wi-Fi and cellular modules) externally connected. This will make the system suitable for mass production as an **ASIC** for various applications.

## Goals:
- **Wireless video/audio capture and broadcasting** through the Ultra96-V2 FPGA.
- **Real-time data compression** using the FPGA fabric.
- **AI-driven audio feedback** through a server, with output via a speaker.
- Future migration to a **fully FPGA-based design** for production as an **ASIC**.

## Technologies Used:
- **Ultra96-V2 FPGA board**
- **MIPI camera module** for video capture
- **Microphone** for audio capture
- **Speaker** for audio output
- **Wi-Fi and cellular modules** for wireless data transmission
- **FPGA-based compression algorithms**
- **Arm Cortex-A53 processor** for initial communication protocols
- **Cloud-based AI** for video/audio data processing

---

## Future Development:
This project will continue with the implementation of communication protocols in the FPGA fabric and further optimization of data compression and transmission. The ultimate objective is to create a scalable hardware platform that can be integrated into **smart wearable devices** and mass-produced as an **ASIC**.

