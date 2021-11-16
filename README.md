# Project is closed 

# Rtc-SSH
##### SSH (Secure Shell) over WebRTC
Rtc-SSH enables connection with SSH  Raspberry PI, BeagleBone and other devices, from the browser or (cli) client  <a href="https://github.com/mxseba/rtc-terminal">rtc-terminal</a>   using WebRTC. Solves the problem of the lack of public IP address, proxy server, servers behind NAT etc. You can connect to an SSH session: https://webrtc.sqs.io

### Install from binary
```
wget https://github.com/mxseba/rtc-ssh/releases/download/v0.3.1/rtc-ssh_0.3.1_Linux_armv7.tar.gz
tar xvfz rtc-ssh_0.3.1_Linux_armv7.tar.gz
cd rtc-ssh_0.3.1_Linux_armv7
./rtc-ssh -newkey
uuid xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
Signal OK
```
Other architectures and releases: https://github.com/mxseba/rtc-ssh/releases<br />

or get source using the Go compilator:

### Usage
```
go get -u github.com/mxseba/rtc-ssh
cd $GOPATH/bin
```
### First run
```
./rtc-ssh -newkey
uuid xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
Signal OK
```
Option <code>-newkey</code> usage only first run, enter the <b>uuid</b> key on the website: https://webrtc.sqs.io <br />
If ssh has a different port on our server than 22, set the option <code>-port=xxxx</code><br /><br />
Rtc-SSH uses the pion-WebRTC library: https://github.com/pion/webrtc

