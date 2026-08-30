# DTstudio — releases

Distribution assets for [DTstudio](https://dtstudio-landing.netlify.app), a
visual editor and generator for Device Trees. The application source lives
elsewhere; this repository only carries what the app and the website download.

Each release publishes three assets:

| Asset | What it is |
|---|---|
| `dtstudio_amd64.deb` | The Linux package. The name carries no version, so `releases/latest/download/dtstudio_amd64.deb` always points at the current build. |
| `bindings.db` | The device-tree bindings database, built from the kernel YAML bindings. |
| `manifest.json` | Version, URL, `sha256` and size of `bindings.db`. DTstudio reads it to fetch and verify the database. |

## Installing the beta

```bash
wget https://github.com/serg4life/dtstudio-releases/releases/latest/download/dtstudio_amd64.deb
sudo apt install ./dtstudio_amd64.deb
```

The bindings database is downloaded by the application on first run; there is
no need to fetch it by hand.
