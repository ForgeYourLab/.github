**ForgeYourLab** is a journey to build a <mark>privacy-first</mark>, <mark>zero-trust</mark>
personal homelab, with <mark>least-privilege</mark> and <mark>default-deny</mark> principles for
security through multiple defensive layers. The focus is privacy, security, and resilience of all
services (and infrastructure) in this homelab.

Just as we expect physical security and privacy around the clock, why not aim for the same in the
digital world? Digital security and privacy should be foundational rights, not afterthoughts, and
not just for enterprise solutions.

## The Homelab Arc (Infra → Resilience)

<!-- Own your infra → Control identity → Enforce least privilege → Protect data → Prove resilience. -->

### Own your infra

- Run and control your own router & DHCP server.
- Run Pi-hole/AdGuard + Unbound for DNS (with DoH).
- Use an authoritative DNS server for internal services.
- Enforce VLAN segmentation, strict firewall, and access point policies.
- Maintain secure provision/deployment pipelines. {{< /collapse >}}

###  Control identity

- Run your own Certificate Authority.
- Use root & intermediate CAs as trust anchors.
- Automate certificate issuance/renewal for all internal services (DNS-ACME).
- Enforce mTLS between clients, reverse proxy, and services.
- Harden clients (browsers, etc.) to reject untrusted services. {{< /collapse >}}

### Enforce least privilege

- Default-deny firewall with explicit egress/ingress policies.
- Provision hardened servers with minimal packages, SSH hardening, fail2ban, strict sudo/user
  policies.
- Secure containers using seccomp & AppArmor profiles, segmented networks, restricted Docker
  defaults. {{< /collapse >}}

### Protect data

- Use encrypted OS and service storage (with LUKS).
- Encrypted RAID NAS for regular backups.
- Automate offline/offsite backup copies (encrypted, immutable and versioned). {{< /collapse >}}

### Prove resilience

- Aggregate centralized logging, metrics, and alerting.
- Run periodic storm and restore drills. {{< /collapse >}}

<br />

<i><b><mark>Privacy and security are not optional; they are a non-negotiable operational
baseline.</mark></b></i>

> 🥂 to a secure and clean digital life!
