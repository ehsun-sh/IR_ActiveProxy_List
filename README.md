# iran_proxy data

This branch is rewritten by the `Update proxy list` workflow on every run. Do not
commit to it by hand.

| File | What it is |
|---|---|
| `proxies.json` | Working proxies with an Iranian exit IP, best score first |
| `domains.json` | Iranian sites outside `.ir` that clients send through the proxy |
| `*.sig` | ed25519 signatures of the files above (when a signing key is set) |
| `stats.jsonl` | One line per run: how many candidates were found, reachable and alive |
| `state.json` | Per-proxy history the updater uses to compute uptime |

Proxies come from public lists; nothing here scans IP ranges. Free proxies are run
by unknown people: use them only for HTTPS sites and never for passwords you care about.

Attribution: IP geolocation by [DB-IP](https://db-ip.com) (CC BY 4.0), via
[ip-location-db](https://github.com/sapics/ip-location-db). Iranian domains from
[iran-hosted-domains](https://github.com/bootmortis/iran-hosted-domains).
