+++
title = "Portfolio"
#date = "2014-04-09"
menu = "main"
weight = "40"
meta = "true"

+++

The collection of my professional projects.

---

## Cisco Systems: 2024 - ongoing
- Solely designed, prototyped and developed software using a third party serial Bluetooth dongle to collect BLE MAC addresses for an IoT application.
    - Third party dongle received AT commands over DB9 cabling, spews back binary data ended by b"\r\nOK\r\n".
    - Used an Inquiry Bluetooth scan to query for nearby devices within a ~30m radius.
    - Normalised, transmitted the data via a proprietary 22-byte network protocol. 
    - Used the container orchestration system (IOx) of IR1101 router to host dockerised service. 
    - Circa 2 months project part-time. $2M sales outcome.

- Automated firewall (FXOS) builds via API using YAML configuration templates. Setting up interfaces, port-channels, AAA, NTP, syslog, backups, logical device(s). 
    - Three layered solution - Parser, FXOS, Model(s).
    - Uses YAML to define template configurations, read by Parser object.
    - FXOS object offers connection to device and main logic of the application.
    - Model objects contain logic for configuring the equivalent API model(s).
    - ~1 month project part-time. Lack of interest from business :( 
- Automatic population of Zscaler PoP IP addresses as FMC Dynamic Objects using Ansible.
    - Wrote playbook to initialise FMC environment with two Dynamic Objects - zscaler_hubs, zscaler_cenr
    - Wrote playbook to handle GET requests to Zscaler API endpoints for Hubs and CENR addresses, parse and normalise JSON.
    - In same playbook, made relevant calls to FMC Ansible Galaxy module to populate Dynamic Object with JSON data, push objects to ACP rule.
    - Found bugs in the Galaxy module that prevented expected ease, had to find work arounds...
    - ~1 month project part-time. Lots of waiting on the client.
- Zscaler Internet Access Jinja2 document for policy visibility.
    - Wrote Jinja2 Word/docx template using docxtpl library.
    - Wrote class to handle and normalise data that is wanted from ZIA API.
    - Pass data from class to template. Eazy peazy.
    - ~1 week project part-time, if that. Lots of waiting for the API key from client.