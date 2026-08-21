# Agent and Developer Operating Rules

## Scope and public boundary

This is a **public** fork of a PepperDash Essentials plug-in. Treat every tracked change, issue, release note, workflow log, example, and generated artifact as permanently public. Do not add customer or product integration details, internal topology, personnel information, credentials, environment values, deployment evidence, or private documentation. Keep such material in an approved private repository.

## Branching and upstream

Develop only on approved non-default branches. Do not push to `main`, rewrite published history, create a release manually, or open a pull request without explicit approval. Preserve the approved PepperDash upstream baseline and retain `upstream` as the read-only sync remote. Before an upstream sync, compare the intended ref, preserve local work deliberately, and repeat release checks after integration.

## Device-control implementation

Use typed device interfaces for new device-control features and methods. Do not introduce reflection, `dynamic`, or string-based member dispatch where a typed interface can define the required contract. Keep public changes generic and independently understandable.

## Conventional Commits and semantic release

The repository uses Conventional Commits. `feat:`, `fix:`, and `perf:` are release-producing commit types under the configured Angular preset. `docs(no-release):` is for non-release documentation. Use `fix(force-patch):` only for an explicitly authorized, controlled validation release. Do not manually edit release versions, tags, or generated changelog output; the configured release workflow owns those values.

## Build and artifact proof

A release decision is not proof of a usable artifact. For each controlled release, independently verify the CI job outcome, release tag/channel, `.cplz` asset, GitHub Packages `.nupkg` publication, exact consumer restore/selection, and rollback version. A build or package proof does not authorize deployment; deployment requires separate approval.

## Before committing

Review the diff for public-safe content, preserve framework package versions unless an approved source change requires them, and state the test or CI evidence plus known limitations. If a release/publish failure involves package credentials, branch protection, shared workflows, or artifact publication, stop and report the missing prerequisite rather than bypassing controls.
