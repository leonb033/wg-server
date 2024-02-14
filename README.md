# wg-server

This tool automates configuration of wireguard interfaces on Debian.

## Requirements
- Debian 12
- wireguard
- wireguard-tools

## Installation
`wget -O setup.sh https://raw.githubusercontent.com/leonb033/wg-server/main/setup.sh && bash setup.sh`

## Commands
### wg-server create \<INTERFACE\>
Sets up a new wireguard interface.

### wg-server delete \<INTERFACE\>
Deletes this wireguard interface.

### wg-server generate-keys \<INTERFACE\>
Generates new public and private key for this interface.

### wg-server add-peer \<INTERFACE\>
Adds a new peer to this interface.

### wg-server remove-peer \<INTERFACE\>
Removes a peer from this interface.

## Useful wireguard commands:
### sudo wg show
List all running wireguard interfaces.

### sudo systemctl [start/stop] wg-quick@\<INTERFACE\>.service
Start / stop this interface service.

### sudo systemctl [enable/disable] wg-quick@\<INTERFACE\>.service
Enable / disable autostart for this interface service.
