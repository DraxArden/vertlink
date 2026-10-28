# VERTLINK

A network analyzer that runs in your browser, with nothing to install. It also works as an installable app on Android and iPhone.

**Open it:** the GitHub Pages address of this repository, for example `https://<your-username>.github.io/vertlink/`.

## What it does

- **Overview:** real-time latency to Cloudflare and Google, jitter, packet loss, connection quality, speed test with bufferbloat, public IP, provider and NAT type.
- **Route and DNS:** DNS response times (Cloudflare and Google) and lookups for any record. On a computer, also a visual traceroute.
- **History and alerts:** one measurement per minute kept for 7 days, "when it gets worse" map, outages, speed over time against your plan, alerts.
- **Services:** continuous checks of websites and devices, with uptime history.
- **Capture:** reader for Wireshark/tcpdump files (.pcap, .pcapng), analyzed locally.
- **On a computer:** also local network devices, Wi‑Fi analysis, system connections and the optional local agent ([download](download/VERTLINK.zip)).

Interface in English and Italian, light and dark themes.

## Install on a phone

- **Android (Chrome):** open the page and tap **Install app**, or menu ⋮ › **Install app**.
- **iPhone (Safari):** tap **Share** › **Add to Home Screen**.

## Online version vs. the downloaded file

Browsers don't let an `https://` page contact `http://` devices on your local network. For the device scan and router latency, open `vertlink.html` from the downloaded package on your computer, or connect the local agent.

Phones don't allow programs like the agent and don't expose Wi‑Fi details to the browser, so the phone version shows the tabs that work there.

## Privacy

Everything you paste and all history stays in your browser. To measure, the page contacts Cloudflare, Google, ipify and ipwho.is (public IP and location), and macvendors.com (device vendor from MAC).

## Responsible use

Use network scanning and captures only on your own network, or with permission from whoever manages it.

## Verify the downloads

Download the package only from this repository or from the VERTLINK page. These are the SHA-256 fingerprints of the current files:

| File | SHA-256 |
|---|---|
| `VERTLINK.zip` | `d0878892cb9fe1cd0031fbac259e2f661e7fb95f9758f694739c2497017485a4` |
| `vertlink-agent-linux-amd64` | `0bb7e333098af072e75bd0b6e07fcbefe72540047dee061831b2a548c60fbc70` |
| `vertlink-agent-linux-arm64` | `115faaa386e736fecf74c3f01eac697b55bcd92839efba3933b107c63a50e4c1` |
| `vertlink-agent-mac-apple-silicon` | `bdc8861a8be2c5f7349639f44ba1ab9bb085b5182bf11db9605727efa2dbefda` |
| `vertlink-agent-mac-intel` | `5361508370a7cc67329fbf9f79ff3c6b315fe2566d96a52979726e7971fc5110` |
| `vertlink-agent-windows-amd64.exe` | `b800bc2da417f3dd50c33cd22eafcf82a865192f93b9b9720ed2076627df3c0d` |
| `vertlink-agent-windows-arm64.exe` | `fb08a8df5a2cf918be191aeb7987003ac01b7c893eedd1ddc2f876acdfa14d51` |

How to check:

- **Windows (PowerShell):** `Get-FileHash .\agent\vertlink-agent-windows-amd64.exe`
- **macOS:** `shasum -a 256 agent/vertlink-agent-mac-apple-silicon`
- **Linux:** `cd agent && sha256sum -c ../SHA256SUMS.txt`

The agents are not code-signed, so Windows and macOS show a warning on first launch. The source code is in the package, under `source/`.

## License

[MIT](LICENSE). VERTLINK is provided as is, without warranty of any kind.

---

# VERTLINK (italiano)

Analizzatore di rete che funziona nel browser, senza installare nulla, e si installa come app su Android e iPhone.

- **Android (Chrome):** apri la pagina e tocca **Installa app**, oppure menu ⋮ › **Installa app**.
- **iPhone (Safari):** tocca **Condividi** › **Aggiungi alla schermata Home**.

Per la scansione della rete locale e la latenza del router usa il file `vertlink.html` del [pacchetto da scaricare](download/VERTLINK.zip) oppure l'agente locale. Tutti i dati restano nel tuo browser.

Usa la scansione della rete e le catture solo sulla tua rete, o con il permesso di chi la gestisce. Scarica il pacchetto solo da qui e verifica le impronte SHA-256 indicate sopra. Licenza MIT: VERTLINK è fornito così com'è, senza garanzie.
