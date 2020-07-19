# Ad blocking

Advertisements are bad for our ecosystem or computer. The majority of threats to users come through malicious advertisements displayed on mainstream websites \(source - [ZDNet](https://www.zdnet.com/article/hackers-have-breached-60-ad-servers-to-load-their-own-malicious-ads/) and [paper](https://users.cs.northwestern.edu/~ychen/Papers/ndss16.pdf)\). plus blocking advertise has multiple security and performance benefits too.

We can implement blocking mechanism on three different levels of infrastructure using feature called "Filter Lists" \(Host file with blacklisted URL rules\).

1. [Application based \(i.e Browsers extensions\)]()
2. [Operating system based]()
3. [DNS based]()

### Application based

Modern browsers depend on browser extensions to block the content. After reviewing options, "[uBlock Origin](https://github.com/gorhill/uBlock)" is the clear winner \(for me\). It's open-source, performs better than other extensions and has multiple filter list options available too.

### OS based

A hosts file is a plain-text file used by all operating systems to map hostnames to IP addresses. In most OS, the hosts file is preferential to DNS. Therefore if a domain name is resolved by the hosts file, the request never leaves your computer.

traditionally `127.0.0.1` is a loopback address used by local machine to establish a connection, whereas `0.0.0.0` is defined as non-routable meta-address used to designate an invalid, unknown, or non-applicable target.

So, Using `0.0.0.0` is much faster, possibly because there's no wait for a timeout resolution.\(Source - [Steven Black](https://github.com/StevenBlack/hosts/blob/master/readme.md)\)

File path for windows - `..\Windows\System32\drivers\etc\`

File path for Linux/Android - `/etc/hosts`

Note- you will require root permission to modify hosts file in android. [Adaway](https://github.com/AdAway/AdAway) is an open-source adblocker for Android which utilize the hosts file method.

### DNS

The Domain Name System \(DNS\) is the internet’s version of the Yellow Pages. DNS servers can be configured to block access to domains known to serve ads by spoofing the address.

Users can either use a modified DNS server or they can setup their own by deploying projects like [Pi-hole](https://pi-hole.net/) [\(Github\)](https://github.com/pi-hole/pi-hole) a Raspberry Pi device that doesn’t only hide ads, it blocks the connection between your network and the domains you blacklist completely. You set the IP of your Raspberry Pi running Pihole as your DNS server and that’s it. It comes preconfigured with a lot of blacklisted domains, but there are tons of lists you can add to block even more.

Cisco Umbrella is a commercial alternative for the enterprise.

### Recursive Local VPN

Applications can run a local VPN connection with its own host filtering ability and DNS address without requiring root access. Android application like [Blokada](https://blokada.org/) [\(Github\)](https://github.com/blokadaorg/blokada) and [DNS66](https://jak-linux.org/projects/dns66/) [\(Github\)](https://github.com/julian-klode/dns66) are such apps which accomplish adblocking without root permission.

[Adaway](https://github.com/AdAway/AdAway) is also in process to include vpn-based blocking in its future release.

### Build-Your-Own-List

* [Multi-purpose Filter List](https://filterlists.com/)
* [Steven Black](https://github.com/StevenBlack/hosts/blob/master/data/StevenBlack/hosts)
* [Lenny Zeltser](https://zeltser.com/malicious-ip-blocklists/)
* [Energized Protection](https://energized.pro/)
* [Easy List](https://easylist.to/)
* [HpHosts](https://hosts-file.net/)

### ATT&CK ID

[Mobile - T1472](https://attack.mitre.org/techniques/T1472/)

### Links

* [Bromite](https://github.com/bromite/bromite) - Chromium plus ad blocking and privacy enhancements; take back your browser.
* [Ad blocking with Raspberry Pi and Pi-hole \(2020\)](https://cri.dev/posts/2020-05-03-Ad-blocking-with-Raspberry-Pi-and-Pi-hole/) \([HN](https://news.ycombinator.com/item?id=23073109)\)
* [Should I Block Ads? \(2020\)](https://shouldiblockads.com/) \([HN](https://news.ycombinator.com/item?id=23276117)\)

