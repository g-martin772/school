# 1. Test year 3

## WLAN

[Wikipedia page on 802.11](https://en.wikipedia.org/wiki/IEEE_802.11)

![2.4_GHz_Wi-Fi_channels_(802.11b,g_WLAN).svg.png](2.4_GHz_Wi-Fi_channels_(802.11b,g_WLAN).svg.png)

![NonOverlappingChannels2.4GHz802.11-en.svg.png](NonOverlappingChannels2.4GHz802.11-en.svg.png)

### Standards:

| Wifi gen | IEE Standard | Year | 2,4GHz | 5Ghz | Max Data rate                   | Channel width  |
|----------|--------------|------|--------|------|---------------------------------|----------------|
| Wifi     | 802.11       | 1997 | Yes    | No   | 2 Mbps                          | 22 MHz         |
| Wifi 1   | 802.11b      | 1999 | Yes    | No   | 11 Mbps                         | 22 MHz         |
| Wifi 2   | 802.11a      | 1999 | No     | Yes  | 54 Mbps                         | 20 MHz         |
| Wifi 3   | 802.11g      | 2003 | Yes    | No   | 54 Mbps                         | 20 and 40 MHz  |             |
| Wifi 4   | 802.11n      | 2009 | Yes    | Yes  | bis 4x 150 Mbps -> Max 600Mbps  | 20 and 40 MHz  |
| Wifi 5   | 802.11ac     | 2013 | No     | Yes  | bis 8x 433 Mbps -> Max 6,93Gbps | 80 and 160 MHz |
| Wifi 6   | 802.11ax     | 2019 | Yes    | Yes  | 4x 802.11ac                     | 80 and 160 MHz |              |

Extra note for the 60GHz 802.11ad standard with a speed of 4.620 MBit/s or 6.757 MBit/s no idea and 2GHz channels

### Security

There actually are laws that force you to encrypt your Wifi because you could be hold accountable
for someone else using your connection for illegal actions.

| Type  | Name                     | Year | Considered Secure | Encryption  | KeySize           |
|-------|--------------------------|------|-------------------|-------------|-------------------|
| WEP   | Wired Equivalent Privacy | 1997 | Oh no             | RC4         | 40bit + 24bit IV  |
| WPA   | Wifi protected access    | 1999 | No                | TKIP        | 128bit per packet |
| WPA 2 | Wifi protected access 2  | 1999 | Yes               | AES -> CCMP | -                 |
| WPA 3 | Wifi protected access 3  | 2003 | Yes               | Extra BFP   | -                 |
| WPS   | Wifi Protected Setup     | 2009 | Yes               | -           | -                 |

WPA-Personal vs WPA-Enterprise with RADIUS Auth Server

### WIFI Channels

![wlan-frequenzen.png](wlan-frequenzen.png)

![WLAN-5GHz-Kanaele-Deutschland.png](WLAN-5GHz-Kanaele-Deutschland.png)

Why usually only pick channel 1, 6, and 11 on 2.4GHz band?
Every channel is 20MHz but they are only 5MHz apart!

![wlan-channel-1-6-11.png](wlan-channel-1-6-11.png)

![wlan-interference-2.png](wlan-interference-2.png)

### Interference

![wlan-interference1.png](wlan-interference1.png)

### Additional info

- Max send power = 200mW
- DFS - Dynamic frequency selection
- Without DFS only first 4 channels allowed
- ISM - Industrial, Scientific, Medicine
- Low band on 863Mhz for long range and IOT (prop more interference) bis 1km
- 1-6-11 in US is 1-7-13 in Europe

### WLAN-Topology

- IBSS - Independent Basic Service Set (Ad-hoc)
  - Not used much
  - No real encryption
  - Bad compatibility
  - Bluetooth better and easier
- BSS - Basic Service Set
  - Access point mit client
  - SSID (Service Set Identifier)
- ESS - Extended Service Set / IEEE 802.11c / Wireless Bridging
  - Connection between 2 Access points
- WDS - Wireless Distribution System (WLAN-Repeater)
  - Repeater sits between access point and client
- MIMO - Multiple Input Multiple Output
  - Multiple sender stations and maybe multiple recipients