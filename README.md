# balena-pihole

[balena.io](https://www.balena.io/) multi-container base, configured to work with [pihole](https://hub.docker.com/r/pihole/pihole/)



## Getting Started

See [balena.io's documentation on getting started](https://www.balena.io/docs/learn/getting-started)



## Deployment

### Device Environment Variables

|Name|Value|
|---|---|
|`TZ`|`America/New_York` _[See [here](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) for more]_|
|`DNS1`|`1.1.1.1` _[Cloudflare DNS -- check out more [here](https://1.1.1.1)]_|
|`DNS2`|`1.0.0.1` _[Cloudflare DNS fallback]_|
|`DNSMASQ_LISTENING`|`wlan0`|
|`INTERFACE`|`wlan0`|
|`ServerIP`|_[external device ip]_|
|`WEBPASSWORD`|_[optional]_|


## Usage

* Browse to `http://<device-ip>:80/admin` to access the pi-hole admin interface _[Working on bringing support to accessing admin panel thru the device public URL]_
* Above you will find a list of **mandatory** device enviroment variables -- more variables can be found on [pihole's page on dockerhub](https://hub.docker.com/r/pihole/pihole/)



## Acknowledgments

Huge thanks to [Kyle Harding](mailto:kylemharding@gmail.com) for the help on this project, and his contribution to this topic on the [balena.io forums](https://forums.balena.io/t/pihole-in-debian-container-on-balenaos/4645/2).  See Kyle's GitHub repository for more info, along with the other following resources to get started on building your own project with [balena.io](https://www.balena.io/)!

* https://github.com/klutchell/balena-pihole
* https://github.com/balena-io-projects/multicontainer-getting-started
* https://github.com/pi-hole/docker-pi-hole/
