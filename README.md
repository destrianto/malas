# Malas (Multi-vendor automation leverage at slouching)<br>
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/malas)](https://pypi.org/project/Malas)
[![PyPI](https://img.shields.io/pypi/v/malas)](https://pypi.org/project/Malas)
[![Downloads](https://pepy.tech/badge/malas)](https://pepy.tech/project/malas)
<br>
<br>
**What is 'Malas'?**<br>
_Malas_ is a word from Bahasa Indonesia. The _Malas_ word meaning is _Lazy_ (Too inclined to avoid hard work).<br>
<br>
**What Malas really is?**<br>
Malas is a simple multi-vendor network automation program powered by netmiko for general configuration or retrieve information via SSH parallelly.<br>
<br>
**Why Malas though?**<br>
Malas is an abstraction layer in a wizard-type CLI for simplicity's sake.
## Main features
- IPv4 target hosts.
- [Supported platforms](https://github.com/ktbyers/netmiko/blob/develop/PLATFORMS.md) based on netmiko.
- Verify submitted User's file formats before accepted.
- Performing _parallel_* connectivity tests before remote executions.<br>
*_Parallel tasks capabilities based on CPU's capabilities._
- Performing _parallel_* remote configurations or retrieve information.<br>
*_Parallel tasks capabilities based on CPU's capabilities._
- Show remote output results immediately.
- Save remote output results per-remote host (Optional).
- Auto-install missing modules (If uninstalled accidentally).
## WIP
- IPv6 target hosts
- Hostname target hosts
## Getting started
**Installation:**
```
python -m pip install malas
or
python3 -m pip install malas
```
**Start the program:**
```
python -m malas
or
python3 -m malas
```
**File formatting:**
```
1. The device information list file's format is a set of three
   that contains IP address, username (has privilege), and password separated by double colons '::'
   per line in row formats, for example (Ignore the bracket):

   #==== Device Information List.txt ====#
   #10.0.0.2::netadmin::password         #
   #10.0.0.3::netadmin::password         #
   #=====================================#

2. The configuration file's format is one command per line in row formats, for example (Ignore the bracket):

   #========= Configuration.txt =========#
   #interface GigabitEthernet0/11        #
   #description Guest_Networks           #
   #IP address 192.168.1.1 255.255.255.0 #
   #no shutdown                          #
   #exit                                 #
   #do write                             #
   #=====================================#

```
---
**Ade Destrianto**<br/>
https://destrianetworks.id
