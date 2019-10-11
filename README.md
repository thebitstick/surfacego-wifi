# surfacego-wifi
Automatically overrides ATH10K QCA6174 Wi-Fi Driver after firmware update

Put the two init scripts in `/etc/systemd/system`  
Then get the [proprietary binary driver](http://www.killernetworking.com/support/K1535_Debian/board.bin) and place it in `/opt/wifi-driver/board.bin`  
Then put the replacement `script` in `/opt/wifi-driver/script`  

Then:  
`$ sudo systemctl enable --now surfacego-wifi.path`
