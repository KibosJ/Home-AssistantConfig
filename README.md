# Home Assistant Configuration

## Hardware

**Device**
QNAP TS-451+

**CPU**
Intel(R) Celeron(R) CPU J1900 @ 2.00GHz (4 cores)

**RAM**
8GB

## Environment

**Install method**
Docker-Compose

**Docker version**
Docker version 17.09.1-ce, build 0bbe3ac

**docker-compose**

    home-assistant:
        image: homeassistant/home-assistant
        container_name: home-assistant
        hostname: home-assistant
        network_mode: host
        depends_on:
    	    - letsencrypt
    	environment:
    		- TZ=Europe/London
    	volumes:
    		- /share/Docker/home-assistant/config:/config
    	ports:
    		- 32561:8123
    	restart: always

## Other Docker Services

- [Plex Media Server](https://hub.docker.com/r/linuxserver/plex)
- [Letsencrypt Nginx server](https://hub.docker.com/r/linuxserver/letsencrypt)
- [Portainer](https://hub.docker.com/r/portainer/portainer)
- [Bitwarden Server](https://hub.docker.com/r/bitwardenrs/server)
- [Sabnzbd](https://hub.docker.com/r/linuxserver/sabnzbd)
- [Sonarr](https://hub.docker.com/r/linuxserver/sonarr)
- [Radarr](https://hub.docker.com/r/linuxserver/radarr)
- [MKVToolNix](https://hub.docker.com/r/jlesage/mkvtoolnix)
- [OpenVPN-AS](https://hub.docker.com/r/linuxserver/openvpn-as)
- [Grocy](https://hub.docker.com/r/linuxserver/grocy)

# Devices Used for Automation

## Lights

- [Hue Bridge](https://www2.meethue.com/en-gb/p/hue-hue-bridge/8718696516850)
- [Hue White Ambience Spotlight](https://www2.meethue.com/en-gb/p/hue-white-ambience-single-bulb-gu10/8718696598283) - 4x kitchen - 3x hallway
- [Hue White and Colour Ambience Spotlight](https://www2.meethue.com/en-gb/p/hue-white-and-colour-ambience-1-pack-gu10/8718699628659) - 3x living room
- [Hue White Ambience Bulb](https://www2.meethue.com/en-gb/p/hue-white-ambience-single-bulb-b22/8718696548813) - 1x landing - 1x bedroom
- [Hue Smart Button](https://www2.meethue.com/en-gb/p/hue-smart-button/8718699693985) - 1x living room - 1x kitchen - 1x landing - 1x bedroom - 2x hallway

## Media

- Living Room - [Apple TV 4K](https://www.apple.com/uk/apple-tv-4k/) - [SkyQ 2TB](https://www.sky.com/shop/tv/sky-q/) - [Sony Bravia KD-55XG8796](https://www.sony.co.uk/electronics/televisions/xg8505-series) - [Amazon Echo Dot](https://smile.amazon.co.uk/Echo-Dot-3rd-Gen-Charcoal/dp/B07PJV3JPR) - [Samsung R5 Wireless Speaker](https://www.samsung.com/uk/audio-video/multiroom-360-sound-speaker-wam5500/)
- Kitchen - [Apple iPad 6th Generation](https://smile.amazon.co.uk/2018-Apple-iPad-WiFi-32GB/dp/B07DVBRVQM/ref=sr_1_11?dchild=1&keywords=2018%20ipad&qid=1590746335&sr=8-11) - [Samsung R5 Wireless Speaker](https://www.samsung.com/uk/audio-video/multiroom-360-sound-speaker-wam5500/)
- Bedroom - [Amazon Echo Dot](https://smile.amazon.co.uk/Echo-Dot-3rd-Gen-Charcoal/dp/B07PJV3JPR)

# Home Assistant Configuration

## Integrations

- [Google Cast](https://www.home-assistant.io/integrations/cast/)
- [Homekit](https://www.home-assistant.io/integrations/homekit/)
- [Mobile App](https://www.home-assistant.io/integrations/mobile_app/)
- [Philips Hue](https://www.home-assistant.io/integrations/hue/)
- [Plex Media Server](https://www.home-assistant.io/integrations/plex/)
- [Shopping List](https://www.home-assistant.io/integrations/shopping_list/)
- [Sony Bravia TV](https://www.home-assistant.io/integrations/braviatv/)
- [Spotify](https://www.home-assistant.io/integrations/spotify/)
- [UPnP](https://www.home-assistant.io/integrations/upnp/)

## Custom Integrations

- [Alexa Media Player](https://github.com/custom-components/alexa_media_player)
- [Apple TV](https://github.com/postlund/hass-atv-beta)
- [Climacell Weather](https://github.com/r-renato/ha-climacell-weather)
- [Custom Header](https://github.com/maykar/custom-header)
- [Grocy Custom Component](https://github.com/custom-components/grocy)
- [HACS](https://github.com/hacs/integration)
- [Lovelace Layout-card](https://github.com/thomasloven/lovelace-layout-card)
- [Mini Media Player](https://github.com/kalkih/mini-media-player)

## Theme

[Google Dark Theme](https://github.com/JuanMTech/google_dark_theme)

# Screenshots

## Main Dashboard

![Main lovelace dashboard](https://raw.githubusercontent.com/KibosJ/Home-AssistantConfig/master/screenshots/Dashboard_main.png)

## Lights

![Lights tab](https://raw.githubusercontent.com/KibosJ/Home-AssistantConfig/master/screenshots/Dashboard_lights.png)

## Kitchen Dashboard

![Kitchen lovelace dashboard](https://raw.githubusercontent.com/KibosJ/Home-AssistantConfig/master/screenshots/Dashboard_kitchen.png)
