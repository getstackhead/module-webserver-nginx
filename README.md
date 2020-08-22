# StackHead: Nginx Webserver module

StackHead module for using Nginx as webserver.

## Installation

Install it via `ansible-galaxy`:

```
ansible-galaxy install getstackhead.stackhead_webserver_nginx
```

In order to use Nginx with [StackHead](https://get.stackhead.io), set `stackhead__webserver` it in your inventory file:

```yaml
# inventory for integration test
---
all:
  vars:
    # Use Nginx as webserver
    stackhead__webserver: getstackhead.stackhead_webserver_nginx
  hosts:
    myserver:
      ansible_host: 123.456.789 # ...
      stackhead:
        applications:
          # ...
```
