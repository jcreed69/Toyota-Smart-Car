# Toyota-Smart-Car
Makes Old Toyota Cars Smart and Feel New

# what is this project?
This is a project where you use an ESP32 a round display and rotary encoder and it displays info about the car Example: Time, speed, Weather and more. This project is not too expensive and can be homemade
# pictures
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/cff12292-9e95-4124-9be0-d99b00d7debf" />
<img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/d43adb2b-543a-44f5-bacb-a3ebb5ba27f9" />
<img width="400" height="700" alt="IMG_3956" src="https://github.com/user-attachments/assets/93207b93-c88b-4f55-acfd-386caeb8dae2" />
<img width="400" height="700" alt="IMG_3955" src="https://github.com/user-attachments/assets/cb479b98-b6b6-45bf-ac6e-0fa839da657c" />
<img width="300" height="300" alt="IMG_3954" src="https://github.com/user-attachments/assets/ba52de01-c4e2-41d6-9a48-722a7f894e2e" />
<img width="300" height="300" alt="IMG_3953" src="https://github.com/user-attachments/assets/a755ec12-1a0c-4529-af0f-78e274091f7f" />
<img width="300" height="300" alt="IMG_3952" src="https://github.com/user-attachments/assets/29206282-913e-4482-808b-7082d3c2bdb6" />
<img width="300" height="300" alt="IMG_3951" src="https://github.com/user-attachments/assets/6d6971e2-3f4a-4892-b697-746bf79d3515" />
<img width="300" height="300" alt="IMG_3950" src="https://github.com/user-attachments/assets/c59f856f-9ce5-4c83-8f6d-7129f3082489" />
<img width="300" height="300" alt="IMG_3949" src="https://github.com/user-attachments/assets/f4cc9030-3dac-4759-ad1f-b0e6a4142391" />



# What you need:
1. __FreeNove ESP32 Wroom__ ---- https://www.amazon.co.uk/Freenove-Dual-core-Microcontroller-Wireless-Projects-2-Pack/dp/B0C9TGJRPH/ref=sr_1_2_sspa?crid=29W0QUWX9LBRD&dib=eyJ2IjoiMSJ9.beVRzgfFpa7S78WssaJYRQiS_c-vR-ZReQGUvDayev4s7gjNmL5oTh9_x25u_38YoKWxnaIrqT4ZcbmkeUb_R1IV0iwtU8mVcdv_jC5qHhjC03-cJr0dm_wbTZ9mKoLlcznQNbza2Rhq2MVQI0UPxG1mnY0jZKB1K-reI7F_ZPjY1Bt_zX-XeDOW4gNgBOM8Rs6E2om6ANyr4jqt9DGiWsSB9L9U0lz_F1f0dkIcacQ.4d-2ImyNRxpJd79tiDCN4grWqcSQNPfMk7iPdsL3u_I&dib_tag=se&keywords=freenove%2BESP32%2Bwroom&qid=1790503621&sprefix=freenove%2Besp32%2Bwroom%2Caps%2C121&sr=8-2-spons&aref=MU1dvsmDmW&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1

2. __Rotary Encoder__- https://www.amazon.co.uk/dp/B0BN1MN2KM/ref=sspa_dk_crr_aax_0?psc=1&aref=up00kWO9Bo&sp_csd=d2lkZ2V0TmFtZT1zcF9jcnJfc2hhcmVk

3. __TFT Display GC9A01__ - https://www.amazon.co.uk/Display-Arduino-Colour-Screen-GC9A01/dp/B0H33VDLX3/ref=sr_1_2?crid=1TYCRGI883USR&dib=eyJ2IjoiMSJ9.hIU0xm82MIG9QQkX7T-vUyNgkjLUjtzA6DDoCpzh4e0ZwBciXKTd-RduLcqa4bx6VRAa91uHlda_vj5a9Vq6q3QDsBgNB631UhCkECoLR2998oV-GGCyTlbNpyDqYVwPtfkY8yXnRVIoGOli88-aFm9zUjvEh0K2yUCYyyzYz3-n7iqWXZWA7ZUlV14w1Be9IeeW216-TPA8y0xqw8CU849vRIP7bGqZ9TvZrPCic3tko6G4-lTh3wuvIZw5WfL5GcufrE7KScSYmuNbLJG6rY7l2S10Yiul6acr9F3DD7Q.pS2_dPpc0MP9Bms8pTmfmC25hBTQtAtLA9B8T1E7lQA&dib_tag=se&keywords=TFT+display+GC9A01+round&qid=1790503866&s=industrial&sprefix=tft+display+gc9a01+round%2Cindustrial%2C107&sr=1-2

4. Female to Female Jumper cables

5. Working Laptop running latest arduino IDE



# Connections
Firstly connect the pins to the ESP32

__TFT display GC9A01__

| Pins | Connect | Description/Notes |
| :--- | :---: | :--- |
| VCC | Any 3.3V | Power - DO NOT CONNECT TO 5V |
| GND | Any GND | cycles the power |
| SCL | Pin 18 | No Notes |
| SDA | Pin 23 | No Notes |
| DC | Pin 26 | No Notes |
| CS | Pin 27 | No Notes |
| RST | Pin 25 | Doesn't reset anything |

__Rotary Encoder__

