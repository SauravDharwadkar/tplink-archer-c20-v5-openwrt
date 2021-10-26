# tplink-archer-c20-v5-openwrt-20-02-0
recompile version of offitial tplink config without ipv6 and ppp , and change libustream from wolfssl to openssl (required by tor so using common lib)
# optimize for tor ~500KB space remain after tor install on fresh system

How To Compile 

https://openwrt.org/docs/start

copy config.build to openwrt/.config

make menuconfig 


make -j$(nproc) or make or make -j4

#note
while acticating hidden service change the torrc HiddenServiceDir /var/lib/tor/hidden_service/ to HiddenServiceDir /root/lib/tor/hidden_service/ or change directory as you please just keep it under root directory so it wont change (clear from ram ) after reboot
