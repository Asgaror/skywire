
![skywire logo](https://user-images.githubusercontent.com/26845312/32426764-3495e3d8-c282-11e7-8fe8-8e60e90cb906.png)

### Official guide how to use the Skywire SSH functionality

*This guide assumes that you have read and understood the readme.md, downloaded the official images or installed Skywire from source and do every step exactly the way it is described. Misconduct will lead to inability to connect and to potential reflashing. It is very important that there is no IP collision with your existing home router subnet. The default settings of the official images as well as the router of the skyminer are using the 192.168.0.0/24 subnet.*

#### Table of Contents
* [Introduction](#introduction)
* [Requirements](#requirements)
* [Usage](#usage)

## Introduction

After finishing this guide you will be able to remotely connect to your running Skywire nodes per SSH.
Your nodes need to be up and running and have a working network connection to the [discovery](discovery.skycoin.net:8001). Check if your public keys are listed on their before you start and use the other [guides ](https://github.com/skycoin/skywire/wiki) and our telegram chats to troubleshoot if they are not on there.

The instructions about setting up the necessary port forwarding rule for this to work were made on the official miner router, you might have different settings on your model and need to act accordingly.

## Requirements in Hardware & Software

* Computer/laptop with LAN port
* LAN cable
* Running Skywire manager & node(s)
* Network connection, connection to the discovery 
* Running SSH client on the nodes + in the managers web interface
* Installed Skywire node on the device used for remote connection or access via port forwarding to a node

***

## Usage

As previously stated you need to have Skywire running and have access to the manager in your browser. If that is not the case please install Skywire first, you can use guides from our [forum](https://skywug.net/forum/Forum-Skywire) or use the [official images](https://github.com/skycoin/skywire/wiki/Skyminer-Skywire-installation-guide).

### Preparation
The pi that is used for establishing the connection in the following guide has the local IP 192.168.0.3.

#### Start SSH service and save keys

First we need to start the SSH service on your node that you later want to connect to. 
Click on `SSH`:

![ssh](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/SSH%20guide/SSH.png)

This will start the SSH server that will enable incoming connections to be established. 
Should look like this: 

You need to note down the public key of the node, as well as the SSH key (sshs). Both are marked with a red rectangle.

![SSH_Client](https://raw.githubusercontent.com/Asgaror/skywire/aa3c07d38072233db8c40dd0674b7e48f7764a55/pictures/SSH%20guide/SSH_success.png)

```
node key = public key; 
in this example public key = 02c9239fc5e8abe11363a8c6b9d6f8f738b6bd25412d08305ef2b1c478f2f423cf

app key = sshs key; 
in this example sshs key = 03e41c6edeacf87a5637365695310cd6d16d0db63ca15c2d505c12a5d31e5ba01b
```
You really need to do this process only once, since you can access the whole subnet after establishing a connection to one pi, but to be safe you should do it on at least one other node in case the pi crashes. 

*Best practice would be to note down the keys (public key + sshs key) of all 8 nodes and enable the SSH service on all pi's. This way you'd still be able to gain access even if 7 of the eight pi would crash.*

#### Connect via Skywire SSH to another node

To do this from remote you need to have a Skywire node running on the device your using, or you need to have access to one via port forwarding. Check the linked resources if you need guidance how to do this.
Open the manager web interface and click on `SSH Client`. 

![SSH_Client](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/SSH%20guide/SSH_Client.png)

The node key is the previously noted public key and the app key is the sshs key.
Enter them in the popup window and click on `Connect`.

![SSH_Client_popup](https://raw.githubusercontent.com/Asgaror/skywire/aa3c07d38072233db8c40dd0674b7e48f7764a55/pictures/SSH%20guide/SSH_Client_popup.png)

A successful connection should look like this:

![SS_working](https://raw.githubusercontent.com/Asgaror/skywire/aa3c07d38072233db8c40dd0674b7e48f7764a55/pictures/SSH%20guide/SSH_working.png)

Please note down the port that is being displayed on which the connection was established. In this example the port is `30000`.

***

### Use the established connection

By now you have successfully established a SSH connection to another Skywire node. Now you just need to put it to use.

First note down the local IP of the pi you're using right now by executing `hostname -I`. In this example the local IP is `192.168.0.5`.
To do this, open a terminal in the manager, or connect to the node which you used for establishing the connection via SSH (Use putty if you're on windows and the terminal on mac/linux).

Then execute `ssh localhost -p 30000`, note that you might have to replace 30000 in case you have multiple connections established.

Option 1, login via terminal on linux:

![Login_terminal](https://github.com/Asgaror/skywire/blob/aa3c07d38072233db8c40dd0674b7e48f7764a55/pictures/SSH%20guide/Login_terminal.png)

Option 2, use the terminal inside the manager web interface:

![Login_web_interface](https://raw.githubusercontent.com/Asgaror/skywire/aa3c07d38072233db8c40dd0674b7e48f7764a55/pictures/SSH%20guide/Login_web_interface.png)

Now you are logged into the remote pi via SSH session. You have gained access to modify the file system, reboot the pi and of course, SSH access to the whole subnet. 
First obtain the local IP address of the pi you're connected to by executing `hostname -I`.

![hostname](https://raw.githubusercontent.com/Asgaror/skywire/aa3c07d38072233db8c40dd0674b7e48f7764a55/pictures/SSH%20guide/SSH_hostname.png)

*Please note that typing might suffer from a performance lag and the characters will be displayed after a short delay. As you can see the SSH connection worked, the local IP changed from 192.168.0.5 (local pi) to 192.168.0.3 (remote pi)*

That's it, you are now logged into your pi from a remote location using the Skywire SSH function.

#### Testing

Test the connection by requesting your ipv4 address via `curl v4.ifconfig.co`, the output should be different that your actual IP address at your current location.

Furthermore you could try to login to the other pi's via SSH, by executing `ssh root@192.168.0.2`

![Login_manager](https://raw.githubusercontent.com/Asgaror/skywire/aa3c07d38072233db8c40dd0674b7e48f7764a55/pictures/SSH%20guide/Login_manager.png)
