# Let's Play with Raspberry Pi

```text
ls ~/.ssh
```

```text
ssh-keygen -t rsa
```

```text
ssh-copy-id pi@raspberrypi
```

```text
ssh pi@raspberrypi
```

```text
sudo nano /etc/ssh/sshd_config
```

```text
#PasswordAuthentication yes
```

```text
PasswordAuthentication no
```

```text
sudo systemctl restart ssh
```

```text
sudo raspi-config
```

```text
sudo apt update
```

```text
sudo apt upgrade -y
```

```text
sudo reboot
```

```text
sudo poweroff
```

## Mosquitto (MQTT Broker)

```text
sudo apt install -y mosquitto
```

```text
sudo systemctl start mosquitto
```

```text
sudo systemctl enable mosquitto
```

```text
sudo nano /etc/mosquitto/mosquitto.conf
```

```text
bind_address 0.0.0.0
allow_anonymous true
# log_type debug
```

```text
sudo systemctl restart mosquitto
```

```text
sudo tail -n 20 /var/log/mosquitto/mosquitto.log
```

```text
ip a
```

## Node.js

```text
uname -m
```

```text
wget https://nodejs.org/dist/v18.12.1/node-v18.12.1-linux-armv7l.tar.xz
```

```text
VERSION=v18.12.1; echo $VERSION
```

```text
DISTRO=linux-armv7l; echo $DISTRO
```

```text
sudo mkdir -p /usr/local/lib/nodejs
```

```text
sudo tar -xJvf node-$VERSION-$DISTRO.tar.xz -C /usr/local/lib/nodejs 
```

```text
nano ~/.profile
```

```text
# Nodejs
VERSION=v18.12.1
DISTRO=linux-armv7l
export PATH=/usr/local/lib/nodejs/node-$VERSION-$DISTRO/bin:$PATH
```

```text
. ~/.profile
```

```text
node -v
```

```text
npm version
```
