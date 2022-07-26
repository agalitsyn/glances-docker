# Glances using docker-compose

Copy of https://github.com/nicolargo/glances/tree/develop/docker-compose but image is replaced to use latest official release.

## Usage

1. `scp` to your server, move folder under `/opt`
2. Allow traffic
    - On host, add port to firewall, for example `sudo ufw allow 61208`
    - Ensure that security group in cloud provider allows port `61208`
3. cd into folder, run `docker-compose up -d`
4. open in browser <your-ip>:61208

None: port is configurable in docker-compose file
