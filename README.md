# SD-WAN APIs Integration

Cisco has provided a full-fledged Python-based SDK for Cisco vManage that has tools, libraries, and documentation to simplify the interactions with the REST API. It is intended for engineers interested in automating the administration and operation of the SD-WAN solution using Python without any GUI interaction.

There are many great things that you can do when using Cisco vManage programmatically. A few typical use-cases are:

* Software integrations with other platforms;
* Programatically keeping track of device status and acting upon change;
* Management of policies and device templates in an automated fashion;
* Automated backup and restore;
* Automatic querying and aggregating of device and traffic statistics.
* CI/CD integrations;


![vmanage-python-sdk](./screenshot/vmanage-python-sdk.png)

Cisco SD-WAN has been designed with automation and extensibility in mind. Cisco vManage provides northbound RESTful APIs that allow customers to build their own unique business logic on top of the SD-WAN solution. For example, enterprises can integrate their existing OSS (Operational Support System) and BSS (Billing Support System) tools and consume telemetry data, automate incident tickets creation and lifecycle, and automate the deployment of new services.

The northbound APIs open a new world of possibilities to network engineers as well. Many trivial operational tasks that consume lots of time and effort in a large-scale environment can be easily automated. For example, configuration audits, network/security audits, inventory reports, automated backup/restore, 3rd-party tools integration, and so on.

![cisco-sdwan-rest-apis](./screenshot/cisco-sdwan-rest-apis.png)

## Requirements

To use this code you will need:

* Python 3.7+
* vManage user login details.

## Install and Setup

- Clone the code to local machine.

```
git clone https://github.com/sbarissonmez/sd-wan_api_integration.git
cd sd-wan_api_integration
```
- Setup Python Virtual Environment (requires Python 3.7+)

```
python3.7 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
```

- Create **vmanage_login.yaml** using below sample format to provide the login details of vManage

## Example:

```
# vManage Connectivity Info
vmanage_host:
vmanage_port:
vmanage_username:
vmanage_password:
```
