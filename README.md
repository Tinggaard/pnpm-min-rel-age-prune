# Steps to reproduce

```bash
pnpm install
```

Notice that the `pnpm-workspace.yaml` has changed, and now contains invalid YAML:

```diff
diff --git a/pnpm-workspace.yaml b/pnpm-workspace.yaml
index f371248..4f2cd9a 100644
--- a/pnpm-workspace.yaml
+++ b/pnpm-workspace.yaml
@@ -1,4 +1,5 @@
 minimumReleaseAgeExcludePrune: true
 minimumReleaseAgeExclude:
+  - is-number
 - is-number
 - unused-package
```
