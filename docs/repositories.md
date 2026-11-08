# Repository guide

This is the navigation map for CraysCircle. It separates implementation source, website snapshots, mobile projects, documentation and upstream forks. These roles are based on the inspected repository trees and existing migration source evidence; a role is not a functional acceptance result.

## Platform services

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-platform](https://github.com/CraysCircle/crays-platform) | Shared CRAYS service source. Qlo gateway and Clubs Commerce BFF, original tests and notices, plus reviewed gateway and Delivery operations source. | Current gateway source capture; license closure and broader platform import remain in progress. |

Preserved platform components:

- [Qlo gateway](https://github.com/CraysCircle/crays-platform/tree/main/services/qlo-gateway), with original tests.
- [Clubs Commerce BFF](https://github.com/CraysCircle/crays-platform/tree/main/services/clubs-commerce-bff), with original build/test source and fourteen exact dependency notices.
- [Operations](https://github.com/CraysCircle/crays-platform/tree/main/operations), with separate Qlo and Delivery source records and execution boundaries.

## Websites and web applications

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-club](https://github.com/CraysCircle/crays-club) | Retained original Club static website source. | A newer AWS Club composition must be mapped separately. |
| [crays-coffee](https://github.com/CraysCircle/crays-coffee) | Qualified Coffee Next.js capture and original public source files. | Exact eight-file source state preserved; remaining media/dependency/license and earlier-history closure stays explicit. |
| [crays-org](https://github.com/CraysCircle/crays-org) | Association website source, static assets, server wrapper and scripts. | Original repository plus later AWS supplements must be distinguished. |
| [crays-web-codex](https://github.com/CraysCircle/crays-web-codex) | Primal-derived CRAYS Nostr website source. | Retains its upstream fork relationship and original MIT license. |
| [crays-franchise](https://github.com/CraysCircle/crays-franchise) | Franchise Investment OS interface using React, TanStack Start and Vite. | Retained original source; not assumed identical to the current Club AWS build. |
| [crays-fund](https://github.com/CraysCircle/crays-fund) | Fund static website source snapshot. | The exact AWS server/build-source relationship is being reconciled. |
| [crays-world](https://github.com/CraysCircle/crays-world) | World website pages, assets and retained editable source. | The exact latest AWS composition is being reconciled. |
| [crays-gym](https://github.com/CraysCircle/crays-gym) | Retained Gym and shared-platform source tree with development history. | Contains multiple areas; current AWS releases and uncommitted derivatives require separate source records. |

## Mobile applications

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-ios](https://github.com/CraysCircle/crays-ios) | Native CRAYS iOS application source: SwiftUI, Nostr and Core integration. | Kept separate from the Circle iOS project. |
| [CraysCircleApp-Android](https://github.com/CraysCircle/CraysCircleApp-Android) | CRAYS Circle Android application project. | Original project and license retained. |
| [crayscircle-ios](https://github.com/CraysCircle/crayscircle-ios) | CRAYS Circle iOS WifiAware project. | A separate source project from crays-ios. |
| [crays-ble](https://github.com/CraysCircle/crays-ble) | Separate Android and iOS source trees for the BLE project. | Component-level documentation and license mapping are being completed. |

## Web interfaces

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-circle-admin-plus-vendor](https://github.com/CraysCircle/crays-circle-admin-plus-vendor) | Separate administrator and vendor dashboard source trees. | Do not confuse these interfaces with a verified current AWS service release. |

## Project and protocol documentation

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-circle-app](https://github.com/CraysCircle/crays-circle-app) | Circle project overview, contribution guide and original license. | The inspected root contains project documentation rather than the application implementation. |
| [dnc-protocol](https://github.com/CraysCircle/dnc-protocol) | DNC protocol project overview, contribution guide and original license. | The inspected root contains documentation. |

## Upstream open-source forks

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [calendar](https://github.com/CraysCircle/calendar) | Fork of nextcloud/calendar. | Original upstream relationship and Git history retained. |
| [crm](https://github.com/CraysCircle/crm) | Fork of frappe/crm. | Original upstream relationship and Git history retained. |
| [openproject](https://github.com/CraysCircle/openproject) | Fork of opf/openproject. | Original upstream relationship and Git history retained. |
| [twenty](https://github.com/CraysCircle/twenty) | Fork of twentyhq/twenty. | Original upstream relationship retained; component-specific license terms must be respected. |
| [primal-web-app](https://github.com/CraysCircle/primal-web-app) | Fork of Chandan-codedidea/primal-web-app. | Separate upstream reference; not a substitute for the exact CRAYS deployed source. |

## How to find an exact AWS version

1. Identify the service or website and its recorded artifact identity.
2. Open the corresponding source/release record. Distinguish a Git commit from a Docker image ID, registry manifest digest, framework build ID and configuration revision.
3. Follow the exact commit and any required upstream/base-component references. Include later source changes and hosting wrappers; an old HEAD or upstream link alone is insufficient.
4. Read the project's original license texts, NOTICE files, modification notes and source-availability record.

Source and documentation imports are continuing until the AWS migration owner reports completion and the final GitHub reconciliation passes. The [status page](source-and-license-status.md) records established milestones and remaining gaps.

See the [repository structure and update rules](https://github.com/CraysCircle/.github/blob/main/docs/repository-structure.md) for where current sources, shared components, operations and historical versions belong.
