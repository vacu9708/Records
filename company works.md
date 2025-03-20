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
