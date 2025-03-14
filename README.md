# Index
- [1. Open source contributions](#Open-source-contributions)
- [2. Personal works](#Personal-works)
- [3. Company works](#Company-works)
  - [3.1. Embedded BSP intern at Coasia, nexell](#embedded-bsp-intern---at-Coasia-nexell)
  - [3.2. Embedded BSP engineer at Coasia, nexell](#Embedded-BSP-engineer---at-Coasia-nexell)
    - [3.2.1. Contributions](#Contributions)

# Open source contributions

# Personal works
## [Automatic parking lot guide using AI object tracking](https://github.com/vacu9708/Smart-CCTV) `2022/05 - 2022/12`
<img src="https://github.com/user-attachments/assets/5f891cd7-bb45-49bc-b7d3-094bab260ea1" width="60%"><br>
-	Developed a system that tracks cars and displays parking information on LEDs to reduce wasted time when searching for parking spaces.

## [Guitar tuner](https://github.com/vacu9708/Guitar-tuner) `2020/05 - 2020/06, 2022/02 - 2022/03`
![image](https://github.com/vacu9708/WHO-AM-I/assets/67142421/343937f2-4515-4fd1-91eb-ee834690f735)
![image](https://github.com/user-attachments/assets/4c0dc765-d0ee-4ecb-830a-73c4da03ac69)
<img src="https://github.com/vacu9708/WHO-AM-I/assets/67142421/5a4266c7-eaea-4b97-96ae-4e87b6524b30" width="60%"><br>
- Developed sound frequency analyzer
- Studied [Fast Fourier Transform](https://github.com/vacu9708/Signal-processing/tree/main/Fourier%20transform)

## [Studying how computer memory works](https://github.com/vacu9708/Game-hacking) `2024/11 - 2024/12`
<img src="https://github.com/user-attachments/assets/d4a40ab2-8d29-4d0e-8c65-48245d5bd141" width="70%"><br>
![image](https://github.com/user-attachments/assets/fa9eff64-66f5-4359-9bd5-530b5c28de2d)

- Studied how memory works by researching how to bypass video games' security mechanisms, track enemy positions, and draw rectangles around them.

## [Inter Process Communication](https://github.com/vacu9708/Study-records/tree/main/Computer%20science/Operating%20system/Inter-Process-Communication)
![image](https://github.com/user-attachments/assets/125b91aa-bf73-4217-ae6d-6cb12f7e492d)

## [Webpage update notifier](https://github.com/vacu9708/Information_notifier) `2022/06~2022/07`
<img src="https://github.com/vacu9708/WHO-AM-I/assets/67142421/4efa38a6-52f3-44a1-b0a0-bc1e4a9b369a" width="60%"><br>
- Developed a program sends notifications each time new information is uploaded to specified webpages.

## [Video conference](https://github.com/vacu9708/video-conference) `2022/09 - 2022/10`
<img src="https://github.com/vacu9708/WHO-AM-I/assets/67142421/17c4c315-af24-4067-8def-6413399343e0" width="60%"><br>
- Developed a web page using JavaScript and WebRTC where three or more participants can have group chat and video calls

# Company works
## Embedded BSP intern - at Coasia, nexell
(December 2023 – March 2024)
- Studied core concepts in embedded SW including data structures, computer architecture, operating systems, Yocto, and Docker.
- Studied bootloader development and U\_BOOT\_CMD implementation.
- Explored Linux kernel and device driver development.

## Embedded BSP engineer - at Coasia, nexell
(March 2024 – Present)

### Contributions
Focused on the camera of the BSP
- **AI Object Detection Support:**
    - Created a shell script to switch camera device drivers without requiring rebuilds or reboots.
    - Used OpenCV to align streaming windows in Wayland when using Gstreamer.
- **Technical Support for Camera Software:**
    
    - Reviewed hardware datasheets to verify support (e.g., confirming the absence of RGB-to-RGBA conversion support) and communicated findings to customers.
    - Explained methods for running simultaneous camera streams with Gstreamer.
    - Applied and verified a patch to resolve a vsync bug by checking the board schematics and confirming a 60Hz frequency with an oscilloscope.
- **BSP Validation and Debugging:**
    
    - Set up test environments and validated camera performance across various models using automated shell scripts.
    - Verified Android External View System functionality.
    - Resolved remote I/O errors in the camera device driver by addressing separated I2C settings and adjusting rx/tx rate configurations.
    - Fixed JSON parsing issues in the camera middleware and added missing color format support for RGGB20.
- **Porting Pi Camera to ExynosAuto:**
    
    - Enabled MIPI pins (pwr\_enable, 2-lane MIPI) and validated functionality with an oscilloscope.
    - Read CSI registers to confirm PHY\_STATUS and modified the Raspberry Pi camera device driver (with added debug prints) to align settings with the ExynosAuto board.
    - Noted limitations in real-time ISP tuning, resulting in lower image quality compared to GMSL cameras.
- **ISP Tuning Support for Naver Labs Cameras:**
    
    - Investigated I2C errors on a specific CSI channel by testing multiple boards to isolate hardware issues.
    - Modified the camera device driver to support single-camera operation per CSI channel and developed a Python script to auto-generate driver code.
    - Integrated I2C communication logging within the driver for debugging purposes and verified functionality following ISP algorithm updates.
- **Android Camera Sample App Development:**
    
    - Developed an Android sample application (using Android Studio) featuring preview, capture, image thumbnail, and parameter configuration.
    - Resolved issues with fixed resolution in the camera HAL to enable high-resolution camera usage.
- **Code Analysis and Presentations:**
    
    - Analyzed camera middleware, color space conversion middleware, and Android External View System code using block and sequence diagrams.
    - Utilized VSCode call hierarchy, reference searches, and GDB to understand code flow.
- **Unit Testing for Camera Device Driver:**
    
    - Developed unit tests with KUnit and gcov for the camera device driver.
    - Wrote a Python script to automate the creation of KUnit templates, enhancing test code development efficiency.
- **Additional:**
    
    - Developed a Python script to log the latest commit from all BSP repositories for easier troubleshooting after updates.
    - Completed trace32 training.
