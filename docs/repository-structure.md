# Repository structure and update rules

The existing twenty project repositories are the starting point. Current source belongs in the repository of the same project after its origin and history have been checked. A migration capture, build attempt or source revision does not create a new product repository.

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

Do not rename repositories, move product directories, rewrite history or replace framework conventions merely to make names look uniform. A README can explain a mixed historical tree while the current source mapping is being resolved.

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

Use existing framework layouts and original filenames. For a new shared service, the existing crays-platform layout uses services/<component>, operations/<area> and docs. These conventions are not a claim that every existing repository has already been reorganized or fully documented.

## Eleven website compositions

All eleven known website compositions must be reconciled individually. This table distinguishes retained repository candidates from completed current-source coverage.

| Website | Existing source repository relationship | Current reconciliation |
| --- | --- | --- |
| Club | crays-club retains the original static site; newer Club/Member composition has distinct source ancestry | Map the complete newer composition and shared inputs before calling the repository current. |
| Gym | crays-gym retains Gym and historical platform source | Reconcile current source and WIP separately from older committed material. |
| Coffee | Qualified migration source and deployed CSS delta are recorded | Exact existing destination and complete current bytes remain to be reconciled. |
| Shop | Qualified migration source and later source fix are recorded | Resolve the complete composition and existing destination. |
| Pro | Qualified migration source and later source fix are recorded | Resolve the complete composition and existing destination. |
| Net | crays-web-codex retains the Primal-derived website | Bind exact application source, AWS hosting wrapper and original license. |
| Org | crays-org retains the association site | Preserve later source supplements in addition to its original commit. |
| Fund | crays-fund retains a static source snapshot | Editable/build/server-source gaps remain explicit. |
| World | crays-world retains pages, assets and editable source | Reconcile the complete latest AWS composition. |
| Award | Qualified migration website evidence exists | Resolve exact source ancestry and destination. |
| Fun | Qualified migration website evidence exists | Editable/build/server-source gaps and destination remain explicit. |

Redirects and historical variants require separate records where they differ; they do not disappear into the count of eleven. A prepared source tree or successful build is not proof of deployment.

## A recoverable source checkpoint

For every preserved component, compare the original bytes with the committed bytes and read them back from GitHub. Bind the exact commit to the relevant build inputs and artifact record. Preserve required later source deltas, tests and documentation.

A completion record must distinguish source preservation, dependency completeness, reproducible build verification, deployment and license closure. Keep unresolved checks visible rather than treating repository existence or public visibility as proof.

Secrets, private keys, customer data and database exports remain in separately protected backups. Source recovery instructions must identify those prerequisites without disclosing their contents.
