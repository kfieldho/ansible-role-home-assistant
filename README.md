Home Assistant Ansble Role
======================

Install [Home Assistant](https://home-assistant.io/) for a Raspberry Pi.  Tested on Rasbian Stretch.
Installs using [Pip](https://pypi.python.org/pypi/pip) 
and [venv](https://docs.python.org/3/library/venv.html).

Requirements
-------------------

Tested on Rasbian Stretch

Role Variables
--------------------



* `home_assistant_destination`: Location of the virtual environment containing Home Assistant (default: `/opt/homeassistant`)
* `home_assistant_config_file`: If specified, this file is installed in `~/.homeassistant/configuration.yaml` (default:  Allow home assistant to install its default configuration)

Dependencies
------------

None


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: kfieldho.home-assistant, home_assistant_config_file: "iot/configuration.yaml" }
```

Note: Role example configures Home Assistant with a custom configuration file stored in `files/iot/configuration.yaml`

License
-------

BSD

Author Information
------------------

Keith Fieldhouse
@kfieldho on GitHub
github@fieldhouses.net
