# nftables persistent firewall configuration

Configuration files for Linux kernel iptables firewall. Read [this article](https://cryptsus.com/blog/advanced-perimeter-based-iptables-firewall-on-linux.html) for more information.

Make nftables configuration persistent on start-up:
```bash
$ systemctl enable nftables
$ systemctl start nftables
$ systemctl status nftables
```

File location:
```bash
$ vi /etc/nftables.conf
```

Test config file:
```bash
$ systemctl restart nftables && systemctl status nftables && nft list ruleset
```

# License
Berkeley Software Distribution (BSD)

# Author
[Jeroen van Kessel](https://twitter.com/jeroenvkessel) | [cryptsus.com](https://cryptsus.com) - we craft cyber security solutions
