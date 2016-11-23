PPP Files
Copyright (c) NimbeLink 2016

Description
===========
This repo contains PPP files needed for the various Skywire modems.

Usage
=====
Copy the script file and its associated chat file into "/etc/ppp/peers/" (or copy all
of the files to "/etc/ppp/peers/").

If you have a Skywire modem that uses a SIM card, follow instructions in your "-chat" file
to set the APN.

Run your respective command:

sudo pppd call [name of script file]
sudo pon [name of script file]

Example
=======
To use the NL-SW-LTE-TSVG Skywire that was activated at go.nimbelink.com, copy the following files:

vzw-TSVG
vzw-TSVG-chat

to "/etc/ppp/peers/". 

Edit the file:

vzw-TSVG-chat

to insert the APN. In this example, replace:

[apn]

with:

NIMBLINK.GW12.VZWENTP

Finally, issue the following command:

sudo pon vzw-TSVG