# CRAYS

### Build the software behind real-world communities.

CRAYS is building software for members, guests and venue operators across clubs, hospitality and community projects. The goal is to connect people and places with the tools behind member access, personal experiences, venue services and business operations.

For developers, that means web and native applications, Nostr-related social work, account boundaries and adapters connecting established open-source systems. Personal, Member and Work give these different responsibilities a shared context.

We build the CRAYS-specific experience and integration code while keeping the underlying projects, their authors and their licenses identifiable. This organization is where developers can explore that work, understand the system and contribute.

**[Explore the platform](https://github.com/CraysCircle/crays-platform) · [How it fits together](https://github.com/CraysCircle/crays-platform/blob/main/docs/architecture.md) · [Contribute](https://github.com/CraysCircle/crays-platform/blob/main/CONTRIBUTING.md)**

## Explore CRAYS

| Area | What we are building | Where to begin |
| --- | --- | --- |
| **Platform** | Personal and Member experiences, Work services and the connections between accounts, documents, commerce and operations. | [crays-platform](https://github.com/CraysCircle/crays-platform) |
| **Websites** | Distinct CRAYS websites for communities, hospitality, commerce and the wider ecosystem. Each has its own source and development history. | [Website and project map](https://github.com/CraysCircle/.github/blob/main/docs/repository-structure.md#eleven-website-compositions) |
| **Mobile and connectivity** | Native iOS and Android projects, Nostr integration, BLE and nearby-connectivity work. These projects have different purposes and stages of development. | [Mobile source map](https://github.com/CraysCircle/.github/blob/main/docs/native-source-map.md) |

## Inside the platform

The [platform service hub](https://github.com/CraysCircle/crays-platform/blob/main/docs/services/README.md) explains the role of each system and points to the actual CRAYS implementation:

- **[Frappe / ERPNext](https://github.com/CraysCircle/crays-platform/blob/main/docs/services/frappe.md):** finance and company-scoped business workflows, including the CRAYS commerce-to-ERP adapters.
- **[Nextcloud](https://github.com/CraysCircle/crays-platform/blob/main/docs/services/nextcloud.md):** files, member documents and collaboration, with CRAYS access and reconciliation adapters.
- **[Plane](https://github.com/CraysCircle/crays-platform/blob/main/docs/services/plane.md):** the canonical project and work-item area within Work, with delivery contracts and signed-webhook handling.
- **[Qlo](https://github.com/CraysCircle/crays-platform/blob/main/docs/services/qlo.md):** hospitality requests and accommodation operations, connected through the CRAYS gateway and Work integration.
- **Commerce, identity and the wider ecosystem:** Vendure, account boundaries, Personal/Chuck, Gym, Nostr and delivery tooling, each documented in the same hub.

Personal, Member and Work are related parts of the ecosystem with separate responsibilities. An integration's presence in the source tree does not mean every user journey is already complete; the component guides explain what is implemented and what is still being connected.

## Build with us

We welcome developers who want to improve useful connections between open systems. Current contribution directions include account-boundary tests, document access, ERP event mapping, project webhooks, hospitality adapters, accessibility and clearer developer documentation.

**A small first contribution:** follow the [Qlo projection-test walkthrough](https://github.com/CraysCircle/crays-platform/blob/main/docs/services/qlo.md#first-local-check-the-two-projection-tests), then add a synthetic invalid-input case using the [contributor exercise](https://github.com/CraysCircle/crays-platform/blob/main/CONTRIBUTING.md#a-small-first-test). These two local projection checks need Node.js and the source checkout, without provider credentials or running a live service.

Start with [the contributor guide](https://github.com/CraysCircle/crays-platform/blob/main/CONTRIBUTING.md). It explains how to choose a component, find its real setup instructions, propose a focused change and show that it works. You can also use [platform issues](https://github.com/CraysCircle/crays-platform/issues) to discuss a concrete problem before writing code.

## Find the details

[All repositories](https://github.com/CraysCircle/.github/blob/main/docs/repositories.md) · [Source and license status](https://github.com/CraysCircle/.github/blob/main/docs/source-and-license-status.md) · [Historical projects](https://github.com/CraysCircle/.github/blob/main/docs/legacy-projects.md)

Source publication and integration work are continuing. Original project licenses and notices apply to their respective components; each component's technical records state its source, version and recovery coverage.
