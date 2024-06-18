
## Context
The intention of the guide is to : 
- 
 
## References


## Requirements

-   [Hardware Needed for students and instructors]
	- **64bit linux distribution** 
		- running in virtual machine (VM) or dedicated server 
		- within a simple virtual machine on desktop if required. 
	-   two CPU / 3GB Memory / 32 GB Storages
-   [Software Needed for students and instructors]:
	- Docker
	-  Domain Name System (DNS) Server if possible
		- This will allow local domains such as mail.local
	-  Web Browser
- All devices on the same local network


## Instructions
### Handouts Required 
#### Opening
#### Lesson 01
#### Lesson 02
#### Lesson 03
#### Lesson 04
#### Lesson 05
#### Lesson 06
#### CAPSTONE
#### Closing

### Setup
#### Full Scripts
```BASH

```


#### By The Numbers
```BASH
#Install Docker
#commands if needed in the course
sudo apt update; sudo apt install -y docker docker.io
```

```BASH
#run docker command after modifying domain
#setting up a mail server or other services as needed for the POI if it directly calls for it
docker run \
    --net=host \
    -e TZ=America/New_York \
    -v /var/mailserver:/data \
    --name "mailserver" \
    -h "mail.example.local" \
    -t analogic/poste.io
```

