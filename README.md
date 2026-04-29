# NZB Mule

NZB Mule is a lightweight iOS helper app for opening `nzblnk://` links and `.nzb` files, then sending them directly to your selected download client.

The app supports both **NZBGet** and **SABnzbd**.

## Features

- Open `nzblnk://` links on iPhone or iPad
- Open or share `.nzb` files to the app
- Send NZBs directly to NZBGet
- Send NZBs directly to SABnzbd
- Store client settings securely in the iOS Keychain
- Scan SABnzbd API keys via QR code
- Supports local HTTP and HTTPS connections
- Simple client selection between NZBGet and SABnzbd

## How It Works

1. Choose your download client: NZBGet or SABnzbd.
2. Enter your local connection settings.
3. Open an `nzblnk://` link or share a `.nzb` file to NZB Mule.
4. NZB Mule sends the NZB to your selected client.

For `nzblnk://` links, NZB Mule searches for the matching NZB file and forwards it to your configured client.

For regular `.nzb` files, NZB Mule reads the file directly and forwards it without searching.

## Requirements

- iOS device
- A running NZBGet or SABnzbd instance
- Local network access to your download client
- SABnzbd API key if using SABnzbd
- NZBGet username/password if using NZBGet

## SABnzbd Setup

In SABnzbd, make sure your server is reachable from your iOS device.

Check:

- Host is not limited to `localhost` only, set to 0.0.0.0
- Port is reachable from your local network
- API key is copied or scanned into NZB Mule
- Firewall allows local connections

If you use HTTPS with a self-signed SABnzbd certificate, NZB Mule can connect to your local instance.

## NZBGet Setup

Enter your NZBGet connection details:

- IP address
- Port
- Username
- Password

NZB Mule sends NZBs to NZBGet through its JSON-RPC API.

## Opening NZB Files

NZB Mule can be selected from the iOS share sheet for `.nzb` files.

Typical flow:

1. Download or save an `.nzb` file.
2. Tap Share.
3. Choose NZB Mule.
4. The app forwards the NZB to your selected client.

## Opening NZBLNK Links

When an `nzblnk://` link is opened on your device, NZB Mule launches automatically and processes the link.

## Privacy

NZB Mule does not host, provide, or distribute downloadable content.

The app only processes links and files that you open yourself and forwards NZB data to your configured download client.

Client settings are stored locally on your device using the iOS Keychain.

## Support

For issues, bug reports, or feature requests, please use the GitHub Issues tab.

## Disclaimer

NZB Mule is an independent utility app and is not affiliated with NZBGet, SABnzbd, NZBKing, or NZBIndex.

Users are responsible for ensuring that they comply with all applicable laws and terms of service when using NZB files, Usenet services, or download clients.

## License

All rights reserved.

© 2026 JS
