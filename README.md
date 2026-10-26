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

---

# VERTLINK (italiano)

Analizzatore di rete che funziona nel browser, senza installare nulla, e si installa come app su Android e iPhone.

- **Android (Chrome):** apri la pagina e tocca **Installa app**, oppure menu ⋮ › **Installa app**.
- **iPhone (Safari):** tocca **Condividi** › **Aggiungi alla schermata Home**.

Per la scansione della rete locale e la latenza del router usa il file `vertlink.html` del [pacchetto da scaricare](download/VERTLINK.zip) oppure l'agente locale. Tutti i dati restano nel tuo browser.
