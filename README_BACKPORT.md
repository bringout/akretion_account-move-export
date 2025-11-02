## 16.1 Backport

- Framework backports provide `_read_group`, mail composer `default_res_ids`,
  OWL modifier support, and the extended lock dates.
- Module sources are identical to upstream 18.0; only the manifest version is
  pinned to `16.1.x`, so behaviour matches 18.0.
- Analytic plans: The exporter falls back to `account_id` when per-plan columns
  are absent (as in 16.x). This can produce duplicate plan columns unless you
  filter them in your export logic.

