# Advertisements

<p align="center">
  <img src="undraw_surveillance.png" width="500">
</p>

Advertisements are bad for our ecosystem or computer. The majority of threats to users come through malicious advertisements displayed on mainstream websites. plus blocking advertising has multiple security and performance benefits too.

Advertisements can be blocked on three different levels and with the help of a feature called "Filter Lists" (File with blacklisted URL rules)
1. [Browser](#browser-based)
2. [Operating System](#system-based)
3. [DNS](#dns-filtering)

## Browser based
Modern browsers depend on browser extensions to block the content. After reviewing options, "[uBlock Origin](https://github.com/gorhill/uBlock)" is the clear winner (for me). It's open-source, performs better than other extensions and has multiple filter list options available too.

## System based
A hosts file is a plain-text file used by all operating systems to map hostnames to IP addresses. In most OS, the hosts file is preferential to DNS. Therefore if a domain name is resolved by the hosts file, the request never leaves your computer.

traditionally `127.0.0.1` is a loopback address used by local machine to establish a connection, whereas `0.0.0.0` is defined as non-routable meta-address used to designate an invalid, unknown, or non-applicable target.

So, Using `0.0.0.0` is much faster, possibly because there's no wait for a timeout resolution.(Source - [Steven Black](https://github.com/StevenBlack/hosts/blob/master/readme.md))

File path for windows - `..\Windows\System32\drivers\etc\`

File path for Linux/Android - `/etc/hosts`

Note- root permission is required to replace hosts file in android. AdAway is an open-source ad blocker for Android which utilize the hosts file method.

## DNS Filtering
The Domain Name System (DNS) is the internet’s version of the Yellow Pages. DNS servers can be configured to block access to domains known to serve ads by spoofing the address. Users can use a modified DNS server or they can set up their server by deploying projects like [Pi-hole](https://pi-hole.net/) [(Github)](https://github.com/pi-hole/pi-hole).

Cisco Umbrella is a commercial alternative for the enterprise.

## Recursive Local VPN
Applications can run a local VPN connection with its own host filtering ability and DNS address without requiring root access. [Blokada](https://blokada.org/) [(Github)](https://github.com/blokadaorg/blokada) and [DNS66](https://jak-linux.org/projects/dns66/) [(Github)](https://github.com/julian-klode/dns66), are popular apps which accomplish adblocking without root permission.

## Build-Your-Own-List
- [Multi-purpose Filter List](https://filterlists.com/)
- [Steven Black](https://github.com/StevenBlack/hosts/blob/master/data/StevenBlack/hosts)
- [Lenny Zeltser](https://zeltser.com/malicious-ip-blocklists/)
- [Energized Protection](https://energized.pro/)
- [Easy List](https://easylist.to/)
- [HpHosts](https://hosts-file.net/)

## ATT&CK ID
[Mobile - T1472](https://attack.mitre.org/techniques/T1472/)
