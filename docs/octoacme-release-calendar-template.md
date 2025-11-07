# OctoAcme Release Calendar Template

## Purpose
Track planned releases to maintain visibility across teams and stakeholders.

## How to Use
- Update this calendar during sprint planning when releases are scheduled
- Include all relevant fields for each release entry
- Keep entries up to date as dates or scope change
- Archive completed releases to a separate section or document

## Release Entry Template

```yaml
release_name: v2.3.0
target_date: 2025-12-15
owner: Jane Doe
release_type: Minor
rollback_plan: docs/rollback-procedures.md#v2.3.0
notes: Includes new dashboard feature, requires DB migration
```

## Example Releases

| Release | Target Date | Owner | Type | Rollback Plan | Notes |
|---------|-------------|-------|------|---------------|-------|
| v2.2.1 | 2025-11-20 | John Smith | Patch | Standard rollback | Hotfix for login bug |
| v2.3.0 | 2025-12-15 | Jane Doe | Minor | Custom rollback | New dashboard, DB migration required |
