# wabot-aq
#### Simple WhatsApp 

# FOR TERMUX/UBUNTU/SSH USER
```
apt update && apt upgrade
apt install git -y
apt install nodejs -y
apt install ffmpeg -y
apt install imagemagick -y
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update
```

# INSTALL ON TERMUX WITH UBUNTU
# [ INSTALLING UBUNTU ]
```
apt update && apt full-upgrade
apt install wget curl git proot-distro
proot-distro install ubuntu
echo "proot-distro login ubuntu" > $PREFIX/bin/ubuntu
ubuntu
```
# [ INSTALLING REQUIRED PACKAGES ]
```
ubuntu
apt update && apt full-upgrade
apt install wget curl git ffmpeg imagemagick build-essential libcairo2-dev libpango1.0-dev libjpeg-dev libgif-dev librsvg2-dev dbus-x11 ffmpeg2theora ffmpegfs ffmpegthumbnailer ffmpegthumbnailer-dbg ffmpegthumbs libavcodec-dev libavcodec-extra libavcodec-extra58 libavdevice-dev libavdevice58 libavfilter-dev libavfilter-extra libavfilter-extra7 libavformat-dev libavformat58 libavifile-0.7-bin libavifile-0.7-common libavifile-0.7c2 libavresample-dev libavresample4 libavutil-dev libavutil56 libpostproc-dev libpostproc55 graphicsmagick graphicsmagick-dbg graphicsmagick-imagemagick-compat graphicsmagick-libmagick-dev-compat groff imagemagick-6.q16hdri imagemagick-common libchart-gnuplot-perl libgraphics-magick-perl libgraphicsmagick++-q16-12 libgraphicsmagick++1-dev
```
# [ INSTALLING NODEJS & WABOT-AQ ]
```
ubuntu
curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash -
apt install -y nodejs gcc g++ make
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update
```
# FOR WINDOWS/VPS/RDP USER

- Download And Install Git Click Here
- Download And Install NodeJS Click Here
 Download And Install FFmpeg Click Here (Don't Forget Add FFmpeg to PATH enviroment variables)
- Download And Install ImageMagick Click Here
```
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update
```
# Run
```
node .
```
# Arguments node . [--options] [<session name>]
### --session <file name>
Use another session with another name, default is session.data.json

### --prefix <prefixes>
prefixes are seperated by each character Set prefix
### --server
Used for heroku or scan through website

### --db <json-server-url>
Use external db instead of local db, Example Server https://json-server.nurutomo.repl.co/

Code: https://repl.it/@Nurutomo/json-server

node . --db 'https://json-server.nurutomo.repl.co/'

The server should have like this specification

### GET
```
GET /
Accept: application/json
```
### POST
```
POST /
Content-Type: application/json

{
 data: {}
}
```
### --big-qr
If small qr unicode doesn't support

### --img
Enable image inspector through terminal

### --test
Development Testing Mode

### --trace
conn.logger.level = 'trace'
### --debug
conn.logger.level = 'debug'
#Settings
Now set using switch enable.js, among others are
```
anticall: false, // Auto Reject better than autoblock
autoread: false, // If true all chats are automatically read
nyimak: false, // No bot, just print received messages and add users to database
restrict: false, // Enables restricted plugins (which can lead your number to be banned if used too often)
self: false, // Activate self mode (Ignores other)
pconly: false, // If that chat not from private bot, bot will ignore
gconly: false, // If that chat not from group, bot will ignore
jadibot: false, 
```
