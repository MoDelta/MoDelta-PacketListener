# MyPacketListener

Use of : python3 packet_listener.py

Using this application, we can listen to the target's network after performing a man-in-the-middle attack.

To listen to https sites, you need to do the following commands:

We download dns2proxy. You can find it on Github.

We run the following commands separately in the terminal :

iptables -t nat -A PREROUTİNG -p tcp --destination-port 80 -j DEDİRECT --to-port 10000

iptables -t nat -A PREROUTİNG -p udp --destination-port 53 -j DEDİRECT --to-port 53

We run the sslstrip command in the terminal

We run the python dns2proxy.py command in the terminal

All of these will be written in a different terminal.

sslstrip comes installed on Linux. 

We just need to download dns2proxy extra.

*This software was written by learning from the lessons of instructor Atıl Samancıoğlu.
