PPP Files
===
Copyright &copy; NimbeLink 2018

Description
===
This repo contains example PPP files for various Skywire modems on Linux. These files provide direction on setting up a PPP connection, but they may need to be adapted to the specific embedded design developed by the customer. Each end customer embedded design is different.

We recommend reviewing the PPPD manual page for more information and options:

	man pppd

Usage
===
Copy the script file and its associated chat file (or all of the files) into: 

    /etc/ppp/peers/
     
If you have a Skywire modem that uses a SIM card, follow instructions in your 

    *-chat

file to set the APN.

Run your respective command:

    sudo pppd call [script file]

or

    sudo pon [script file]

Example
===
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
