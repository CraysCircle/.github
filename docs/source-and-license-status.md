# Source and license status

This page distinguishes completed source-preservation work from the remaining AWS/version/license reconciliation. It is not a declaration of full legal or production acceptance.

## Established milestones

- All nine repositories originally owned by ThorbenAroundTheWorld were transferred natively to CraysCircle, including four private repositories. No source repository was replaced with a copy or deleted.
- The authenticated, fully paginated personal-owner repository query returned zero owned repositories after the transfers.
- Before/after Git references, branches, issues/PRs, releases, hooks, deploy keys and collaborator permissions were compared. The Git content was preserved. Newly registered organization CodeQL/dependency-graph jobs were documented separately from product deployment workflows.
- The original Qlo gateway's five qualified source/build files are preserved in [crays-platform at commit 1b6e9188a1723be54d1f21e718142f019088f0d4](https://github.com/CraysCircle/crays-platform/commit/1b6e9188a1723be54d1f21e718142f019088f0d4). Their remote file bytes match the supplied original/build hashes. This is a source-capture milestone; it does not approve runtime startup or close its remaining license evidence.

- The platform repository is public, with anonymous metadata and original gateway source access verified. Its [supplement commit e490404d43c400f397d2eb6e4b9f0fd62b48966b](https://github.com/CraysCircle/crays-platform/commit/e490404d43c400f397d2eb6e4b9f0fd62b48966b) preserves four original tests, the original README and reviewed Qlo account2/storage-guard programs. All fifteen supplemented source/documentation files were read back and compared byte for byte; no program was executed.
- All twenty project descriptions and category topics have been verified. The [structure and update rules](repository-structure.md) explain how existing repositories receive newer source and how the eleven websites are tracked.

## Public access

The owner has requested public access to every source repository. Existing private repositories are being checked across their contents and Git history before their visibility changes. Secrets, private keys and personal customer data must not be exposed. The public-access work is not complete until the actual repository visibility and unauthenticated access have been verified.

## License and source evidence still being completed

- Exact original license and NOTICE texts for the versions actually used in AWS images, including runtime and bundled dependencies.
- Corresponding-source and source-offer obligations, with source that the relevant recipients can actually obtain.
- Original authorship and licensing records where the retained CRAYS project roots have no explicit LICENSE/NOTICE metadata. No license is assigned by inference.
- Full source-to-commit-to-artifact mappings for the eleven website compositions and the shared/native services.
- Required uncommitted source changes, test sources and coding/operational documentation. Source snapshots must not omit actual later changes merely because an older Git HEAD exists.

Examples of known source reconciliation points include the Coffee CSS states absent from its prior commit, originally untracked BFF/gateway source files, and native/Core WIP for which metadata is not yet a content-preservation receipt. These points remain open until their actual contents and version relationships are verified.

## Release process

1. Authorized development on a fresh XXL environment.
2. Complete source and documentation committed to Git/GitHub under CraysCircle.
3. Deploy-trigger inspection before push; isolated source branches where needed.
4. Authorized AWS/Amplify build and protected preview.
5. Exact source, commit, artifact, license/NOTICE and source-availability checks.
6. Concrete user approval for the product release.
7. Publication through the responsible deployment owner, with an identified rollback version.

The GitHub consolidation remains active throughout the server migration. Final acceptance requires the AWS owner's actual completion signal and an independent final reconciliation of the resulting sources and documentation. No legal-compliance claim is based solely on a public repository, package license field, build, screenshot or image pin.
