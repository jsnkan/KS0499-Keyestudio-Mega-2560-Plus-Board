# **Keyestudio Mega2560 Plus Board**

![](media/dfda3e220c1d582990808384b3a76b9f.jpeg)


##  **1.Description**

Keyestudio Mega 2560 plus Board, whose processor core is ATMEGA2560-16AU, is fully compatible with Arduino Mega 2560 REV3.

USB to TTL chip adopts more economic and stable CP2012.

This plus board consists of 54-channel digital input and output ports, of which 15 pins are served as PWM output, 16 analog inputs, 4 serial communication ports, one 16MHz crystal oscillator, 1 USB port, 1 power socket, 1 ICSP interface and 1 reset button.

##  **2.Specification**
-   Microcontroller: ATMEGA2560-16AU
-   USB to TTL chip：CP2102
-   Operating Voltage: 5V
-   Input Voltage (recommended):DC 7-12V
-   Digital I/O Pins: 54 (D0-D53)
-   PWM Digital I/O Pins：15(D2-D13 D44-D46)
-   Analog Input Pins: 16(A0-A15)
-   DC Current per I/O Pin: 20 mA
-   DC Current for 3.3V Pin: 50 mA
-   Flash Memory: 256 KB of which 8 KB used by bootloader
-   SRAM: 8 KB
-   EEPROM: 4 KB
-   Clock Speed: 16 MHz
-   LED_BUILTIN:D13

## **3.Interfaces**

![](media/2bb56979eefdee736d5dc304227b5308.png)

![](media/025f20409040406145532b71475f635c.png)

## **4.Special Interfaces Description**

Serial communication interface(4 channel): Serial（D0 =RX0, D1 =TX0）, Serial1（D19 is RX1, D18 is TX1)

Serial2 （D17 is RX2, D16 equals to TX2）, Serial3（D15 is RX3, D14 is TX3), D0 and D1 are connected to ATMEGA16U2-MU

PWM port（Pulse width modulation): D2-D13 and D44-D46

