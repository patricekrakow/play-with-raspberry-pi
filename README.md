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
