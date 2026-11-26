# SiteWatcher

SiteWatcher keeps a history of website uptime and response times and warns you
before a TLS certificate or domain registration expires.

## Start

From this directory, run:

```sh
docker compose run --rm setup
docker compose up -d
```

The first command asks for a username and password. Then open
http://127.0.0.1:8080/ and sign in. Set `SITEWATCHER_PORT` in `.env` if
port 8080 is already in use.

The web service and worker use the same image and share the SQLite database
and settings in the `sitewatcher-data` volume. Keep that volume when upgrading.
The port listens on loopback by default. For remote access, follow the upstream
reverse-proxy setup.

- [Source and setup](https://github.com/NikKurkov/sitewatcher)
- [Configuration guide](https://github.com/NikKurkov/sitewatcher/blob/main/docs/usage.en.md)
- [Public demo](https://monitoring.kurkov.dev/demo)
