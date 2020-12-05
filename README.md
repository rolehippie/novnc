# novnc

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/novnc) [![Build Status](https://img.shields.io/drone/build/rolehippie/novnc/master?logo=drone)](https://cloud.drone.io/rolehippie/novnc) [![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/novnc)](https://github.com/rolehippie/novnc/blob/master/LICENSE) 

Ansible role to install and configure noVNC via easy-novnc. 

## Sponsor 

[![Proact Deutschland GmbH](https://proact.eu/wp-content/uploads/2020/03/proact-logo.png)](https://proact.eu) 

Building and improving this Ansible role have been sponsored by my employer **Proact Deutschland GmbH**.

## Table of content

* [Default Variables](#default-variables)
  * [novnc_address](#novnc_address)
  * [novnc_arbitrary_hosts](#novnc_arbitrary_hosts)
  * [novnc_arbitrary_ports](#novnc_arbitrary_ports)
  * [novnc_basic_ui](#novnc_basic_ui)
  * [novnc_binary_checksum](#novnc_binary_checksum)
  * [novnc_binary_url](#novnc_binary_url)
  * [novnc_binary_version](#novnc_binary_version)
  * [novnc_cidr_blacklist](#novnc_cidr_blacklist)
  * [novnc_cidr_whitelist](#novnc_cidr_whitelist)
  * [novnc_default_view_only](#novnc_default_view_only)
  * [novnc_host](#novnc_host)
  * [novnc_hosts_selection](#novnc_hosts_selection)
  * [novnc_no_url_password](#novnc_no_url_password)
  * [novnc_params](#novnc_params)
  * [novnc_port](#novnc_port)
  * [novnc_verbose](#novnc_verbose)
* [Dependencies](#dependencies)
* [License](#license)
* [Author](#author)

---

## Default Variables

### novnc_address

Address to listen on for the service

#### Default value

```YAML
novnc_address: 0.0.0.0:8080
```

### novnc_arbitrary_hosts

Allow connections to other hosts

#### Default value

```YAML
novnc_arbitrary_hosts: false
```

### novnc_arbitrary_ports

Allow connections to other ports

#### Default value

```YAML
novnc_arbitrary_ports: false
```

### novnc_basic_ui

Hide connection options from the main screen

#### Default value

```YAML
novnc_basic_ui: false
```

### novnc_binary_checksum

Checksem of the binary release

#### Default value

```YAML
novnc_binary_checksum: sha256:395407ae7e824a7706bc259f0b8fc1c8b98b068a4bb76a3139b02c8a331be5b3
```

### novnc_binary_url

URL where to get the binary release from

#### Default value

```YAML
novnc_binary_url: https://github.com/pgaskin/easy-novnc/releases/download/v{{ novnc_binary_version
  }}/easy-novnc_linux-64bit
```

### novnc_binary_version

Version of the binary to download

#### Default value

```YAML
novnc_binary_version: 1.1.0
```

### novnc_cidr_blacklist

List of CIDR blacklist if arbitrary hosts are enabled

#### Default value

```YAML
novnc_cidr_blacklist: []
```

### novnc_cidr_whitelist

List of CIDR whitelist if arbitrary hosts are enabled

#### Default value

```YAML
novnc_cidr_whitelist: []
```

### novnc_default_view_only

Use view-only by default

#### Default value

```YAML
novnc_default_view_only: false
```

### novnc_host

Default host to connect to

#### Default value

```YAML
novnc_host:
```

### novnc_hosts_selection

List of host selection allowed to connect to

#### Default value

```YAML
novnc_hosts_selection: []
```

### novnc_no_url_password

Do not allow password in URL params

#### Default value

```YAML
novnc_no_url_password: false
```

### novnc_params

List of extra params for noVNC

#### Default value

```YAML
novnc_params: []
```

### novnc_port

#### Default value

```YAML
novnc_port:
```

### novnc_verbose

Default port to connect to

#### Default value

```YAML
novnc_verbose: false
```

## Dependencies

* None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
