# INFORMATION ASSURANCE - FINAL PROJECT
**BSCS 3B**
- Sayson, Nestor Jr. B.
- Tagum, Mark B.
- Salvino, Vincent James O.
- Vela, Angelica P.

##  Step-By-Step Documentation

### 1. Prepare and Install Headless Raspbian OS in Raspberry Pi

#### Step 1: Reformat the SD Card
Insert the SD card into your computer and reformat it using a tool like SD Card Formatter.
<img width="658" alt="Screenshot 2023-12-18 103301" src="https://github.com/vincentjamessalvino/Readme.md/assets/145561497/65131ff4-9729-410d-8a92-82aa86f5deb6">

#### Step 2: Download Raspbian OS
Visit the official Raspberry Pi website and download the latest Raspbian OS image.
<img width="952" alt="Screenshot 2023-12-18 104113" src="https://github.com/vincentjamessalvino/Readme.md/assets/145561497/57abb92f-8e32-4799-950b-287d7399c18a">

#### Step 3:  Install Raspbian OS on SD Card
![Screenshot (456)](https://github.com/vincentjamessalvino/Readme.md/assets/145561497/482dba8a-cb59-42ff-b63d-44ef098d2763)

#### Step 4: Configure
Change the Username and Password and Connect to Wi-Fi and Make sure to enable the ssh
![Screenshot (454)](https://github.com/vincentjamessalvino/Readme.md/assets/145561497/235c1191-aa42-438a-bfce-132f48b9935c)
![Screenshot (499)](https://github.com/vincentjamessalvino/Readme.md/assets/145561497/622b2007-4e27-4999-80ba-3f94ca535870)

#### Step 5: Insert SD Card
Insert the SD card into the Raspberry Pi and power it up.

### 2. Connecting to Raspberry Pi via SSH using the terminal

#### Step 1: Find Raspberry Pi IP
Connect the Raspberry Pi in monitor to check your Raspberry Pi IP in and type in command prompt ifconfig and get the inet. 
![IMG_20231213_161444_914](https://github.com/vincentjamessalvino/Readme.md/assets/145561497/4e89cba9-c124-4db0-a471-0ffbaf916bb2)

#### Step 2: Open Terminal
Open the terminal on your computer.

#### Step 3: SSH Connection
Use the following command to connect to the Raspberry Pi:
```bash
ssh username@<RaspberryPiIP>
```
Enter your password when prompted.

![Screenshot 2023-12-13 161926](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/bf074085-c2ed-46e9-864d-b1332900ae38)

### 3. Deploying LAMP Stack in Raspberry Pi

#### Step 1: Update and Upgrade
Run the following commands to update and upgrade the Raspberry Pi:
```bash
sudo apt update
```
![Screenshot 2023-12-13 162017](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/4fdfd7cb-f854-4e78-8039-47794a4a82fc)

```bash
sudo apt upgrade
```
![Screenshot 2023-12-13 162043](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/a6152e80-1227-4092-90e6-4835c3a806de)

#### Step 2: Install LAMP Components
Install Apache, MySQL, and PHP using:
```bash
sudo apt install apache2 
```
![Screenshot 2023-12-13 162130](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/4ef0a954-37e5-44cf-a5b1-4f7a0ae7f6d7)

```bash
sudo apt install mariadb-server
```
![Screenshot 2023-12-13 162303](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/e7bb1a80-7430-44d6-8cd6-931c0949236e)

#### Step 3: Secure MySQL
Run the MySQL secure installation script to enhance security.
```bash
sudo mysql_secure_installation
```
![Screenshot 2023-12-13 162655](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/f37acd49-7d91-4388-a79f-39c589f984b2)

```bash
sudo apt install php libapache2-mod-php php-mysql
```
![Screenshot 2023-12-13 162744](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/51d93824-eccb-4433-9fe0-554f6f0e803d)

```bash
sudo apt-get install php*
```
![Screenshot 2023-12-13 163102](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/63c57d94-1f93-44d6-a569-4ce07125ccb7)

```bash
sudo apt install phpmyadmin
```
![Screenshot 2023-12-13 163211](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/65c6dd53-670b-40fb-ac8e-3119c7151abf)


### 4. Enabling and Controlling Raspberry Pi using VNC

#### Step 1: Enable VNC
Run the following command to enable VNC:
```bash
sudo raspi-config
```
Navigate to 'Interface Options' > 'VNC' and enable it.

![Screenshot 2023-12-13 164104](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/e042d965-53a2-4841-9f67-f561535560ff)

#### Step 2: Download and Install VNC Viewer
On your computer, visit the official RealVNC website: [RealVNC Download](https://www.realvnc.com/en/connect/download/viewer/)
![Screenshot (497)](https://github.com/vincentjamessalvino/Readme.md/assets/145561497/88ae0ae3-cd12-4858-a814-92340d6172be)

#### Step 3: Connect via VNC Viewer
Connect to the Raspberry Pi using its IP address.

![Screenshot 2023-12-13 163936](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/245c0c3c-3d79-4fd4-86c1-485624e02c7c)

#### Step 4: Control Raspberry Pi
You can now control the Raspberry Pi desktop using VNC Viewer.

![Screenshot 2023-12-13 164040](https://github.com/vincentjamessalvino/Readme.md/assets/145563728/fd575876-424e-4295-b9d6-9b5a13c069d5)
