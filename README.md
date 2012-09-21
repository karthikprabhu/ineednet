#INeedNet

INeedNet is a shell script that lets you disconnect other computers connected to your WiFi network. This is particularly useful if you are connected to a public WiFi and other annoying users are using heavy bandwidth. 

This script is based on the famous Aircrack-ng suite and automates the entire process from scanning clients on your network to sending DeAuth packets.

##Documentation

###Requirements

INeedNet requires the following in order to work :

* [Aircrack-ng suite](http://www.aircrack-ng.org/index.html)
* [Wireless Tools for Linux](http://www.hpl.hp.com/personal/Jean_Tourrilhes/Linux/Tools.html)(This is included by default in most Linux distros)
* Wireless NIC capable of packet injection

Make sure you install the above tools before running the script.

###Usage

Using INeedNet is pretty simple. All you need to do is call the script

```bash
./ineednet
```
and wait until it finishes. It takes approximately 45-60s to complete

If your default card does not support packet injection and you are using an additional card to do so, you can run the script with the following arguments :

```bash
./ineednet -i <interface name>
```
Please keep in mind that the script uses the additional card only for packet injection. You need to be connected to the network on your default card for this script to work.

