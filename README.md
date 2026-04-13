# Hamish

**SOC Analyst · Security Researcher · Barcelona**

I work in cybersecurity with a focus on threat detection, secure software development, and applied security research. Currently a SOC Analyst at N26 (Berlin); previously a Cybersecurity Engineer at Texaport (Edinburgh).

My research interests sit at the intersection of mobile security, overlay networking, and cryptographic protocol analysis.

---

## Projects

### [Ember 5.0](https://github.com/TheFruggg/Ember-5.0)
Serverless, peer-to-peer, end-to-end encrypted Android messaging application.

- No central server. Identity is a P-256 keypair generated at first launch — no phone number, no account, no directory.
- Double Ratchet protocol (Signal-style) over direct TCP on a Yggdrasil IPv6 mesh network.
- X3DH-lite key agreement: both peers derive the same initial root key from persisted identity keys via HKDF(ECDH(...), "ember-dr-init-v1"), requiring no online coordination.
- AES-256-GCM encryption. Ciphertext stored locally via SQLCipher + Room; plaintext is never persisted.
- QR code contact pairing — encodes display name, Yggdrasil address, port, and public key.
- Configurable TTL ephemeral messages (5m–1d) with WorkManager-scheduled cleanup.
- Biometric lock, FLAG_SECURE screen protection, encrypted key storage via Android Keystore.
- Built with Kotlin, Jetpack Compose, Material 3, Hilt, and a custom "Living Flame" dark UI.

`Kotlin` `Android` `Yggdrasil` `Double Ratchet` `E2EE` `Jetpack Compose`

---

### [ARES 2.0](https://github.com/TheFruggg/Ember-5.0) *(private — link pending)*
Advanced Reconnaissance & Event System — a self-hosted, real-time geopolitical and cybersecurity threat intelligence dashboard.

- Ingests and normalises open-source data streams: 20+ RSS/Atom feeds, ADS-B military flight transponders (OpenSky + adsb.fi), AIS vessel tracking, GDELT geopolitical events, and NVD CVE feeds.
- Per-country threat scoring (0–100) recomputed every 20 minutes, weighted by event category and recency.
- Live tactical map: country choropleth, military aircraft markers (zoom-culled, ICAO type decoded), vessel positions.
- Real-time WebSocket push via Celery → Redis pub/sub → browser.
- 6-container stack: FastAPI, Next.js 14, Celery worker + beat, TimescaleDB/Postgres, Redis.
- Flight data merges two independent ADS-B feeds with a three-tier filtering strategy to surface military and government aircraft alongside a deterministic civilian sample.

`FastAPI` `Next.js` `Celery` `Redis` `TimescaleDB` `Leaflet` `Docker`

---

### [VuzixApp](https://github.com/TheFruggg/VuzixApp)
End-to-end encrypted messaging application built for the Vuzix Blade 2 smart glasses platform.

`Kotlin` `Android` `E2EE`

---

## Skills

`SOC Operations` `Threat Detection & Triage` `Android / Kotlin` `Python`  
`Network Forensics` `Penetration Testing` `Zero Trust Architecture`  
`Linux` `Wireshark` `LaTeX` `Docker / Podman`

---

## Education

1st Class Honors BEng Cyber Security & Digital Forensics, Edinburgh Napier University  
Dissertation: *Zero Trust Architecture in Financial Institutions* — designed, implemented, and attack-tested both a traditional perimeter network and a Zero Trust model across segmented VMware environments.

---

## Contact

[LinkedIn](https://www.linkedin.com/in/hamish-a-43bb4693/) · [GitHub](https://github.com/TheFruggg)  
*Personal site coming soon*
