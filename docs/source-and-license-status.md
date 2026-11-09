# Source, license and recovery status

**Consolidation is in progress. GitHub does not yet contain the complete current CRAYS source and recovery set.** Public access, source preservation, reproducible builds and license clearance are checked separately.

Start with the [repository guide](repositories.md) and [structure rules](repository-structure.md). Detailed commit links and byte-verification records are in [verification records](verification-records.md).

## Organization and access

The organization currently contains **23 project repositories and one navigation repository**. The original twenty projects were retained; Coffee, Shop and Pro were added only after establishing their independent source roles and the absence of matching repositories.

All nine repositories originally owned by ThorbenAroundTheWorld were transferred natively, preserving their Git history and repository relationships. The authenticated personal-owner query returned zero owned repositories after those transfers.

As checked on 8 November 2026, **19 repositories are public and five remain private**: crays-fund, crays-gym, crays-franchise, crays-world and crays-ios. Their remaining confidentiality and rights checks must finish before public access is treated as complete. All repository descriptions are present.

## What is preserved in GitHub

“Preserved” below applies to the stated capture, not to every later source version, dependency, media asset or license obligation.

**Components**

- [Shared Next.js application](#source-shared-next-js-application)
- [Personal application and Chuck owner-consumer](#source-personal-application-and-chuck-owner-consumer)
- [Club/Member browser module](#source-club-member-browser-module)
- [Member Next application inputs](#source-member-next-application-inputs)
- [Qlo gateway](#source-qlo-gateway)
- [Clubs Commerce BFF](#source-clubs-commerce-bff)
- [Pure80 BFF build and probe sources](#source-pure80-bff-build-and-probe-sources)
- [Shared web operational helpers](#source-shared-web-operational-helpers)
- [Migration operations](#source-migration-operations)
- [Member document-provider build and lifecycle sources](#source-member-document-provider-build-and-lifecycle-sources)
- [Member51 Forward02 and ingress](#source-member51-forward02-and-ingress)
- [Member51 historical recovery revisions01–03](#source-member51-historical-recovery-revisions0103)
- [Vendure provider operating and verifier sources](#source-vendure-provider-operating-and-verifier-sources)
- [Vendure preferred TypeScript input](#source-vendure-preferred-typescript-input)
- [Nextcloud access-purpose52 source](#source-nextcloud-access-purpose52-source)
- [TLS19 DNS01 bootstrap operations](#source-tls19-dns01-bootstrap-operations)
- [Chuck48 and Common49 integration source](#source-chuck48-and-common49-integration-source)
- [Native iOS selected source](#source-native-ios-selected-source)
- [Native Core selected source](#source-native-core-selected-source)
- [Club Next listener and private HTTPS](#source-club-next-listener-and-private-https)
- [Work/Qlo runtime wrappers](#source-work-qlo-runtime-wrappers)
- [Net](#source-net)
- [Org website](#source-org-website)
- [Coffee](#source-coffee)
- [Shop](#source-shop)
- [Pro](#source-pro)

<a id="source-shared-next-js-application"></a>

### Shared Next.js application

**Preserved source**

2,045 original selected files in [crays-platform/apps/web](https://github.com/CraysWorld/crays-platform/tree/main/apps/web), with exact baseline and prepared-state tags, five original integration files and version-bound dependency records

**Remaining limits**

Current AWS overlays, four operational programs under fixture/contact provenance review, a qualified application lockfile, media, complete history and full rights/recovery closure remain open.

<a id="source-personal-application-and-chuck-owner-consumer"></a>

### Personal application and Chuck owner-consumer

**Preserved source**

[Original baseline and 13-overlay source compositions](https://github.com/CraysWorld/crays-platform/tree/main/apps/personal): 1,435 current text inputs, ten preimages, 30 exact direct package metadata records, 31 original notice files and eleven original generated image inputs. The [54-entry image map](https://github.com/CraysWorld/crays-platform/tree/main/apps/personal/provenance/images) records all original paths and current source evidence. A separate [private owner-consumer snapshot](https://github.com/CraysWorld/crays-gym/blob/6d943ccbfa4cc3d2ba9f80705e2e90a5a1e3ba47/protected-source-archives/chuck-original-owner-consumer54/README.md) preserves six originals (415,148 bytes), including the unchanged third-party notices, with an [exact source/version and restoration map](https://github.com/CraysWorld/crays-gym/blob/6d943ccbfa4cc3d2ba9f80705e2e90a5a1e3ba47/protected-source-archives/chuck-original-owner-consumer54/source-capture.json). The [private preferred-source snapshot](https://github.com/CraysWorld/crays-gym/blob/6d06d21265d49d3cd2526963689b13295995e3ed/protected-source-archives/chuck-build64-preferred-fifteen/README.md) adds fifteen editable originals (114,701 bytes); its [restoration map](https://github.com/CraysWorld/crays-gym/blob/6d06d21265d49d3cd2526963689b13295995e3ed/protected-source-archives/chuck-build64-preferred-fifteen/source-capture.json) also references seven already-public inputs (70,376 bytes), for 22 application-code inputs (185,077 bytes). These snapshot links require private repository access. Both compiled snapshots retain the original package notices and PostgreSQL COPYRIGHT: the separate [prepared builder/pool/bundle snapshot](https://github.com/CraysWorld/crays-gym/blob/a820ef2134a27e1f61401ce82d414e183c19d21d/protected-source-archives/chuck-consumer54-build-recipe/README.md) preserves five source artifacts without replacing the original six or the 22-input application map. The [public selected dependency snapshot](https://github.com/CraysWorld/crays-platform/blob/3cd6831a2e94af8b22b9734a0ca85346860668d0/third-party/chuck-owner-consumer54/README.md) adds 40 installed source inputs (177,251 bytes), fourteen package manifests, 26 original notice files and the PostgreSQL COPYRIGHT supplement, with a [notice index](https://github.com/CraysWorld/crays-platform/blob/3cd6831a2e94af8b22b9734a0ca85346860668d0/third-party/chuck-owner-consumer54/NOTICE.md). The [current private esbuild recovery snapshot](https://github.com/CraysWorld/crays-gym/blob/c88fe99e05fde6da3f8221e218215f73376110eb/protected-source-archives/chuck-esbuild0281-toolchain/README.md) and [artifact/restoration map](https://github.com/CraysWorld/crays-gym/blob/c88fe99e05fde6da3f8221e218215f73376110eb/protected-source-archives/chuck-esbuild0281-toolchain/source-capture.json) require private repository access and preserve ten original paths representing nine unique objects, including both binary paths. The [earlier seven-artifact snapshot](https://github.com/CraysWorld/crays-gym/blob/e20ee8e2cefca769ee2c817c7f8d3cdb06a252bc/protected-source-archives/chuck-esbuild0281-toolchain/README.md) remains preserved at 11,510,423 bytes.

The [installed esbuild 0.28.1 text snapshot](https://github.com/CraysWorld/crays-platform/blob/main/third-party/chuck-esbuild0281-tooling/README.md) preserves eight unchanged installed files (138,116 bytes) with an [upstream notice index](https://github.com/CraysWorld/crays-platform/blob/main/third-party/chuck-esbuild0281-tooling/NOTICE.md). It excludes both binary paths; installed-file identity is not complete preferred compiler source or a runnable compiler/reproduced build.

**Remaining limits**

Latest anonymous readback verified every one of the 1,535 published Personal-directory files. Both full source views restored with all 2,975 independent original comparisons passing. Forty-three image input paths (40 distinct bodies), the protected owner input, original fontkit notice, dependencies beyond the selected build inputs, complete upstream packages, external SDK/Node dependencies, preferred compiler source and assets, current runtime adoption and full rights/recovery closure remain open. One isolated GitHub-to-AWS source recovery verified all 63 non-private original BUILD input paths (362,328 bytes), including the unchanged 2,570-byte loader, plus 41 separately counted package/notice files (69,475 bytes). The protected 9,220-byte binding JSON was excluded. Executable compiler custody establishes neither complete preferred compiler source nor a reproduced build; pristine registry-byte identity and complete 64-input/runnable recovery remain unproven.

<a id="source-club-member-browser-module"></a>

### Club/Member browser module

**Preserved source**

[Original and origin35 133-file input views](https://github.com/CraysWorld/crays-platform/tree/main/modules/club-member), including the exact origin-predicate change, recorded build binding, original notices and source-only restoration

**Remaining limits**

Both views were restored from anonymous GitHub plus the protected owner input: all 266 original comparisons passed. Common-shell/current runtime adoption, original assets, native compiler notice/source questions and full rights/recovery remain open.

<a id="source-member-next-application-inputs"></a>

### Member Next application inputs

**Preserved source**

[Original 1,399-file and AWS 1,401-file source compositions](https://github.com/CraysWorld/crays-platform/tree/main/apps/web/compositions/member-source25), using an immutable common baseline, original changed source bodies and protected test-input templates

**Remaining limits**

Both complete source views were restored from anonymous GitHub plus separately backed-up owner inputs, with all 2,800 original file comparisons passing. Later runtime variants, integration, other WIP/docs, assets and full rights/recovery closure remain open.

<a id="source-qlo-gateway"></a>

### Qlo gateway

**Preserved source**

Original service/build files, original README and four tests in [crays-platform](https://github.com/CraysWorld/crays-platform/tree/main/services/qlo-gateway). The nine identified CRAYS-owned code/build/test revisions have an explicit [AGPL-3.0-only grant](https://github.com/CraysWorld/crays-platform/blob/main/services/qlo-gateway/LICENSING.md) from CRAYS AG.

**Remaining limits**

Exact runtime/dependency notices and complete source/recovery obligations remain open; captured tests were not freshly executed.

<a id="source-clubs-commerce-bff"></a>

### Clubs Commerce BFF

**Preserved source**

Nine original files and fourteen dependency notices in [crays-platform](https://github.com/CraysWorld/crays-platform/tree/main/services/clubs-commerce-bff). The six identified CRAYS-owned code/build/test revisions have an explicit [AGPL-3.0-only grant](https://github.com/CraysWorld/crays-platform/blob/main/services/clubs-commerce-bff/LICENSING.md).

**Remaining limits**

Dependency and upstream terms remain original; exact runtime/base-image licensing, full recovery and deployment acceptance remain separate.

<a id="source-pure80-bff-build-and-probe-sources"></a>

### Pure80 BFF build and probe sources

**Preserved source**

[Two original operation programs](https://github.com/CraysWorld/crays-platform/tree/bff-pure80-original-source-20261109/operations/clubs-commerce-bff/pure80-source-revision01), totaling 42,474 bytes, with exact source-field/version and embedded-probe provenance.

**Remaining limits**

The two exact CRAYS-owned revisions, including the embedded test string, now have a separate [AGPL-3.0-only grant from CRAYS AG](https://github.com/CraysWorld/crays-platform/blob/bff-pure80-own-ops-agpl3-only-20261109/operations/clubs-commerce-bff/pure80-source-revision01/LICENSING.md), bound to the actual source-author confirmation. The existing six-file BFF component grant and imported implementation terms remain separate. No image parity, executed probe, build or customer acceptance is claimed.

<a id="source-shared-web-operational-helpers"></a>

### Shared web operational helpers

**Preserved source**

90 referenced programs and two imported modules in [apps/web/scripts](https://github.com/CraysWorld/crays-platform/tree/main/apps/web/scripts), with historical baseline and exact two-file worktree tags; four additional [protected source views](https://github.com/CraysWorld/crays-platform/tree/shared-web-four-protected-source-20261109/source-archives/shared-web/four-protected-operational-helpers-20261109)

**Remaining limits**

Raw contact/fixture origins for the four templates remain unresolved; exact originals stay recoverable from the existing private GitHub repository. The checked in-memory restorer is separately AGPL-3.0-only; no new license is inferred for the four original/template programs. Runtime compatibility, external inputs and complete rights/recovery remain open; none of the original programs were executed.

<a id="source-migration-operations"></a>

### Migration operations

**Preserved source**

Selected [Personal build/helper programs](https://github.com/CraysWorld/crays-platform/tree/main/operations/personal-build), [Club/Member capture/build/adoption programs](https://github.com/CraysWorld/crays-platform/tree/main/operations/member-origin35), [Qlo/Work runtime-family revisions and original patches](https://github.com/CraysWorld/crays-platform/tree/main/operations/qlo-work-family), Qlo/storage/Postiz programs and [Neon → RDS](https://github.com/CraysWorld/crays-platform/tree/main/operations/neon-rds) sources. The [four Original30 role-preparation sources](https://github.com/CraysWorld/crays-platform/blob/original30-grantee-preparation-source-agpl-20261109/operations/neon-rds/original30-grantee-preparation-revision02/README.md) add 52,167 unchanged bytes with their [own CRAYS AG AGPL-3.0-only scope](https://github.com/CraysWorld/crays-platform/blob/original30-grantee-preparation-source-agpl-20261109/operations/neon-rds/original30-grantee-preparation-revision02/LICENSING.md).

**Remaining limits**

Programs retain protected inputs and historical assumptions. Six RDS files are templates; reconstruction of twelve originals was verified privately. Original30 describes technical NOLOGIN grantees, not LOGIN/authentication parity, consumer activation or restore acceptance.

<a id="source-member-document-provider-build-and-lifecycle-sources"></a>

### Member document-provider build and lifecycle sources

**Preserved source**

[Build revision02](https://github.com/CraysWorld/crays-platform/tree/member-document-provider51-build-rev02-source-agpl-20261109/operations/member-document-provider51/build-revision02) preserves two originals (14,954 bytes); [lifecycle revision01](https://github.com/CraysWorld/crays-platform/tree/member-document-provider51-lifecycle-source-agpl-20261109/operations/member-document-provider51/lifecycle-revision01) preserves five originals (84,208 bytes), with exact existing-helper references.

**Remaining limits**

Each group has its own exact CRAYS AG AGPL-3.0-only scope. These grants cover the listed operation programs, not the separately preserved selector, unchanged helpers, application or dependencies. Source publication is separate from build/adoption results and genuine customer document acceptance.

<a id="source-member51-forward02-and-ingress"></a>

### Member51 Forward02 and ingress

**Preserved source**

[Four exact current-revision programs](https://github.com/CraysWorld/crays-platform/blob/member-document-provider51-forward02-source-agpl-20261109/operations/member-document-provider51/forward-revision02/README.md), 75,294 bytes, with [original-path restoration map](https://github.com/CraysWorld/crays-platform/blob/member-document-provider51-forward02-source-agpl-20261109/operations/member-document-provider51/forward-revision02/source-capture.json)

**Remaining limits**

[CRAYS AG AGPL-3.0-only scope](https://github.com/CraysWorld/crays-platform/blob/member-document-provider51-forward02-source-agpl-20261109/operations/member-document-provider51/forward-revision02/LICENSING.md) covers these four programs. Initial lifecycle/build sources, selector and imported helpers keep separate scopes; source verification does not establish customer acceptance or complete runtime/recovery.

<a id="source-member51-historical-recovery-revisions0103"></a>

### Member51 historical recovery revisions01–03

**Preserved source**

[Five separately retained predecessor programs](https://github.com/CraysWorld/crays-platform/blob/member-document-provider51-historical01-03-source-agpl-20261109/operations/member-document-provider51/historical-revisions01-03/README.md), 75,186 bytes, with [original-path restoration map](https://github.com/CraysWorld/crays-platform/blob/member-document-provider51-historical01-03-source-agpl-20261109/operations/member-document-provider51/historical-revisions01-03/source-capture.json)

**Remaining limits**

[Separate CRAYS AG AGPL-3.0-only scope](https://github.com/CraysWorld/crays-platform/blob/member-document-provider51-historical01-03-source-agpl-20261109/operations/member-document-provider51/historical-revisions01-03/LICENSING.md) covers only these five versions. They are historical source, not approved replay instructions or proof that each revision executed. Dependency, rights and full recovery boundaries remain open.

<a id="source-vendure-provider-operating-and-verifier-sources"></a>

### Vendure provider operating and verifier sources

**Preserved source**

[Ten original operating and verifier programs](https://github.com/CraysWorld/crays-platform/tree/vendure-own-ops-agpl3-only-20261109/operations/vendure-native-provider-integration), totaling 215,470 bytes, with anonymous source-byte verification.

**Remaining limits**

The exact CRAYS-owned revisions and fourteen mapped nested own-code regions have a [scoped AGPL-3.0-only grant from CRAYS AG](https://github.com/CraysWorld/crays-platform/blob/vendure-own-ops-agpl3-only-20261109/operations/vendure-native-provider-integration/LICENSING.md). Vendure/framework implementations retain upstream terms; complete image/dependency source, notices, runtime adoption and recovery remain separate. Private launch/environment inputs are excluded.

<a id="source-vendure-preferred-typescript-input"></a>

### Vendure preferred TypeScript input

**Preserved source**

[The exact 3,574-byte authored source field](https://github.com/CraysWorld/crays-platform/tree/vendure-original-typescript-source-agpl-20261109/operations/vendure-native-provider-integration/preferred-source07-rev04) is now public with its immutable compiler-input relationship.

**Remaining limits**

This one CRAYS-owned revision has a separate scoped AGPL-3.0-only grant. Its original filesystem filename is unknown; the preservation filename does not invent one. No new compilation, upstream relicensing or runtime acceptance is established.

<a id="source-nextcloud-access-purpose52-source"></a>

### Nextcloud access-purpose52 source

**Preserved source**

[Four own source revisions](https://github.com/CraysWorld/crays-platform/blob/nextcloud-purpose52-source-agpl-20261109/operations/nextcloud-access-purpose52/README.md), 96,671 original bytes: pool/function pins unchanged, two SQL views protecting 16 occurrences of one account-linked fingerprint; [exact private original recovery map](https://github.com/CraysWorld/crays-platform/blob/nextcloud-purpose52-source-agpl-20261109/operations/nextcloud-access-purpose52/source-capture.json). [Two historical correction deltas](https://github.com/CraysWorld/crays-platform/blob/nextcloud-purpose45-own-deltas-agpl-20261109/operations/nextcloud-access-purpose45-history/README.md) add 9,756 original bytes.

**Remaining limits**

[CRAYS AG AGPL-3.0-only scope](https://github.com/CraysWorld/crays-platform/blob/nextcloud-purpose52-source-agpl-20261109/operations/nextcloud-access-purpose52/LICENSING.md) covers only these revisions. Account-bound intent/approval/outcome and rollback-qualification source is preserved; SQL and SSO are not activated by this publication. Functional acceptance, Nextcloud Server/apps, dependencies and complete rights/recovery remain separate. Their [separate corrective-change grant](https://github.com/CraysWorld/crays-platform/blob/nextcloud-purpose45-own-deltas-agpl-20261109/operations/nextcloud-access-purpose45-history/LICENSING.md) excludes the original Purpose45 SQL/pool, which remain privately recoverable with unresolved authorship.

<a id="source-tls19-dns01-bootstrap-operations"></a>

### TLS19 DNS01 bootstrap operations

**Preserved source**

[Three original bootstrap and APT-preparation programs](https://github.com/CraysWorld/crays-platform/tree/tls19-own-ops-agpl3-only-20261109/operations/tls19-dns01-bootstrap), totaling 15,367 bytes, with anonymous source-byte verification.

**Remaining limits**

The exact CRAYS-owned revisions have a [scoped AGPL-3.0-only grant from CRAYS AG](https://github.com/CraysWorld/crays-platform/blob/tls19-own-ops-agpl3-only-20261109/operations/tls19-dns01-bootstrap/LICENSING.md). Upstream package implementations, private keys and runtime inputs are excluded; source publication does not establish issuance, installation, renewal or ingress adoption.

<a id="source-chuck48-and-common49-integration-source"></a>

### Chuck48 and Common49 integration source

**Preserved source**

[Original Chuck48 listener](https://github.com/CraysWorld/crays-platform/tree/chuck-forwarded-transport48-source-20261109/operations/chuck-original-transport48), plus [Common49 and revision03 installation/finishing/ingress sources](https://github.com/CraysWorld/crays-platform/tree/chuck48-common49-install-rev03-source-20261109/operations/chuck-original-transport48/install-revision03). The later packet preserves five unchanged originals, 130,403 bytes, with exact existing-helper restoration references; all nine published files were anonymously byte-compared.

**Remaining limits**

Product and lifecycle source reviews passed; prior pure-check evidence was reused. This is source preservation, not authenticated customer acceptance or proof of actual runtime adoption. Protected approval, launch and runtime inputs are excluded.

<a id="source-native-ios-selected-source"></a>

### Native iOS selected source

**Preserved source**

Existing [crays-ios](https://github.com/CraysWorld/crays-ios) branch codex/ios-original-owner-person-binding is preserved at d53dfa590279d8e47accbce09844a77578ce86fa with an immutable source checkpoint tag; [version/coverage map](native-source-map.md)

**Remaining limits**

Six missing original commits and all 29 new blob versions were independently read back; the complete original Git-tree identity covers 3,511 tracked files. Public/history/privacy/rights review, ignored candidates and distinct current Core/WIP/runtime recovery remain open. No native build or development resume was performed.

<a id="source-native-core-selected-source"></a>

### Native Core selected source

**Preserved source**

[Tracked modifications/preimages and additional original inputs](https://github.com/CraysWorld/crays-platform/tree/main/apps/web/compositions/native-core-worktree-20261109) retain 28 tracked changes with exact original preimages. Within the separate 848-candidate input capture, 788 raw originals and 55 reversible protected templates are represented publicly.

**Remaining limits**

Five additional inputs still lack precise source authority. The protected templates require the separately preserved original archive. The 453 additional Core commits, other WIP, latest runtime relationship and complete dependencies/rights/recovery remain open.

<a id="source-club-next-listener-and-private-https"></a>

### Club Next listener and private HTTPS

**Preserved source**

[Original listener/bootstrap/origin/TLS fragments](https://github.com/CraysWorld/crays-platform/tree/main/services/club-next-runtime) and [controller revisions, original patches, acceptance programs and referenced helpers](https://github.com/CraysWorld/crays-platform/tree/main/operations/club-next-runtime): 35 original source-file relationships, 24 new bodies and 11 existing immutable references

**Remaining limits**

Anonymous readback verified all 33 new/changed source-commit files and all 35 original source bodies. Three exact controller hashes match the observed owner execution records. Complete current runtime/image parity, full application acceptance, wider source/dependencies/licenses and protected recovery remain open. Private keys, bound credentials and live owner controls are excluded.

<a id="source-work-qlo-runtime-wrappers"></a>

### Work/Qlo runtime wrappers

**Preserved source**

[Original bootstrap and four local CommonJS modules](https://github.com/CraysWorld/crays-platform/tree/main/services/work-qlo-runtime), with exact source hashes and the matching bootstrap pin in the captured binding-check code

**Remaining limits**

The underlying Next application, dynamic dependencies, client-asset continuity/assets, protected operating inputs and complete runtime/image/license recovery remain open.

<a id="source-net"></a>

### Net

**Preserved source**

Exact 982-file application tree in [crays-web-codex](https://github.com/CraysWorld/crays-web-codex/tree/2b81461e8e8b5ee6fbdb59e36215c4b574d235bf), with original MIT notice and unchanged hosting wrapper in [crays-platform](https://github.com/CraysWorld/crays-platform/tree/main/hosting/net)

**Remaining limits**

Rebuild, runtime and complete dependency notice evidence remain open.

<a id="source-org-website"></a>

### Org website

**Preserved source**

[Topic index, original route/page sources and developer guide](https://github.com/CraysWorld/crays-org/blob/org-page-reader-index-20261109/source-archives/org-web/org05-20261107/PAGE_INDEX.md): all 1,838 JSON inputs (168,384,874 bytes) are public, with the previous 38 original source/technical inputs retained. All 1,842 files in this addition were anonymously compared by size and SHA-256; all 1,838 original bodies match. CRAYS AG grants [AGPL-3.0-only for 25 exact own integration files](https://github.com/CraysWorld/crays-org/blob/org-web-own-code-agpl3-account4-20261109/source-archives/org-web/org05-20261107/LICENSING.md). CRAYS AG also grants [CC BY-SA 4.0 for its original prose](https://github.com/CraysWorld/crays-org/blob/e4b90fe15850d046c6a4f08b6cd5a49ec4110ae9/source-archives/org-web/org05-20261107/CONTENT_LICENSE.md) within 1,837 exact page containers, with [attribution guidance](https://github.com/CraysWorld/crays-org/blob/e4b90fe15850d046c6a4f08b6cd5a49ec4110ae9/source-archives/org-web/org05-20261107/CONTENT_ATTRIBUTION.md) and a [container scope map](https://github.com/CraysWorld/crays-org/blob/e4b90fe15850d046c6a4f08b6cd5a49ec4110ae9/source-archives/org-web/org05-20261107/content-license-scope.json). This separate text-only grant is dated 9 November 2026.

**Remaining limits**

The corpus-origin confirmation remains an owner statement. The prose grant excludes the technical route registry, whole JSON/HTML structure, metadata, code, media, fonts, logos and external material; the separate integration-code grant is unchanged. Historical legal-text pages remain historical versions, not approved current policies. The separately preserved 25,101,191-byte search-index original now has an exact private S3 archive/member restore-hash proof, but is not in this public addition. Private restore mapping and rights for the remaining 405 media/font files, complete root dependency lock/notices and complete runtime recovery remain open. The main branch is unchanged; this is a source-only tag.

<a id="source-coffee"></a>

### Coffee

**Preserved source**

Qualified two-commit capture and 53 app/public-source files in [crays-coffee](https://github.com/CraysWorld/crays-coffee), including all eight recorded source states

**Remaining limits**

Earlier mixed product history, distinct WIP, media and dependency/recovery/license closure remain open.

<a id="source-shop"></a>

### Shop

**Preserved source**

Qualified three-commit capture and 466 selected source/build/public/reference files in [crays-shop](https://github.com/CraysWorld/crays-shop), including original font notices

**Remaining limits**

Media, complete dependencies/runtime notices, application licensing and earlier-history closure remain open.

<a id="source-pro"></a>

### Pro

**Preserved source**

Qualified two-commit capture and 89 selected source/public files in [crays-pro](https://github.com/CraysWorld/crays-pro)

**Remaining limits**

Other Pro systems, media, dependencies/runtime notices, application licensing and earlier history remain separate.

Each listed capture was read back from GitHub and checked against its recorded source bytes. [Verification records](verification-records.md) retain the exact commits and verification scopes.

## Larger source imports still open

| Source area | Current evidence and next requirement |
| --- | --- |
| Club and shared Next.js composition | 2,045 selected original files and their baseline are public in crays-platform/apps/web. Anonymous readback verified 2,154 new or changed current files and 2,045 baseline source files against their original bytes. The prepared state adds one declared source line; it does not establish a new deployment. |
| Shared-source destination | The retained Gym repository contains the historical crays-platform subtree. Of the selected later files, 593 have identical paths and bytes there, 24 have changed at the same paths and 1,428 have new paths. The later composition includes Club, Member/SaaS and investment routes. The selected shared application is now published centrally in crays-platform/apps/web, with exact baseline and prepared-state tags. Product references must distinguish this capture from later AWS overlays. The original Gym history remains retained. |
| Other website compositions | The [eleven-site table](repository-structure.md#eleven-website-compositions) tracks each website. Org supplements, editable Fund/Fun sources and other current source/version gaps remain open. Redirects and historical variants require their own records. |
| Later Member source and runtime integration | The original and AWS source25 input views are now preserved above. Later runtime-family programs, the wider original source pin set, other WIP and coding/operations documents still require their exact source and recovery records. The two fixed test-binding inputs remain separate while their public-demo classification is unresolved. |

The prepared Club source is not a successful new build or deployment. It must not replace the recorded running-version map merely because a source tree exists.

## Explicit licenses for confirmed CRAYS code

On 9 November 2026, CRAYS AG expressly authorized AGPL-3.0-only for the confirmed own Qlo gateway and Clubs Commerce BFF revisions. The [component license map](https://github.com/CraysWorld/crays-platform/blob/main/LICENSING.md) links the complete unchanged GNU license texts and exact source-scope manifests: nine Qlo files and six BFF files, 15 unchanged original source revisions in total. Their hashes identify the original grant scope and do not restrict recipients from modifying or redistributing the covered code under AGPL version 3.

The later [Org integration grant](https://github.com/CraysWorld/crays-org/blob/org-web-own-code-agpl3-account4-20261109/source-archives/org-web/org05-20261107/LICENSING.md) covers 25 own source revisions under the same AGPL-3.0-only designation. The four shared-account inputs are now exactly traced to their original shared project and unchanged Platform revisions. Seven technical CSS/JavaScript files remain outside that grant pending precise modification provenance. Articles, translations, media, fonts and dependencies are excluded.

Original upstream licenses and notices remain unchanged. This initial grant covers the listed own revisions; it does not license other source areas, articles, images, videos, fonts, dependency implementations or unidentified material. It does not establish complete runtime/image or corresponding-source compliance.

## Dependency and license work

For the prepared shared Next.js composition, all **47 directly declared packages** have been matched to their installed versions in the specified borrowed dependency tree. Original root notice texts have been located for **45 of those packages**, using installed files and version-bound upstream sources. The 47 original package manifests, 45 original notice files and two observed dependency locks are now preserved in apps/web. Located notice texts are not complete license clearance.

Two direct-package notice questions remain explicit:

- **server-only 0.0.1:** its metadata declares MIT, but a corresponding original notice text has not yet been established.
- **drizzle-kit 0.31.10:** the exact release package metadata declares MIT, while the located repository-root license is Apache-2.0. A matching package-specific original notice remains unestablished.

The borrowed main package-lock.json differs from the prepared dependency tree for six direct packages; it is not accepted as this application's recovery lockfile. The installed-tree lock records the observed direct versions. Neither lock comparison nor package metadata alone proves a reproducible build.

For the distinct Member source25 input, the original application lock is now preserved and matches the application declarations and all 47 directly installed versions. Its 47 observed package manifests and 41 observed root notice files match the existing public catalog byte-for-byte, so they are referenced without duplication. This Member-specific record does not replace the prepared Club input or close complete transitive/runtime rights and recovery.

The remaining work includes the application's own rights and authorship records; transitive and bundled dependencies; Node/container/runtime notices; original copyright and modification notices; and applicable corresponding-source availability or offers. No blanket application license is assigned by inference.

The captured package manifest references **94 distinct operational program paths**. Qualified originals were located for all 94; **90 are now public**, together with their two imported helper modules. Two worktree changes and their original baseline are preserved separately. Four programs containing embedded contact/realistic business fixture literals remain outside the public selection pending independent synthetic-data provenance review. Original historical sources remain retained in the existing private Gym repository and the reviewed intake. Current AWS compatibility, external datasets and remaining technical documents must still be reconciled. No operational helper or application program was executed.

A separate Gym privacy/context review now covers 77 exact path versions across 73 named paths, including four older versions identified in the existing 20-commit comparison. Those four older versions have no remaining identified privacy-context hold. They are different paths from the four shared-web helper programs withheld above; that separate helper hold is unchanged. These reviews establish neither repository-wide privacy clearance nor authorship, license or publication permission.

## Recovery and release

GitHub must retain every required source revision, WIP, build input, test and technical document. Complete source recovery is not proven while the gaps above remain. Credentials, private keys, customer data, database exports and protected operating bindings belong in separately protected backups, with their restoration prerequisites documented without exposing their values.

All seventeen selected Spot/WebChuck working-source originals (3,729,870 bytes) are now [public with exact original-path and restoration provenance](https://github.com/CraysWorld/crays-platform/tree/spot-personal-web-two-prototype-originals-20261109/source-archives/spot-and-personal-web-working-source15-20261109). They comprise fifteen smaller source/evidence files (85,820 bytes) and two distinct complete Prototype.tsx files (3,644,050 bytes). Both scopes completed source-context/privacy review with no identified redaction holds, and the original private archive/version and member restoration proofs remain retained. The historical source15 folder name is unchanged. These separate working/integration versions do not replace the canonical applications or establish a new license grant, complete imported dependencies, current runtime adoption or complete rights clearance.

The required sequence remains: authorized development → complete GitHub source → authorized build and protected preview → exact source/artifact/license checks → concrete product-release approval → publication with a rollback version. See the [full release sequence](verification-records.md#required-release-sequence).

This assignment remains active throughout the server migration. Final completion requires the AWS owner's actual completion signal and a full reconciliation of the resulting sources, versions, documentation, access and license evidence.

The exact two Personal AWS Build02 configuration bodies and six original Python programs are now preserved under apps/personal/aws-build02 and operations/personal-build. The current configuration hashes match the existing Build02 entry. Eight original code files and four generated food image bodies were anonymously read back; together with 1,510 unchanged earlier source files, all 1,535 selected public file comparisons passed. Both complete input views still reconstruct with all 2,975 original comparisons passing. This closes these particular source gaps, while full build environments, later source and runtime adoption remain open.

## Exact native Core working-tree slice and Club Build38

The [native Core tracked-source composition](https://github.com/CraysWorld/crays-platform/tree/native-core-tracked-wip-source-20261109/apps/web/compositions/native-core-worktree-20261109) preserves 28 modifications and 28 original preimages, with exact source hashes, four immutable existing references and two protected identity templates. Its48-package lock is distinct from the shared application set. The 453-commit history and required untracked source, complete notices and current runtime mapping remain open.

The [Club Build38 composition](https://github.com/CraysWorld/crays-platform/tree/club-source38-preserved-20261109/apps/web/compositions/club-source38) preserves all 2,045 effective input relationships, reusing 2,044 exact existing files and adding the original RDS adapter. The original finite build controller, declared pool overlay/preimage, framework build ID oBGvsXCd08tp4gsMwOOo5 and 3,554 original compiled-file pins remain separate records. Anonymous restoration compared every input with its recorded original. This closes this specific source gap; compiled-output equality, runtime adoption, dependency/media recovery and full legal clearance remain unproven.

## Direct notice evidence by captured source scope

| Captured source scope | Direct packages | Packages with located root notice text | Remaining direct notice questions |
| --- | --- | --- | --- |
| Prepared shared Next.js source | 47 | 45 | server-only 0.0.1; drizzle-kit 0.31.10 |
| Distinct native Core worktree | 48 | 47 | drizzle-kit 0.31.10 |

The [Core source record](https://github.com/CraysWorld/crays-platform/tree/native-core-armor-notices-20261109/apps/web/compositions/native-core-worktree-20261109) preserves all 48 original installed package manifests and 41 installed original notice-file observations, with immutable reuse of 81 already-public original bodies. Eight newly needed original bodies were added in the first dependency capture. Five previously qualified upstream package relationships cover three additional root text files.

For GraphQL Armor cost-limit 2.4.3, max-depth 2.4.2 and max-tokens 2.5.1, exact npm integrity metadata matches the original Core lock. Their publisher gitHead commits contain the exact original package names, versions, MIT declarations and byte-identical already-public manifests. The two applicable source commits have the same original root LICENSE and copyright, with no applicable nested notice in the inspected package/ancestor paths. One unchanged root text is preserved with all three source-version relationships. This brings the Core direct-package root-text count to 47; it does not establish full legal compliance or close transitive, bundled, runtime, asset and corresponding-source obligations.

The drizzle-kit discrepancy remains explicit: package-specific MIT metadata does not establish the matching original notice while the located repository-root text is Apache-2.0. No license text, copyright holder/year or license grant is filled in by inference.

## Original runtime38 operating and browser sources

The [runtime38 source checkpoint](https://github.com/CraysWorld/crays-platform/tree/club-member-runtime38-source-20261109/operations/club-next-runtime/member-runtime38) preserves eight original code bodies: five newly added installer/bootstrap/cache/browser bodies and three immutable earlier dependencies. Both browser assertion revisions remain available. Fourteen private projection fields are documented by name, with no values, live approvals, browser output or runtime private data included.

The owner approval record names the exact already-preserved Build38 application commit. The owner return records a successful private singleton replacement while leaving readiness/customer acceptance open and requiring new Build38 HTTP acceptance. The old source18 GET receipt is not new-build acceptance. A fresh read-only Docker inspection identifies the local image configuration ID; no registry RepoDigest was present. The image configuration ID is not labeled as a registry manifest digest. Full image/source, dependency/license, protected recovery and product acceptance remain open.

## Member account entry: runtime and source versions

The [Member provider-account guide](https://github.com/CraysWorld/crays-platform/blob/main/services/member-identity/provider-account/README.md) explains the identity lookup and preserves the original route, its patch and regression-test source. The [runtime wrappers](https://github.com/CraysWorld/crays-platform/blob/main/operations/member-provider-account42/actual-runtime/README.md) and [operations source guide](https://github.com/CraysWorld/crays-platform/blob/main/operations/member-provider-account42/source-cases/README.md) connect the Member42 adoption record to installation, ingress, probe and historical source versions.

This addition preserves 16 unchanged original source versions, 165,361 bytes; all 24 published source/documentation files were anonymously compared with the prepared originals. The live adoption statement is attributed to the AWS migration owner. Private runtime configuration and customer data are excluded; complete dependency, corresponding-source and recovery checks remain open.
