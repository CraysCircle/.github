# Source, license and recovery status

**Consolidation is in progress. GitHub does not yet contain the complete current CRAYS source and recovery set.** Public access, source preservation, reproducible builds and license clearance are checked separately.

Start with the [repository guide](repositories.md) and [structure rules](repository-structure.md). Detailed commit links and byte-verification records are in [verification records](verification-records.md).

## Organization and access

The organization currently contains **23 project repositories and one navigation repository**. The original twenty projects were retained; Coffee, Shop and Pro were added only after establishing their independent source roles and the absence of matching repositories.

All nine repositories originally owned by ThorbenAroundTheWorld were transferred natively, preserving their Git history and repository relationships. The authenticated personal-owner query returned zero owned repositories after those transfers.

As checked on 8 November 2026, **19 repositories are public and five remain private**: crays-fund, crays-gym, crays-franchise, crays-world and crays-ios. Their remaining confidentiality and rights checks must finish before public access is treated as complete. All repository descriptions are present.

## What is preserved in GitHub

“Preserved” below applies to the stated capture, not to every later source version, dependency, media asset or license obligation.

| Component | Verified source coverage | Remaining limits |
| --- | --- | --- |
| Shared Next.js application | 2,045 original selected files in [crays-platform/apps/web](https://github.com/CraysCircle/crays-platform/tree/main/apps/web), with exact baseline and prepared-state tags, five original integration files and version-bound dependency records | Current AWS overlays, 94 referenced operational helper paths, a qualified application lockfile, media, complete history and full rights/recovery closure remain open. |
| Qlo gateway | Original service/build files, original README and four test files in [crays-platform](https://github.com/CraysCircle/crays-platform/tree/main/services/qlo-gateway) | Runtime/dependency notices and full rights closure remain open; captured tests were not freshly executed. |
| Clubs Commerce BFF | Nine original files and fourteen original dependency notices in [crays-platform](https://github.com/CraysCircle/crays-platform/tree/main/services/clubs-commerce-bff) | Full application/image licensing and deployment acceptance remain separate. |
| Migration operations | Selected Qlo, storage, Postiz and [Neon → RDS](https://github.com/CraysCircle/crays-platform/tree/main/operations/neon-rds) sources | Programs retain protected inputs and historical assumptions. Six RDS files are templates; reconstruction of twelve originals was verified privately. |
| Net | Exact 982-file application tree in [crays-web-codex](https://github.com/CraysCircle/crays-web-codex/tree/2b81461e8e8b5ee6fbdb59e36215c4b574d235bf), with original MIT notice and unchanged hosting wrapper in [crays-platform](https://github.com/CraysCircle/crays-platform/tree/main/hosting/net) | Rebuild, runtime and complete dependency notice evidence remain open. |
| Coffee | Qualified two-commit capture and 53 app/public-source files in [crays-coffee](https://github.com/CraysCircle/crays-coffee), including all eight recorded source states | Earlier mixed product history, distinct WIP, media and dependency/recovery/license closure remain open. |
| Shop | Qualified three-commit capture and 466 selected source/build/public/reference files in [crays-shop](https://github.com/CraysCircle/crays-shop), including original font notices | Media, complete dependencies/runtime notices, application licensing and earlier-history closure remain open. |
| Pro | Qualified two-commit capture and 89 selected source/public files in [crays-pro](https://github.com/CraysCircle/crays-pro) | Other Pro systems, media, dependencies/runtime notices, application licensing and earlier history remain separate. |

Each listed capture was read back from GitHub and checked against its recorded source bytes. [Verification records](verification-records.md) retain the exact commits and verification scopes.

## Larger source imports still open

| Source area | Current evidence and next requirement |
| --- | --- |
| Club and shared Next.js composition | 2,045 selected original files and their baseline are public in crays-platform/apps/web. Anonymous readback verified 2,154 new or changed current files and 2,045 baseline source files against their original bytes. The prepared state adds one declared source line; it does not establish a new deployment. |
| Shared-source destination | The retained Gym repository contains the historical crays-platform subtree. Of the selected later files, 593 have identical paths and bytes there, 24 have changed at the same paths and 1,428 have new paths. The later composition includes Club, Member/SaaS and investment routes. The selected shared application is now published centrally in crays-platform/apps/web, with exact baseline and prepared-state tags. Product references must distinguish this capture from later AWS overlays. The original Gym history remains retained. |
| Other website compositions | The [eleven-site table](repository-structure.md#eleven-website-compositions) tracks each website. Org supplements, editable Fund/Fun sources and other current source/version gaps remain open. Redirects and historical variants require their own records. |
| Personal, Member, native/Core and iOS | Required current source, later overlays, distinct WIP, tests and coding/operations documents must be preserved beyond older Git commits and metadata inventories. |

The prepared Club source is not a successful new build or deployment. It must not replace the recorded running-version map merely because a source tree exists.

## Dependency and license work

For the prepared shared Next.js composition, all **47 directly declared packages** have been matched to their installed versions in the specified borrowed dependency tree. Original root notice texts have been located for **45 of those packages**, using installed files and version-bound upstream sources. The 47 original package manifests, 45 original notice files and two observed dependency locks are now preserved in apps/web. Located notice texts are not complete license clearance.

Two direct-package notice questions remain explicit:

- **server-only 0.0.1:** its metadata declares MIT, but a corresponding original notice text has not yet been established.
- **drizzle-kit 0.31.10:** the exact release package metadata declares MIT, while the located repository-root license is Apache-2.0. A matching package-specific original notice remains unestablished.

The borrowed main package-lock.json differs from the prepared dependency tree for six direct packages; it is not accepted as this application's recovery lockfile. The installed-tree lock records the observed direct versions. Neither lock comparison nor package metadata alone proves a reproducible build.

The remaining work includes the application's own rights and authorship records; transitive and bundled dependencies; Node/container/runtime notices; original copyright and modification notices; and applicable corresponding-source availability or offers. No blanket application license is assigned by inference.

The captured package manifest references **94 distinct operational helper paths** that are absent from this selected source set and its recorded baseline. Their actual qualified source versions and the remaining technical documents must be preserved before full recovery can be claimed. No operational helper or application program was executed during this source publication.

## Recovery and release

GitHub must retain every required source revision, WIP, build input, test and technical document. Complete source recovery is not proven while the gaps above remain. Credentials, private keys, customer data, database exports and protected operating bindings belong in separately protected backups, with their restoration prerequisites documented without exposing their values.

The required sequence remains: authorized development → complete GitHub source → authorized build and protected preview → exact source/artifact/license checks → concrete product-release approval → publication with a rollback version. See the [full release sequence](verification-records.md#required-release-sequence).

This assignment remains active throughout the server migration. Final completion requires the AWS owner's actual completion signal and a full reconciliation of the resulting sources, versions, documentation, access and license evidence.
