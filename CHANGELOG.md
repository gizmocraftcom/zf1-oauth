# Changelog

## 2.0.0

Fork of `diablomedia/zendframework1-oauth`, published as `gizmocraft/zendframework1-oauth`.

### Breaking changes

- Requires PHP `>=8.5`. Tested on PHP 8.5 and 8.6.
- Package renamed from `diablomedia/zendframework1-oauth` to `gizmocraft/zendframework1-oauth`. It now requires `gizmocraft/zendframework1-config` `^3.0.0`, `gizmocraft/zendframework1-crypt` `^2.0.0`, `gizmocraft/zendframework1-exception` `^2.0.0`, `gizmocraft/zendframework1-http` `^2.0.0` and `gizmocraft/zendframework1-uri` `^2.0.0`.

### Other changes

- No library code changes were needed: `src` runs without deprecations on PHP 8.5 and 8.6, and there are no public signature changes.
- Dev dependencies upgraded (PHPUnit 13, PHPStan 2.3, php-cs-fixer 3.95, GrumPHP 2.27). Dropped `composer-require-checker`, which has no release for PHP 8.6.
- Tests migrated to PHPUnit 13 attributes (`#[Group]`, `#[DataProvider]`). Two data-provider tests previously failed without the attribute.
- CI runs PHP 8.5 and 8.6.
