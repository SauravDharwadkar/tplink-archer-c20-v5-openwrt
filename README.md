# tplink-archer-c20-v5-openwrt-20-02-0
recompile version of offitial tplink config without ipv6 and ppp , and change libustream from wolfssl to openssl (required by tor so using common lib)
# optimize for tor ~488KB space remain after tor install on fresh system

How To Compile 

https://openwrt.org/docs/start

copy config.build to openwrt/.config

make menuconfig 


make -j$(nproc) or make or make -j4

