<!-- FreeSDN org profile -->

<p align="center">
  <img src="./assets/freesdn-logo-black-512.png" alt="FreeSDN" height="120">
</p>

<h3 align="center">Manage network gear across brands - Open source & Self-hosted</h3>

<p align="center">
  See all your devices in one place, check health, and run safe fixes across UniFi, Omada, pfSense/OPNsense, ONVIF cameras, and Grandstream GDMS.
</p>


## What is FreeSDN?

FreeSDN is an open platform that sits above your existing controllers and devices to provide:

- **Inventory & health** across sites/vendors
- **Cross-vendor actions** (PoE cycle, SSID toggle, VLAN assign, camera snapshot, firewall alias update, VoIP reprovision)
- **Desired State** via a **Device Capability Model (DCM)**
- **Northbound APIs** (REST/gRPC) and an **Adapter** plugin runtime (gRPC)
- **RBAC, audit, webhooks, backups**

> Canonical spec lives in the main repos: `docs/spec/agent-master-spec.md`.

## Quick start (alpha)

```bash
# docker compose (single-node demo)
git clone https://github.com/freesdn/core
cd core/deployments/compose
docker compose up -d
```

Then open the UI, enroll a controller (UniFi, Omada, etc.), sync devices, and try actions.

## Roadmap (high level)

- **M0 (Public Alpha):** inventory + safe actions across UniFi/Omada/OPNsense/pfSense/ONVIF/GDMS; RBAC, audit, webhooks; Docker Compose.
- **M1:** approvals/policy engine, topology view, alert correlation, NetBox sync.
- **M2:** MSP multi-tenancy, TR-369 gateway, pfSense CE support, UCM provisioning.
- **M3:** OpenConfig/gNMI drivers, ZTP for supported devices.

## Contributing

- Issues & RFCs → `docs/rfc/*` (main repos)
- Conventional Commits + DCO signoff
- Signed releases with SBOMs
- See `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and `SECURITY.md`

## License & Governance

- **Core:** AGPL-3.0 • **SDKs/examples:** Apache-2.0  
- FreeSDN Foundation • Technical Steering Committee (TSC)



---

## Trademark notice

All product names, logos, and brands are property of their respective owners.  
FreeSDN is not affiliated with, endorsed by, or sponsored by any referenced vendor.
