---
layout: home
title: Welcome
---

# ESPHome Device Configuration Repository

This website is a repository of device configuration templates and setup guides for devices running [ESPHome](https://esphome.io) firmware.

{% assign counter = 0 %}{% for item in site.devices %}{% assign counter=counter | plus:1 %}{% endfor %}
There are currently **{{ counter }} devices** documented in the repository.

## Recently Added Devices
{% assign devices = site.devices | sort: "date" | reverse %}
{% for device in devices limit:10 %}
* [{{ device.title }}]({{ device.url }})
{% endfor %} 

## Contributing
This repository relies on the community to keep it up-to-date and accurate. If you identify and errors or find a device that is not added please consider contributing.

[Adding Devices](/adding-devices){: .btn .btn-purple .mr-2 }
[Editing Devices](/editing-devices){: .btn .btn-purple .mr-2 }