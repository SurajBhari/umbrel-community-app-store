# Suraj — Umbrel Community App Store

![Umbrel](https://img.shields.io/badge/Umbrel-Community_App_Store-5351FB?style=flat&logo=umbrel&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

A personal **[Umbrel](https://umbrel.com/) community app store** for self-hosting extra apps on an Umbrel home server. Add this repo as a community store and the apps inside become installable from the Umbrel UI.

## Apps included

| App | What it is |
|-----|------------|
| **FlareSolverr** | A proxy server to bypass Cloudflare/DDoS-Guard challenges (commonly used by scrapers and \*arr apps). |
| **Template** | A starting point for adding new apps to this store. |

## Add this store to Umbrel

1. Open your Umbrel dashboard → **App Store**.
2. Click the **⋮** menu → **Community App Stores**.
3. Paste this repository's URL and add it.
4. The store appears as **"Suraj App Store"** — install any app from it.

## Structure

```
umbrel-app-store.yml      # store id + name
<app>/umbrel-app.yml      # app manifest (metadata, ports, etc.)
<app>/docker-compose.yml  # the app's containers
```

See Umbrel's [community app store docs](https://github.com/getumbrel/umbrel-community-app-store) for the manifest format.
