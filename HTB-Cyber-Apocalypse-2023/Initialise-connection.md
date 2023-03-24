# Initialise-connection
---
creation date:  24-03-2023  21:03
tags: #Difficulty-VeryEasy #pwn
___
## Overview
![[images/initialiseConnection-overview.png]]
The overview for this challenge outlines the process of connecting to the deployed Docker instances throughout the event.

## Solution
### Spawn docker instance
![[images/initialiseConnection-docker.png]]
- After clicking the 'play' icon the Docker container starts and proivdes an IP address and port that we can use to connect and interact.

### Connecting to Docker instance
```bash
$ nc 142.93.38.14 30524
```

- After connecting to the Docker image, the following is displayed:

```bash
$ nc 142.93.38.14 30524

▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣
▣                            ▣
▣  Enter 1 to get the flag!  ▣
▣                            ▣
▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣

>>  
```

- Here we enter 1 and hit enter and recieve the flag.

```bash
nc 142.93.38.14 30524

▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣
▣                            ▣
▣  Enter 1 to get the flag!  ▣
▣                            ▣
▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣▣

>> 1
HTB{...}
```
