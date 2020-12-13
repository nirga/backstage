---
'@backstage/plugin-catalog-backend': minor
---

Write relations directly as part of batch add / update of entities.

Slight change of the CommonDatabase contract:

- `addEntity` removed - it was unused, and unnecessary when `addEntities`
  exists.
- `DbEntityRequest` has a new field `relations` - this is the structure that is
  passed to `addEntities` and `updateEntity`.
