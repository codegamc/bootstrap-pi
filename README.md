# bootstrap-pi
Bootstrap your pi

The goal is to enable someone to start using a pi quickly and easily without dedicating a monitor or keyboard to the pi. They install the linux distro on their pi, plug it in, and it comes configured and ready to use, complete with a VNC server accessible over a browser.

* mDNS discovery, potentially a fallback 
* [noVNC](https://github.com/novnc/noVNC) web-based VNC client.
* Need a cert, self signed, the user accepts the risk warning. see [let's encrypt](https://letsencrypt.org/docs/certificates-for-localhost/) for why
* config is baked right into the OS image when its written to disk.

Other thoughts:

The main computer can add info like MAC address or IP address to the pi so the pi can try and connect immediately (useful when mDNS might not be supported)

A GUI app (eg. electron) to view the VNC stream is not ideal because then it restricts the ability to use other devices (phone, tablet) to control the pi. This is less flexible and provides less opportunity to people using the pi.
