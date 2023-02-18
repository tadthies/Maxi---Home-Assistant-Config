# Network Infrastructure




## Network Segregation:

Running a homelab is not always easy, especially when comes time to route, segregate and firewall multiple networks, each with a very specific use. I ended up with with 6 different networks:
1) Private LAN
   - This network is meant for my usage only. This is where all the main machines are connected, Servers and Main PC. No guests are allowed on this network.
2) Friends LAN
   - This is the "Hotspot" network that I offer to my guests during events. They cannot interact with other networks except for the "Google Cast" network, to allow them to cast to the speakers and chromecasts.
3) IoT LAN
   - This network is reserved for the IoT devices, a few ports are allowed in and out to the "Home-Assistant" Virtual Machine, such as LIFX ports and MQTT ports.
4) Google Home Network
   - This network is reserved for the very chatty Google Home devices. MDNS is enabled from this network to "Private" and "Friends" lan, to allow for control and cast of media content.
5) Game Server LAN
   - This network is higly restricted as the machine living on it is directly exposed to the internet on many ports to allow for game servers such as; Minecraft, Valheim, Conan, ARK, 7 days to die, Project Zomboid. Only a few ports are allowed within the lan. I.e: Inbound port 22 from my PC.
6) Cameras
   - This network is only accessible from the "Frigate" machine. Cameras can only see that machine and cannot ping home.

## Buy again notes:

| Symbol | Means |
| :---: | --- |
| :heavy_check_mark: | Yes |
| :pause_button: | Waiting on the next generation of this. |
| :grey_question: | Maybe - it's not bad, but I'm looking for something better |
| :thumbsdown: | Unlikely, it's not terrible, but it has some issues |
| :small_red_triangle: | There's a newer version that's better |
| :no_entry: | Discontinued |
| :warning: | Won't buy again |

# WiFi Infrastructure
|  Model      | Device Type |Buy Again? |Some Notes |  Quantity In Use     |
| ----------- | ----------- | :----------: |  ----------- | ----------- |
| 	[USG-3P](https://store.ui.com/products/unifi-security-gateway) | Router  |:small_red_triangle:   | Decent router, good network options. Requires a UNIFI controller | 1 |
| [U6-Lite](https://store.ui.com/collections/unifi-network-wireless/products/u6-lite-us) | Access Points | :grey_question:  | I can only reach 400Mbps with these Antennas in Wifi6 |   3 |
| [U6-PRO](https://store.ui.com/collections/unifi-network-wireless/products/unifi-ap6-professional) | Access Points | :heavy_check_mark: |More decent speeds at 700Mbps|   1 |
| [USW-Flex-Mini](https://store.ui.com/collections/unifi-network-switching/products/usw-flex-mini) | Switches |:heavy_check_mark:|Good little switch, not too pricey| 3 |
|   [USW-Lite-8-PoE](https://store.ui.com/collections/unifi-network-switching/products/unifi-switch-lite-8-poe)| Switches|:heavy_check_mark: |Also decent POE switch for edge of the network.| 2 |
| Ethernet Cat6 | Cable    |:heavy_check_mark:| |   Lots |


# WiFi devices

| Model | Device Type | Buy Again? | Some Notes |  Quantity In Use     |
| ----- | ----------- | :--------: | ---------- | :---: |
| Chromecast | Smart TV Dongle | :small_red_triangle: | Very decent integration into Home-Assistant| 1 | 
|[Chromecast Ultra](https://www.bestbuy.com/site/google-chromecast-ultra-4k-streaming-media-player-black/5578628.p?skuId=5578628) | Smart TV Dongle | :small_red_triangle: | Very decent integration into Home-Assistant| 3 | 
|[Google Nest Mini](https://store.google.com/product/google_nest_mini?hl=en-US&pli=1) | Smart speaker | :heavy_check_mark: | | 11|
|[Google Home Mini](https://store.google.com/product/google_nest_mini?hl=en-US&pli=1)| Smart Speaker | :small_red_triangle: || 5 |
|[LIFX Tiles](https://support.lifx.com/lifx-tile-H1b_fuiLu)| Smart Lights | :no_entry: | Very pretty, but one set out of two broke (Firmware issues) | 1 |
|[LIFX Nightvision BR30](https://www.lifx.com/products/lifx-color-br30-nightvision-edition-1pk)| Smart Bulb | :thumbsdown: | Very bright, but has wifi connectivity issues | 1 |
|[LIFX Color E26 ](https://www.lifx.com/products/lifx-color-1pk)| Smart Bulb | :thumbsdown: | Very bright, but has wifi connectivity issues | 1 |
|[ESP32 ](https://www.espressif.com/en/products/modules/esp32)| micro-controllers | :heavy_check_mark:  | Use ad BLE trackers | 7 |