External interrupt pins：D2（interrupt 0), D3(interrupt 1), D21（interrupt 2), D20 (interrupt 3), D19(interrupt 4）and D18（interrupt 5）

SPI communication interface：D53 stands for SS, D51 is MOSI, D50 is MISO, D52 equals to SCK

IIC communication interface：D20 represents SDA, D21 is SCL

## **5.Install Arduino IDE and Driver**

### 5.1 Download Arduino IDE

#### **A. Windows System**

[](https://getting-started-with-arduino.readthedocs.io/en/latest/Arduino%20IDE%20Tutorial.html#a-windows-system)

You could download Arduino IDE from the official website: <https://www.arduino.cc/>

Enter the link and click **SOFTWARE**:

![](media/35689c0bc68d7edba8c627bd3199eef6.png)

There are various versions of IDE for Arduino. Just download a version compatible with your system.

![](media/77e7c042126b8eeea11c791f56b5b4b2.png)

Here we will show you how to download and install the windows version of Arduino IDE.

There are two versions of IDE for WINDOWS system. You can choose between the installer (.exe) and the Zip file. For installer, it can be directly downloaded, without the need of installing it manually while for Zip package, you will need to install the driver manually.

![](media/8cab9c123f890c12acecb2b69da33fa9.png)

You just need to click **JUST DOWNLOAD**.

#### **B. Mac System**

The versions of Arduino IDE vary from operation systems.

For how to download Arduino IDE on Mac, please refer to Windows:

![](media/7d168787a38135d10224dcdf317de4dc.png)

After downloading, double-click to open it and follow the installation instructions.

#### **C.Detailed installation steps：**

1.Save the .exe file downloaded from the software page to your hard drive and simply run the file .

![](media/8f8dc05a74e88f80404c221feb5be436.png)

2.Read the License Agreement and agree it.

![](media/56e65f892f7e0ec8750e4a34fbe30639.png)

3.Choose the installation options.

![](media/c027cb419f67d478118b5714f5ed79a6.png)

4.Choose the install location.

![](media/e7e883fa1ed4d08ed5971c025696abca.png)

5.Click finish and run Arduino IDE

![](media/b956ef7c308fcb0f7dc7e94bbb964f17.png)

### 5.2 Installing Driver

#### **A. Install Driver on Windows System**

Now, let’s install the driver of keyestudio MEGA PLUS control board. Its chip is CP2102 serial chip. Some system（**WIN11**） can’t install automatically driver but you could install it by hand.

**Download driver from:** [**https://fs.keyestudio.com/CP2102-WINDOWS**](https://fs.keyestudio.com/CP2102-WINDOWS)

**Or get dirvers from:**[**https://www.silabs.com/documents/public/software/CP210x_Universal_Windows_Driver.zip**](https://www.silabs.com/documents/public/software/CP210x_Universal_Windows_Driver.zip)

Click the link to download ![](media/1c9b4c541ac50df90a99159db767e4b0.png), and we unzip it to ![](media/2cde1b1f44509733a1b88fefbbb9fb4a.png).

Unzip again and we will get the folder ![](media/f37b95a77c63e40e3162f847bc2cf440.png). Please remember the path of this folder for later use.

Right click Computer—– Properties—– Device Manager.

![](media/ef1c8d62ed502304bcd512349b3211e4.jpeg)

The yellow exclamation mark on the page implies an unsuccessful installation and you should double click ![](media/2417b11a225958b0ba8db020958aef74.jpeg), then click “**Update Drive…**”to update the driver.

![](media/126261aab66afbfb432e50a195e98f55.jpeg)

Click “**Browse my computer for drivers**” to find the downloaded Arduino software.

![](media/fd86e50736422de760b2a4c069fbdbeb.jpeg)

There is a DRIVERS folder in Arduino software installed package, please open this folder and check the driver of CP210X series chips.

Click “Browse…”, then search the driver of CP2102 and click“Next”.

![](media/b18e0a66e88dcf5a6c5964e45dd0db23.png)

After a while, the driver is installed successfully.

![](media/67c754bd8281ab1e1622d9a70688791b.jpeg)

When opening the device manager, we will find that the yellow exclamation mark disappears, which means the driver of CP2102 is installed successfully.

![](media/cc7b58c15299bf0ef8d74d32d9b6e280.jpeg)

#### **B. Install Driver on MAC System**

Connect board we provide to your computer, and open Arduino IDE.

![](media/40a968d312a8b080e52c4559201f498a.png)

Click “Tools” to select **Board: Arduino 2560** and **Port: /dev/cu.usbserial-0001**.




Tap ![](media/98ec72440e6257e5812b408a929a37ba.png) to upload code, if burn successfully, you will view Done uploading.

![](media/e97244571b69d21ff31de3b879b8b0e5.png)

Note: If burn unsuccessfully, you need to install driver of CP2102, please continue to follow the instructions as below:

Download the driver of CP2102:<https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads>

1. Select Mac OSX edition

![](media/6e53a3dacdec57d5ee0b15b48d771a5b.png)

2. Unzip the downloaded package

![](media/8dced2768d5f86d3d0c3f6076d87a9a8.png)

3. Open folder and double-click SiLabsUSBDriverDisk.dmg file.

![](media/61ae3e706a1c4afa7948d5fb2e797a6d.png)

4. You will view the following files as follows:

![](media/3ffd0525e16492ede92bdb8c84198db9.png)

5. Double-click Install CP210x VCP Driver, tick Don’t warn me and tap Open.

![](media/14f6ebb088e654abc2f0149645e34ed1.png)

6. Tap Continue

![](media/a243872cdbb520e4d298c006e001fff5.png)

7. Tap Continue and Agree

![](media/ae367c1894df6745e46bbdfc460c1f99.png)

8. Click Continue and input your password

![](media/27b7214283d7f76aba3557dd629bd965.png)

![](media/29bbca3360d806164717733460574356.png)

9. Select Open Security Preferences

![](media/ca6bc6e536202f07a53c09201a0996ff.png)

10. Click the lock to unlock security & privacy preference.

![](media/379caa1889f4a45614b27c9b2b934869.png)

![](media/88a1b169a192ee6c49e95947d6287fc2.png)

11. Then click Allow

![](media/19e43624efde1b223800201c944d25e9.png)

12. Back to installation page, and wait to install.

![](media/bb0e17afd8bad8b8013f19d7a9da0fd9.png)

13. Successfully installed

![](media/3bd5bb3752abf97e9bab6bf950a75bed.png)

14. Then enter ArduinoIDE, click Tools and select Board: Arduino Uno and /dev/cu.SLAB_USBtoUAPT

![](media/73aed810d216d7da3a3ce9cc0e4dba4a.png)

15. Click![](media/9c9158a5d49baa740ea2f0048f655017.png) to upload code and you will see “Done uploading”.

![](media/d918e2e31a9632f8b272a16595c46a83.png)

### 5.3 Arduino IDE Setting

Click![](media/675ae7298ce0973df720b2fbbb514caa.png)icon and open Arduino IDE.

![](media/4f4f33bb23c495e81b1cfad163653b59.png)

To avoid the errors when uploading the program to the board, you need to select the correct Arduino board that matches the board connected to your computer.

Then come back to the Arduino software, you should click Tools→Board, select the board. (as shown below)

![](media/d27e784f35475d633be807e115c7358f.png)

Then select the correct COM port (you can see the corresponding COM port after the driver is successfully installed)

![](media/a653ae3296bbac0dcf12901534fcdd45.png)

![](media/9995706530f3327b61cd4455d9945299.png)

### 5.4 Start Your First Program

Open file to choose Examples—>BASIC—>BLINK

![](media/54cde01d6569a2b0d61d160775779ed8.png)

![](media/39e05c310f6766d92bb4c3c2b279feaf.png)

Set board and COM port, the bottom right corner of the IDE displays the corresponding board and COM port.

![](media/5fa8949b0b013180bde1f64f324568af.png)

Click![](media/ddd21c81338ae1f6b7f84de2a3caecf0.png)icon to start compiling the program, and check errors.

![](media/e06bf758d9a42d81b346d79e45ca2b29.png)

Click![](media/9c9158a5d49baa740ea2f0048f655017.png)icon to start upload the program, upload successfully.

![](media/c2355513a37fe793976e97d827fe8d8e.png)

The program is uploaded successfully, LED of board lights on for 1s, and lights off for 1s.
