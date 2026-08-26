# Rampage LAN Play Guide

## Current beta status

Rampage can currently connect two PCs to the same private LAN room. The room server, room code, two-player limit, connection status, reconnection credentials, and abandonment timer are implemented.

## What both players need
- Two Windows PCs connected to the same home Wi-Fi or Ethernet network
- The same Rampage beta version on both PCs
- The Windows network should be marked **Private**, not Public
- No Internet connection, cloud account, router port forwarding, or public IP address is required

## Host a room
1. Start Rampage on the PC that will act as the host
2. If Windows Firewall asks whether Rampage may communicate, allow it on **Private networks only**
3. Open **Play Match**, then select **Create/Join Online Game**
4. Leave **Host PC Address** blank
5. Select **Host on This PC**
6. Give the displayed four-character room code to the other player
7. Keep Rampage running on the host PC while the room is in use

## Find the host PC address
1. On the host PC, open PowerShell or Command Prompt
2. Run `ipconfig`
3. Find **IPv4 Address** under the active Wi-Fi or Ethernet adapter. It normally resembles `192.168.1.25` or `10.0.0.14`
4. Give that local address to the joining player. Do not use the router's public IP address

## Joining a room and starting a game
1. Start Rampage on the second PC
2. Each player should select a legal deck from the Play Match > Matching Menu
> Note: Any legal deck (Constructed/Draft/Generated) may be matched against any other legal deck
4. Open **Play Match**, then select **Create/Join Online Game**
5. Enter the host's local IPv4 address in **Host PC Address**. The `:3000` port is optional; Rampage adds it automatically when omitted
6. Enter the four-character room code
7. Select **Join Host**
8. The LAN Lobby should list both players as **Connected** and the Match should begin
> Note: The server on the host PC creates one authoritative engine after both players are connected. Clients send only commands — cast, target, attack, defend, pass, etc. The server validates and dispatches each command,
then broadcasts the resulting state. Disconnect timeout (2 minutes) results in a forfeit. The existing match UI is adapted to consume either the current local CPU adapter or a network-backed LAN adapter.

## Troubleshooting
If the second PC cannot connect:
1. Confirm both PCs are on the same home network and neither is using a VPN
2. Confirm the address belongs to the host's active Wi-Fi or Ethernet adapter
3. On the joining PC, open `http://HOST-ADDRESS:3000/health` in a browser, replacing `HOST-ADDRESS` with the host IPv4 address. A reachable server returns a short JSON response containing `"ok":true`
4. Allow Rampage on Private networks in Windows Firewall
5. Avoid guest Wi-Fi, which may prevent devices from communicating with one another
6. Restart Rampage on the host and create a new room code.

## Disconnects and room lifetime
- LAN rooms are kept in memory and are not saved to disk
- A disconnected player has a two-minute reconnection window
- When both players disconnect, the room remains for five minutes before being deleted
- Closing the host application ends all rooms hosted by that PC

## Home-network safety
Use LAN mode only on a trusted private network. Do not configure router port forwarding, expose port 3000 to the Internet, or share a public IP address
