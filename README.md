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
