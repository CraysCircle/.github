# Repository structure and update rules

The original twenty project repositories are the starting point. Coffee, Shop and Pro were added as standalone projects only after checking all existing repositories and confirming that no matching project repositories existed. They represent actual websites, not one repository per build attempt. Current source belongs in the repository of the same project after its origin and history have been checked. A migration capture, build attempt or source revision does not create a new product repository.

The [.github profile](../profile/README.md) is the organization entry point. [The repository guide](repositories.md) identifies each project's role. This navigation repository contains organization documentation; application implementations remain in their project repositories.

## Choosing the destination

| Material | Destination rule |
| --- | --- |
| A newer revision of an existing product | Update that product repository, retaining its original history. Record the previous and new version relationships. |
| Uncommitted product source | Preserve the actual reviewed bytes in the matching project, with its base commit and source provenance. A clean old Git HEAD does not preserve WIP. |
| Shared service code | Use the matching component in crays-platform, with a component README. Record which products consume it. Do not mix unrelated service code into an upstream fork. |
| Migration, recovery and operations programs | Keep reviewed source under the responsible repository's operations area, separately from application code, with dependency and execution assumptions. |
| An upstream project | Preserve its fork/history, original licenses and CRAYS modifications. Record the exact deployed upstream version; an unrelated current upstream branch is insufficient. |
| A historical static website or prototype | Preserve it with its historical role clearly stated. Do not present it as the current editable or deployed application. |
| A demonstrated independent project with no matching repository | Document the source ownership and reason for a separate repository before adding another project. |

The later Next.js composition includes shared Member/SaaS and investment routes as well as the Club website. Its historical crays-platform subtree remains in the retained Gym repository. The current shared application is assigned to crays-platform; product repositories reference exact composition versions rather than duplicating the full shared tree. The selected 2,045-file application and its baseline are now public in [apps/web](https://github.com/CraysCircle/crays-platform/tree/main/apps/web); later overlays, operational helpers, full history, dependencies and rights remain subject to the status page.

Do not rename repositories, move product directories, rewrite history or replace framework conventions merely to make names look uniform. A README can explain a mixed historical tree while the current source mapping is being resolved.

Member source25 uses [named compositions under apps/web](https://github.com/CraysCircle/crays-platform/tree/main/apps/web/compositions/member-source25). Each complete file manifest references unchanged source by immutable commit and retains changed source bodies or protected templates. The source-only materializer restores an exact input view; this preserves distinct versions without replacing the prepared Club tree or creating another repository. The two owner-supplied test inputs and full runtime recovery remain separate.

The separately built [Club/Member browser module](https://github.com/CraysCircle/crays-platform/tree/main/modules/club-member) is retained under modules/club-member in the same platform repository. Its original candidate has no own project package/lock. Original dependency-environment metadata stays identified as metadata; exact source views, compiler observations and the recorded build are documented independently of the Next application and current runtime adoption.

The [Personal React/Vite application](https://github.com/CraysCircle/crays-platform/tree/main/apps/personal) is preserved under apps/personal in the existing platform repository. Its original package is crays-unified-web-personal. The original output-folder source was not tracked at its original path; an exact GitHub tree comparison found only 17 current blobs in the retained historical Gym tree. The source archive therefore retains its actual baseline and ten preimages, with the 13 changes recorded explicitly. This source composition includes Gym/Personal/Member views without claiming complete current-source coverage of those products.

Personal Build02 configuration bodies stay under apps/personal/aws-build02, separate from the unchanged original configuration in source. Three original build-controller revisions and their lease/artifact/adoption helper source stay under operations/personal-build. Four generated food illustration bodies are now retained at their original source paths with their original source-authority record; 50 other source images still need custody/publication review.

## Reading a project

Each project needs a concise README explaining purpose, intended readers, implementation location, related services and its current source/release status. From there, readers should reach:

- Architecture and component responsibilities.
- Original package manifests, lockfiles, build configuration and required custom dependency sources.
- Development, build and meaningful test instructions, with actual verification limits.
- Configuration variable names and safe examples; protected credentials are supplied separately.
- Exact source commit and artifact/version bindings, plus a useful changelog.
- Original licenses, copyright, NOTICE texts, upstream provenance and modification records.
- Applicable source-availability instructions, contribution guidance and known gaps.
- Recovery prerequisites: what Git restores, what must be built, and which protected data or configuration the runtime owner restores separately.

Use existing framework layouts and original filenames. The existing crays-platform layout uses apps/web for the shared Next.js application, apps/personal for the separately built Personal React/Vite application, services/<component> for shared services, operations/<area> for reviewed operations source, hosting/<site> for hosting wrappers and docs for component/version records. These conventions are not a claim that every existing repository has already been reorganized or fully documented.

## Eleven website compositions

All eleven known website compositions must be reconciled individually. This table distinguishes retained repository candidates from completed current-source coverage.

| Website | Existing source repository relationship | Current reconciliation |
| --- | --- | --- |
| Club | crays-club retains the original static site; the later shared Next.js composition is assigned to crays-platform with exact product-version references | The 2,045 selected original files and baseline are publicly byte-verified in crays-platform/apps/web. A supplemental capture preserves 90 operational programs and two imported helpers; four programs remain under contact/fixture provenance review. Later overlays, execution inputs, full dependencies, assets and rights/recovery closure remain open. |
| Gym | crays-gym retains Gym and historical platform source; crays-platform/apps/personal preserves the captured shared frontend including Gym views | Exact Personal baseline/13-overlay text sources and ten preimages are public. The remaining 50 image bodies, later Gym/WIP, full runtime/dependency and rights/recovery closure remain open. |
| Coffee | crays-coffee now preserves the qualified Next.js capture and public source files | All eight recorded source states, including the two later CSS files, are preserved; media/dependency/license and earlier-history closure remain open. |
| Shop | crays-shop preserves the qualified capture, final fallback and original reference code | Source/history/font notices verified; media/dependency/license and earlier-history closure stay open. |
| Pro | crays-pro preserves the qualified public website and final menu/login fix | Source/history verified; other Pro systems, media/dependency/runtime and rights acceptance remain separate. |
| Net | crays-web-codex retains the exact 982-file Primal-derived source; crays-platform preserves hosting/net | Exact original tree/license and wrapper bytes verified; reproducible build and full runtime/dependency notice closure remain open. |
| Org | crays-org retains the association site | Preserve later source supplements in addition to its original commit. |
| Fund | crays-fund retains a static source snapshot | Editable/build/server-source gaps remain explicit. |
| World | crays-world retains pages, assets and editable source | Reconcile the complete latest AWS composition. |
| Award | Qualified migration website evidence exists | Resolve exact source ancestry and destination. |
| Fun | Qualified migration website evidence exists | Editable/build/server-source gaps and destination remain explicit. |

Redirects and historical variants require separate records where they differ; they do not disappear into the count of eleven. A prepared source tree or successful build is not proof of deployment.

## A recoverable source checkpoint

For every preserved component, compare the original bytes with the committed bytes and read them back from GitHub. Bind the exact commit to the relevant build inputs and artifact record. Preserve required later source deltas, tests and documentation.

A completion record must distinguish source preservation, dependency completeness, reproducible build verification, deployment and license closure. Keep unresolved checks visible rather than treating repository existence or public visibility as proof.

If source embeds a protected operational binding, preserve a clearly identified template, record both original and exported file hashes, and verify reconstruction with separately protected values. Describe the remaining protected-backup requirement; a template alone does not prove full disaster recovery.

Secrets, private keys, customer data and database exports remain in separately protected backups. Source recovery instructions must identify those prerequisites without disclosing their contents.
