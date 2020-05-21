# Manjaro Basics

1. `sudo -Syu <package to install>`

2. `sudo -Rs <package to delete along with dependencies>`
   
3. git autocompletion in manjaro - ```sudo pacman -S bash-completion```

4. Setting DNS server
   ```
   sudo nano /etc/resolvconf.conf
   sudo resolvconf -u
   ```

5. OpenVPN config and startup
   ```
   sudo openvpn --config '/home/rafayat-lappy/Documents/impulsebd.ovpn'
   ```

6. Kill a certain port
   ```
   fuser -k 8000/tcp
   ```

7. Increase the maximum number of file watches
   ```
   echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf

   sudo sysctl -p
   ```
