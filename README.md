# X11 Remote Desktop
This is a rudimentary remote desktop tool for the X11 protocol exploiting unauthenticated x11 sessions.

Our approach is to automate the process of using the default X toolset into an easy to use tool for exploiting unauthenticated X11 access. Our tool provides a streamlined method for connecting to an X server in order to send commands and receive output hijacking the remote host. The provided user interface is designed to resemble a remote desktop connection apart from the added user input fields. Before using the tool, a vulnerable host will need to be found using available scanners or using the Nmap script we developed to find vulnerable hosts with currently active displays that can be hijacked.

## Requirements:
xwininfo

xwatchwin

xdotool

## Installation:
```
sudo apt-get install xdotool
wget http://old-releases.ubuntu.com/ubuntu/pool/universe/x/xwatchwin/xwatchwin_1.1.1-2_amd64.deb && sudo dpkg -i xwatchwin_1.1.1-2_amd64.deb && sudo apt-get install -f
```

## Usage:
```
python xrdp.py <IP>:<DP>
python xrdp.py 10.2.10.190:0
```

## Functionality:
spr		= toggle on + type character in entry + press enter to send

ctrl 		= toggle on + type character in entry + press enter to send

alt 		= toggle on + type character in entry + press enter to send

Enter 		= press button to send enter key

Backspace 	= press button to send backspace key

R-Shell 	= type ip:port + press button to automatically open terminal and run reverse shell then minimize window

## Authors:
Darryn@SensePost.com

Thomas@SensePost.com
