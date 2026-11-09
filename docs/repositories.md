# Repository guide

CRAYS develops software connecting members, guests and venue operators: personal experiences, membership, commerce and business operations. This guide helps you choose the repository for the experience or integration you want to improve.

**[Understand the architecture](https://github.com/CraysWorld/crays-platform/blob/main/docs/architecture.md) · [Explore service integrations](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/README.md) · [Try a first local test](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/qlo.md#first-local-check-the-two-projection-tests) · [Contribute](https://github.com/CraysWorld/crays-platform/blob/main/CONTRIBUTING.md)**

Project repositories, shared implementations and retained upstream forks have different roles. Their detailed source/version records remain linked below.

## Shared application and platform services

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-platform](https://github.com/CraysWorld/crays-platform) | Shared Next.js application under apps/web, Personal React/Vite application under apps/personal, Qlo gateway and Clubs Commerce BFF under services, hosting wrappers, and reviewed migration operations. | Exact application baseline/prepared-state tags and separate service/version records. Later source overlays, recovery inputs and full license closure remain in progress. |

Preserved platform components:

- [Shared Next.js application](https://github.com/CraysWorld/crays-platform/tree/main/apps/web), containing Club, Member/SaaS and investment routes, original integration source, dependency notices and recovery instructions.

- [Personal web application](https://github.com/CraysWorld/crays-platform/tree/main/apps/personal), with original 1,486-file and 13-overlay/1,489-file compositions, 1,435 current text inputs, ten preimages, exact dependency notices and source restoration. Eleven original generated image inputs are now preserved. The [54-entry image source map](https://github.com/CraysWorld/crays-platform/tree/main/apps/personal/provenance/images) names the 43 remaining image input paths and their source/privacy/rights review state; the protected owner input remains separate.
- [Personal build operations](https://github.com/CraysWorld/crays-platform/tree/main/operations/personal-build), retaining three original controller revisions, a lease adapter, artifact inspection and adoption-plan programs, plus the exact [AWS Build02 configuration bodies](https://github.com/CraysWorld/crays-platform/tree/main/apps/personal/aws-build02).
- [Qlo gateway](https://github.com/CraysWorld/crays-platform/tree/main/services/qlo-gateway), with original tests.
- [Clubs Commerce BFF](https://github.com/CraysWorld/crays-platform/tree/main/services/clubs-commerce-bff), with original build/test source and fourteen exact dependency notices.
- [Club/Member browser module](https://github.com/CraysWorld/crays-platform/tree/main/modules/club-member), with exact original/origin35 source views, build and dependency records, original notices and protected source restoration. This is the separately built Common-shell client; the Next application remains under apps/web.
- [Member source25 compositions](https://github.com/CraysWorld/crays-platform/tree/main/apps/web/compositions/member-source25), preserving the complete original and AWS input views with a source-only reconstruction tool and protected test-input templates. The [version evidence](https://github.com/CraysWorld/crays-platform/tree/main/apps/web/provenance/member-source25) links their recorded build, original lock and existing notice catalog.
- [Shared web operational programs](https://github.com/CraysWorld/crays-platform/tree/main/apps/web/scripts), with original baseline/worktree records, 90 referenced programs, two imported modules and explicit four-file provenance limits.
- [Club Next listener and private HTTPS](https://github.com/CraysWorld/crays-platform/tree/main/services/club-next-runtime), with exact listener/bootstrap/origin/TLS fragments and [original controller revisions, patches and acceptance-program source](https://github.com/CraysWorld/crays-platform/tree/main/operations/club-next-runtime). Eleven already-public bodies are referenced by immutable commit; later origin35 completion/adoption source stays in its existing area.
- [Work/Qlo runtime](https://github.com/CraysWorld/crays-platform/tree/main/services/work-qlo-runtime), with its original bootstrap and four local modules, separately from the underlying application and its still-open runtime/asset source relationships.
- [Qlo/Work operating-source revisions](https://github.com/CraysWorld/crays-platform/tree/main/operations/qlo-work-family), with historical/current-family/start-only revisions, original patches and binding-check source; the existing storage guard is linked without duplication.
- [Operations](https://github.com/CraysWorld/crays-platform/tree/main/operations), with separate Qlo and Delivery source records and execution boundaries.

## Websites and web applications

The [eleven-website map](repository-structure.md#eleven-website-compositions) covers **Club, Gym, Coffee, Shop, Pro, Net, Org, Fund, World, Award and Fun**. Website compositions and repository counts are different: some experiences use shared platform code, while Award and Fun still have unresolved source destinations. Use that map to choose the website, then follow the repository and component links below.

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-club](https://github.com/CraysWorld/crays-club) | Retained original Club static website source. | The selected later shared Next.js source is preserved in [crays-platform/apps/web](https://github.com/CraysWorld/crays-platform/tree/main/apps/web); current deployment and later overlays require their exact version records. |
| [crays-coffee](https://github.com/CraysWorld/crays-coffee) | Qualified Coffee Next.js capture and original public source files. | Exact eight-file source state preserved; remaining media/dependency/license and earlier-history closure stays explicit. |
| [crays-shop](https://github.com/CraysWorld/crays-shop) | Qualified storefront, original public source and Store/worker references. | Three-commit capture, 466 selected source/build/reference files and original font notices verified; remaining media/dependency/license/earlier-history scope stays explicit. |
| [crays-pro](https://github.com/CraysWorld/crays-pro) | Qualified public Pro website; crays-franchise component paths retain their original names. | Two-commit capture and 89 selected sources verified; Franchise Manager and Targomo runtime acceptance are separate. |
| [crays-org](https://github.com/CraysWorld/crays-org) | Association website: multilingual CRAYS pages, Nostr research and ecosystem directories, account entry and event/moderation APIs. | [Browse all page routes by topic](https://github.com/CraysWorld/crays-org/blob/org-page-reader-index-20261109/source-archives/org-web/org05-20261107/PAGE_INDEX.md): 1,838 route/page JSON files alongside 38 source/technical inputs; every new public file was anonymously hash-verified. The exact 25-file own-code grant remains AGPL-3.0-only; content and assets retain separate terms. Media/font custody and rights, complete dependencies and runtime recovery remain open. |
| [crays-web-codex](https://github.com/CraysWorld/crays-web-codex) | Primal-derived CRAYS Nostr website source. | Retains its upstream fork relationship and original MIT license. |
| [crays-franchise](https://github.com/CraysWorld/crays-franchise) | Franchise Investment OS interface using React, TanStack Start and Vite. | Retained original source; not assumed identical to the current Club AWS build. |
| [crays-fund](https://github.com/CraysWorld/crays-fund) | Fund static website source snapshot. | The exact AWS server/build-source relationship is being reconciled. |
| [crays-world](https://github.com/CraysWorld/crays-world) | World website pages, assets and retained editable source. | The exact latest AWS composition is being reconciled. |
| [crays-gym](https://github.com/CraysWorld/crays-gym) | Retained Gym and shared-platform source tree with development history. | Contains multiple areas; current AWS releases and uncommitted derivatives require separate source records. |

## Mobile applications

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-ios](https://github.com/CraysWorld/crays-ios) | Native CRAYS iOS app, Core bridge, tests, original vendor notices and owner handoffs. | [Current branch, immutable source tag and Core boundaries](native-source-map.md). The current original source checkpoint d53dfa5 is preserved; public-access/privacy/rights and native product acceptance remain open. |
| [CraysCircleApp-Android](https://github.com/CraysWorld/CraysCircleApp-Android) | CRAYS Circle Android application project. | Original project and license retained. |
| [crayscircle-ios](https://github.com/CraysWorld/crayscircle-ios) | CRAYS Circle iOS WifiAware project. | A separate source project from crays-ios. |
| [crays-ble](https://github.com/CraysWorld/crays-ble) | Separate Android and iOS source trees for the BLE project. | Component-level documentation and license mapping are being completed. |

## Web interfaces

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-circle-admin-plus-vendor](https://github.com/CraysWorld/crays-circle-admin-plus-vendor) | Separate administrator and vendor dashboard source trees. | Do not confuse these interfaces with a verified current AWS service release. |

## Project and protocol documentation

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [crays-circle-app](https://github.com/CraysWorld/crays-circle-app) | Circle project overview, contribution guide and original license. | The inspected root contains project documentation rather than the application implementation. |
| [dnc-protocol](https://github.com/CraysWorld/dnc-protocol) | DNC protocol project overview, contribution guide and original license. | The inspected root contains documentation. |

## Upstream open-source forks

| Repository | Source role | Version guidance |
| --- | --- | --- |
| [calendar](https://github.com/CraysWorld/calendar) | Fork of nextcloud/calendar. | Original upstream relationship and Git history retained. |
| [crm](https://github.com/CraysWorld/crm) | Fork of frappe/crm. | Original upstream relationship and Git history retained. |
| [openproject](https://github.com/CraysWorld/openproject) | Historical fork, no longer used in the current CRAYS stack; retained with original history and license. See [legacy projects](legacy-projects.md). | Original upstream relationship and Git history retained. |
| [twenty](https://github.com/CraysWorld/twenty) | Historical fork, no longer used in the current CRAYS stack; retained with original history and license. See [legacy projects](legacy-projects.md). | Original upstream relationship retained; component-specific license terms must be respected. |
| [primal-web-app](https://github.com/CraysWorld/primal-web-app) | Fork of Chandan-codedidea/primal-web-app. | Separate upstream reference; not a substitute for the exact CRAYS deployed source. |

## How to find an exact AWS version

1. Identify the service or website and its recorded artifact identity.
2. Open the corresponding source/release record. Distinguish a Git commit from a Docker image ID, registry manifest digest, framework build ID and configuration revision.
3. Follow the exact commit and any required upstream/base-component references. Include later source changes and hosting wrappers; an old HEAD or upstream link alone is insufficient.
4. Read the project's original license texts, NOTICE files, modification notes and source-availability record.

Source and documentation imports are continuing until the AWS migration owner reports completion and the final GitHub reconciliation passes. The [status page](source-and-license-status.md) records established milestones and remaining gaps.

See the [repository structure and update rules](https://github.com/CraysWorld/.github/blob/main/docs/repository-structure.md) for where current sources, shared components, operations and historical versions belong.
