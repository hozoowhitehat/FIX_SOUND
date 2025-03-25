# FIX_SOUND 🔉🔊

git clone https://github.com/hozoowhitehat/FIX_SOUND

cd FIX_SOUND

docker run -d \
  -p 6080:80 \
  -v /tmp/.X11-unix:/tmp/.X11-unix \
  -e RESOLUTION=1920x1080 \
  -e PULSE_SERVER=unix:/run/user/1000/pulse/native \
  --name novnc \
  dorowu/ubuntu-desktop-lxde-vnc
  