| Pins | Connect | Description/Notes |
| :--- | :---: | :--- |
| VCC | Any 3.3V | Power - DO NOT CONNECT TO 5V |
| GND | Any GND | Cycles the Power |
| SW | Pin 21 | Switch - To rotate the menu |
| DT | Pin 33 | No Notes |
| CLK | Pin 32 | Enables the button to be clicked |

NOTE: Recommended to use tape so connections will not be loose

# Flashing and Set-Up

Now all the pins are connected and secured we are now flashing the firmware and configuring the Device

1. install Arduino IDE for your Operating System : https://support.arduino.cc/hc/en-us/articles/360019833020-Download-and-install-Arduino-IDE
   (If Arduino IDE is taking longer than 5 mins to open scroll till you see Fixes and FAQ)

2. Once installed and the UI opens Head to File > Preferences scroll down till you see Additional boards manager URL's, paste this link: https://espressif.github.io/arduino-esp32/package_esp32_index.json and close Preferences. Use the image to help you. <img width="990" height="490" alt="image" src="https://github.com/user-attachments/assets/f17eeb0a-fd25-4e36-bf71-93362184f6dd" />

3. Now head to Tools > Board > Board manager and type in the search box esp. scroll down to see esp 32 by Espressif Systems Press install. Use the image to help you  <img width="245" height="237" alt="image" src="https://github.com/user-attachments/assets/206ec1b2-ce0f-4548-82be-66b8c8829455" />

4. Close the tab and then head to Tools > Manage Librarys and a tab will open.

5. Install These Librarys
   
| Library | description |
| :--- | :--- |
| Adafruit GC9A01A | Connects the Display | 
| Adafruit GFX Library | Draws Texts shapes and Graphics| 
| Adafruit BusIO | Dependency used by the display libraries | 

These should already be installed when you install the Library Adafruit GC9A01A but please double check without these the device will not run and give errors


__OPTION 1__: Use Arduino to Manually flash the Firmware (requires .Zip) - used to be flashed first time OR versions V0.2.0 or under

1. Download the latest .zip  from releases
2. Extract the .zip and open Smart toyota.ino
3. Press Select device or USB and a window opens and search esp32 dev Module<img width="557" height="43" alt="image" src="https://github.com/user-attachments/assets/2dc35a96-8aad-488f-b65e-cd364fa861b7" />
<img width="866" height="495" alt="image" src="https://github.com/user-attachments/assets/a3090cb6-6fcb-4048-8337-c90ace4ae178" />

4. in Arduino IDE to Flash by pressing upload or the arrow going left
5. You now have flashed the firmware!

You will be able to Flash Firmwares VIA Bluetooth by app and OTA.. but requires to flash the firmware VIA Arduino first.

__OPTION 2__: OTA Updates VIA App/Versions requires V0.2.0+ (You need to use option 1 to use OTA updates)

1. Head to How to control your device Tab to get the app and device set-up
2. Connect the display to the app
3. head to the top right or settings
4. scroll down to see the Title 'Wireless Update'
5. press Enter update mode this will reset the device
6. reconnect to the display
7. head back to settings and press Install latest. This will take a long time

# Features

- Flash Firmware without Arduino IDE (OTA Updates VIA Bluetooth (requires V0.2.0+))
- Demo mode
- pinn your favorite faces via app
- Cycles differnt faces: Speed, Time, Journey route, Journey time in car, Navigation, compass heading, weather
- Change settings via website
- Makes your car feel new

# How to control your device
You can control your device by app. Android and iOS behave differntly. Find the steps for YOUR OS

iOS
1. Download Bluefy(it is free and no ads)
2. paste this link: https://smart-toyota-companion.x4fk2h4gq4.chatgpt.site (Used chatGPT to puplish the website)
3. The website will show up you can save it by pressing the star in the search bar on the right
4. connect the display and allow permissions

Android:
1. copy this link: https://smart-toyota-companion.x4fk2h4gq4.chatgpt.site
2. connect to the display and allow permissions

# Other Versions
If you require other versions

| Version | Link | Main Change |
| :--- | :--- | :--- |
| V0.1.5 |https://github.com/jcreed69/Toyota-Smart-Car/releases/download/Smart-Toyota/SmartToyota.zip| First Release |
| V0.2.0 |https://github.com/jcreed69/Toyota-Smart-Car/releases/download/V0.2.0/SmartToyota.zip| OTA Updates |
| V0.2.4 |https://github.com/jcreed69/Toyota-Smart-Car/releases/download/V0.2.4/SmartToyota.zip| Faces changes|

# Fixes and FAQ:

How to fix Arduino IDE taking so long to load the UI

1. press win + R head to %userprofile% and delete the arduino folder
2. press win + R head to %appdata% and delete the folder (lowercase) arduino not the captilaised

Does this have to be for the Toyota?
No. There is no line of code which recognises that you are in a toyota or driving a toyota. this can go on a bike(3D print mounts) and any other car. This is only an upgrade to the car

Does it need Wifi?
Yes . Wi-fi is required to connect to the display as it needs to send data and connect to the website and use map services and location.

# upcoming features
V0.2.6
 - Upside mode - gives a better oppotunity to place this device in the car
 - Faster OTA updates - currently takes an hour
 - Ability to use 2 round display an one OLED display
 - Ability to rename the device for easy connection
 - Ability to auto connect
 - ability to chnage the UI
   





    


   
