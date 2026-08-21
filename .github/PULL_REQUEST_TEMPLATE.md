## Summary

Describe the generic plug-in change and its intended behavior.

## Baseline and scope

- [ ] I identified the approved upstream branch/tag/commit used as the baseline.
- [ ] This pull request targets an approved non-default branch.
- [ ] I did not include customer, product-integration, environment, credential, personnel, or deployment context.
- [ ] New device-control behavior uses typed interfaces rather than reflection, `dynamic`, or string-based member dispatch.

## Validation

- [ ] I reviewed the configured package references and source compatibility.
- [ ] I ran the applicable local checks or documented why they could not run.
- [ ] I reviewed CI results and recorded any limitation or failure.

## Release impact

- [ ] Commit messages follow Conventional Commits.
- [ ] `feat:`, `fix:`, or `perf:` is used only when a release is intended.
- [ ] `docs(no-release):` is used for documentation-only work.
- [ ] `fix(force-patch):` is used only for an explicitly approved controlled validation release.
- [ ] If a release occurs, I will verify the tag/channel, `.cplz` asset, GitHub Packages publication, consumer selection, and rollback reference separately.

## Deployment boundary

- [ ] This pull request does not authorize processor or production deployment.
