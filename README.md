# Hawa Hawai V2 — OpenVPN TCP controller

This version is designed for the easiest free mobile build path.

## What it does
- Imports a standard OpenVPN `.ovpn` profile
- Requires the profile to use TCP
- Connect / Disconnect controls
- Shows OpenVPN status callbacks
- Connection timer
- Internet / public-IP test
- Does not store the profile contents in GitHub or bundle live VPN credentials

## VPN engine
Hawa Hawai V2 uses the external API of the free **OpenVPN for Android**
application (`de.blinkt.openvpn`) as the VPN engine. The engine must be installed
on the Android phone.

The external-control API and remote example are provided by the OpenVPN for
Android project for controlling it from another app. The API/remoteExample code
is exempted from the project's GPL restrictions and is provided for external
control use. See upstream licensing before redistribution.

## Provider profile
Use a TCP `.ovpn` file from a VPN provider/server that you own or are authorized
to use. Some providers require separate OpenVPN username/password credentials.

## Privacy
Never upload a live `.ovpn` profile containing credentials, private keys,
certificates, or tokens to a public GitHub repository.
