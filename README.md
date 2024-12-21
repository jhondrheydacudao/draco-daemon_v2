# Hydra Daemon 

## Overview
Hydra Daemon is the daemon for the Hydra Panel.

## Installation
1. Clone the repository:
`git clone https://github.com/hydren-dev/HydraDAEMON`

2. Install dependencies:
`npm install`

3. Configure HydraDAEMON:
- Get your Panel's access key from the Hydra panel's config.json file and set it as 'remoteKey'. Do the same for the other way, set your Aird access key and configure it on the Panel.

4. Start the Daemon:
`node . # or use pm2 to keep it online`

## Configuration
Configuration settings can be adjusted in the `config.json` file. This includes the authentication key for API access.

or use

## Docker
```
docker pull ghcr.io/hydren-dev/daemon:latest
```
**Configure the `/etc/hydra/daemon.json`**
```json
{
  "panel": "https://panel.example.com",
  "key": "your-node-configure-key-here"
}
```
**Run the Container**
```
docker run -it --privileged ghcr.io/hydren-dev/daemon:latest
```

## Usage
The daemon runs as a background service, interfacing with the Hydra Panel for operational commands and status updates. It is not typically interacted with directly by end-users.

## Contributing
Contributions to enhance the functionality or performance of the Hydra Daemon are encouraged. Please submit pull requests for any enhancements.

## License
(c) 2024 MJ and contributors. This software is licensed under the MIT License.


## Credits
SRYDEN
