# Native iOS and Core source map

This page identifies the retained native source and the separate Core/source-recovery work. Source custody, privacy/license review, current AWS runtime mapping and native product acceptance are tracked individually.

## Current native checkpoint

| Item | Exact source relationship |
| --- | --- |
| Repository | [CraysWorld/crays-ios](https://github.com/CraysWorld/crays-ios), repository ID 1426572268. Currently private while full source/history/privacy/rights review continues. |
| Current selected source branch | [codex/ios-original-owner-person-binding](https://github.com/CraysWorld/crays-ios/tree/codex/ios-original-owner-person-binding) |
| Preserved source commit | `d53dfa590279d8e47accbce09844a77578ce86fa` |
| Immutable source checkpoint tag | [native-ios-source-preserved-20261109](https://github.com/CraysWorld/crays-ios/tree/native-ios-source-preserved-20261109) |
| Original Git tree | `aa426f9352f5e6924ffe3491cb07da82ab42343c`, containing 3,511 tracked files. Tree identity was verified; this record does not claim a new individual hash readback of all 3,511 files. |
| Original branch update | Six original commits after `8977297e844c893cd3377168402005bab356360e`, preserving original commit IDs and parent relationships. Nineteen documentation/handoff paths changed, with 29 original blob versions independently size/SHA-256 checked through GitHub. Native product code is unchanged across this source update. |
| Default branch | main remains at its existing `cad62055f47fe73185b65e5279e5a79cd0e99d91` checkpoint. Use the selected branch/tag above to inspect the current owner source and handoffs. |

The selected branch contains the native app, Core bridge, original tests/build configuration, retained vendor/license material and current owner handoffs. Other historical branches remain preserved. The direct native-repository inspection found a clean tracked working tree at the captured commit. Separately ignored source candidates, protected state and evidence still require individual reconciliation; a clean Git status does not establish their complete custody.

The private code and historical notices remain subject to the existing public-access review. Exact upstream comparisons have already qualified many public cryptographic test fixtures; remaining application/binary/privacy/rights work is still open. This source checkpoint does not close that review or introduce a blanket license.

## Build and product evidence

The existing iOS workflow supports workflow_dispatch only, with its original cost gate. No workflow was dispatched, no new run was observed for this source commit, and repository Actions permissions were preserved. The default branch, visibility, native product source, owner development pause and device/TestFlight gates remain unchanged.

Native source preservation is separate from a new build, simulator/device proof or installable release. Original owner handoffs retain the earlier Apple/source relationships and their acceptance limits.

## Core and later shared runtime source

The preserved source authority still identifies the Core worktree at `/srv/crays/worktrees/ios-core-native-01a14a1b`, base commit `c2018d04f6a52d8716326a098dde7624cbb18963`. A fresh normal Git status reproduces the handoff's 595 entries: 28 tracked modifications and 567 untracked entries. Expanding untracked directories produces 5,202 file-status entries. These counts include local dependency fixtures, generated material, source candidates and protected/certificate-related material; they are not a count of accepted or publicly preserved source files.

The [28-file tracked Core working-tree slice and all 28 exact committed preimages](https://github.com/CraysWorld/crays-platform/tree/native-core-tracked-wip-source-20261109/apps/web/compositions/native-core-worktree-20261109) are now preserved in the existing platform repository. Four preimages reuse immutable existing source; two files retain reversible protected identity-seed templates. Source commit 8580d3227f4ab6928e4eba3fa7fa751b289c6379 passed anonymous readback of 61 changed/new files and all 56 original reconstructions using 13 separately protected seed bindings. The separately versioned private binding backup passed exact body readback.

The [distinct 48-package Core dependency record](https://github.com/CraysWorld/crays-platform/tree/native-core-armor-notices-20261109/apps/web/compositions/native-core-worktree-20261109) now retains all original package metadata and 41 installed root notice files. Version-specific upstream evidence supplies root texts for eight additional packages. Root texts are located for 47 of 48 direct packages; drizzle-kit 0.31.10 remains unresolved. The three GraphQL Armor relationships match exact npm integrity values, publisher source commits and byte-identical original manifests. Transitive, bundled/runtime, copyright/modification and source-availability obligations remain open. This Core package set must not be substituted for the shared application set.

The 453-commit Core history after the known Gym ancestor and required untracked source remain open. The expanded untracked set includes5,174 files, with substantial dependency fixtures/artifacts requiring qualification. The older checkout is a recovery/source authority, not an automatic selection of the newest shared Core runtime.

The original native migration handoff distinguishes later Web/Core and Chuck-owned integrations. Read their actual source/release manifests, exact selected artifacts and protected recovery dependencies when mapping AWS runtime versions. Historical artifact-root IDs, Git commits, framework build IDs and image manifest digests each retain their own meaning. Current whole-runtime/source/dependency/notice and protected recovery reconciliation remains open.

Use the [repository structure rules](repository-structure.md), [overall source/license status](source-and-license-status.md) and [verification records](verification-records.md) for the broader consolidation.
