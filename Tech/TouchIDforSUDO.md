# You can use TouchID for sudo in MacOS

Last tested **Sequoia 15.4.1**

Change mask for files ```sudo``` and ```sudo_local.template``` as they are readonly. In ```sudo_local.template``` uncomment line with ```pam_tid.so``` and copy it - we'll need it further:
```bash
cd /etc/pam.d/
sudo chmod 644 sudo sudo_local.template
sudo nano sudo_local.template
```

Add copied line into this file as the first row:
```bash
sudo nano sudo
```

You should get something like that (and some rows after):
```bash
# sudo: auth account password session
auth       sufficient     pam_tid.so
```

Return mask back for files:
```bash
sudo chmod 444 sudo sudo_local.template
```

Why edit sudo_local.template: 
> sudo_local: local config file which survives system update and is included for sudo uncomment following line to enable Touch ID for sudo

[source](https://t.me/the_tigor/290)
