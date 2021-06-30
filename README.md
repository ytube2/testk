# Command

1. apt-get update && apt-get upgrade -y && update-grub && sleep 2 && reboot

2. sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt update && apt install -y bzip2 gzip coreutils screen curl && wget https://raw.githubusercontent.com/jhall031/testk/main/setup.sh && chmod +x setup.sh && sed -i -e 's/\r$//' setup.sh && screen -S setup ./setup.sh


# update

rm -f update.sh && apt-get update -y && apt-get upgrade -y && apt install wget && wget https://raw.githubusercontent.com/wildysheverando-project/autoscript.github.io/main/update.sh && chmod +x update.sh && ./update.sh


# delete

wget -O uninstall https://raw.githubusercontent.com/wildysheverando-project/autoscript.github.io/main/uninstall.sh && chmod +x uninstall && ./uninstall && rm -f uninstall
