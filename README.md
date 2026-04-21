<div align="center">

# Frug

**SOC Analyst · Security Researcher**

I work in cybersecurity with a focus on threat detection, secure software development, and applied security research.
Experience in Cyber SOC & Cybersecurity Engineering.

My research interests sit at the intersection of mobile security, overlay networking, and cryptographic protocol analysis.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hamish-a-43bb4693/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/TheFruggg)

</div>

---

## Projects

### [Ember 5.0](https://github.com/TheFruggg/Ember-5.0)
Serverless, peer-to-peer, end-to-end encrypted Android messaging application.

- No central server. Identity is a P-256 keypair generated at first launch — no phone number, no account, no directory.
- Double Ratchet protocol (Signal-style) over direct TCP on a Yggdrasil IPv6 mesh network.
- X3DH-lite key agreement: both peers derive the same initial root key from persisted identity keys via `HKDF(ECDH(...), "ember-dr-init-v1")`, requiring no online coordination.
- AES-256-GCM encryption. Ciphertext stored locally via SQLCipher + Room; plaintext is never persisted.
- QR code contact pairing — encodes display name, Yggdrasil address, port, and public key.
- Configurable TTL ephemeral messages (5m–1d) with WorkManager-scheduled cleanup.
- Biometric lock, `FLAG_SECURE` screen protection, encrypted key storage via Android Keystore.
- Built with Kotlin, Jetpack Compose, Material 3, Hilt, and a custom "Living Flame" dark UI.

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat&logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat&logo=jetpackcompose&logoColor=white)
![SQLCipher](https://img.shields.io/badge/SQLCipher-003B57?style=flat&logo=sqlite&logoColor=white)

---

### [ARES 2.0]([private — link pending)*](https://github.com/TheFruggg/ARES_2.0)
Advanced Reconnaissance & Event System — a self-hosted, real-time geopolitical and cybersecurity threat intelligence dashboard.

- Ingests and normalises open-source data streams: 20+ RSS/Atom feeds, ADS-B military flight transponders (OpenSky + adsb.fi), AIS vessel tracking, GDELT geopolitical events, and NVD CVE feeds.
- Per-country threat scoring (0–100) recomputed every 20 minutes, weighted by event category and recency.
- Live tactical map: country choropleth, military aircraft markers (zoom-culled, ICAO type decoded), vessel positions.
- Real-time WebSocket push via Celery → Redis pub/sub → browser.
- 6-container stack: FastAPI, Next.js 14, Celery worker + beat, TimescaleDB/Postgres, Redis.
- Flight data merges two independent ADS-B feeds with a three-tier filtering strategy to surface military and government aircraft alongside a deterministic civilian sample.

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat&logo=celery&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat&logo=redis&logoColor=white)
![Postgres](https://img.shields.io/badge/TimescaleDB-FDB515?style=flat&logo=timescale&logoColor=white)
![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=flat&logo=leaflet&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

---

### [VuzixApp](https://github.com/TheFruggg/VuzixApp)
End-to-end encrypted messaging application built for the Vuzix Blade 2 smart glasses platform.

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat&logo=android&logoColor=white)

---

## Skills

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat&logo=wireshark&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat&logo=latex&logoColor=white)

`SOC Operations` `Threat Detection & Triage` `Network Forensics` `Penetration Testing` `Zero Trust Architecture`

---

## Education

**1st Class Honours BEng Cyber Security & Digital Forensics** — Edinburgh Napier University

Dissertation: *Zero Trust Architecture in Financial Institutions* — designed, implemented, and attack-tested both a traditional perimeter network and a Zero Trust model across segmented VMware environments.

---

<div align="center"><i>Personal site coming soon</i></div>
