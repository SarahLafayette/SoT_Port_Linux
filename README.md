# SoT_Port_Linux
Sea of Thieves port checker for Linux


![Screenshot from 2023-08-26 16-25-02](https://github.com/SarahLafayette/SoT_Port_Linux/assets/129413356/8a49d3cb-13e1-4491-8ed1-1a15168880d4)



This is a simple tool that constantly uses tcpdump to grab UDP traffic and find traffic in the 30000-31000 range and display the current recieving port number. 

Why? 

This is a simple Linux tool to allow Linux users to monitor their port number for spiking purposes most typically in the creation of an Alliance server. 

Use:

user:~$./port.sh

-or-

user:~$./path/to/file/port.sh

THIS RUNS CONSTANTLY
If you are trying for a certain port, just leave this tool running and it will update itself, no need to relaunch for every spike. 

Bug: 

Don't run as sudo, allow the tool to prompt you for your password. I'm not sure why, but this is how it works.
In some rare cases traffic will go back and forth between two ports and the displayed number will flash between them. In this case your 'port' is the lower number. 
This is very rare and if more than three people ever use this I'll look into it. 

This is my first bash script and public commit for the most niche of users, be gentle. 

~Sarah
