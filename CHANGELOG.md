# Changelog

All notable changes to this project will be documented in this file.

## [0.1.0] — 2026-02-27

### Breaking Changes

- **SurrealDB v3 + surrealdb@2.0.0** — Now targets SurrealDB v3 server with `surrealdb@2.0.0` JS SDK (previously `surrealdb@^1.3.2`)

### Changed

- Replace `PreparedQuery`/`Gap`/`Fill` with `BoundQuery` API from surrealdb@2.0.0
- Update `type::thing()` and `type::table()` to `type::record()` (v3 rename)
- Remove invalid `DEFINE FIELD id` and `DEFINE INDEX ... COLUMNS id` from schema generator (v3 restriction)
- Simplify `RecordId` serialization for SDK v2
- Update peer dependency to `surrealdb@2.0.0`
- Fork from [oskar-gmerek/surreal-better-auth](https://github.com/oskar-gmerek/surreal-better-auth) v1.0.0

---

## Pre-fork History (oskar-gmerek/surreal-better-auth)

### 1.0.0

- Full v1.0.0 adapter release for SurrealDB v2 with surrealdb@^1.3.2

### 0.6.0

- Update dependencies and bump version

### 0.5.3

- Fix unnecessary async causing unexpected Promise return
- Add `count` method to query record counts

### 0.5.0

- Dependency updates (better-auth 1.1.18, bun 1.2.2)

### 0.4.1

- Fix test RecordId type casting
- Transform date strings to `Date` objects

### 0.3.2

- Rewrite adapter to align with better-auth internal adapters
- Remove debug logs

### 0.1.0 (initial)

- Initial release with SurrealDB adapter for Better Auth
