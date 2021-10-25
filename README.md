# tplink-archer-c20-v5-openwrt-20-02-0
recompile version of offitial tplink config without ipv6 and ppp , and change libustream from wolfssl to openssl (required by tor so using common lib)


How To Compile 

https://openwrt.org/docs/start

copy config.build to openwrt/.config

make menuconfig 


make -j$(nproc) or make or make -j4

