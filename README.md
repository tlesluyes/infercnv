# infercnv

Visit project [wiki](https://github.com/broadinstitute/inferCNV/wiki) for InferCNV documentation.

## Forked from [broadinstitute/infercnv](https://github.com/broadinstitute/infercnv)

### Custom changes (tlesluyes)

- 2024/07/11:
  - Use `ward.D2` as the default hclust method (instead of `ward.D`).
  - Propagate `hclust_method` to the `hclust` functions.
  - Add and propagate `dist_metrics` (default is `"euclidean"`) to the `parallelDist` functions.
  - Add `custom_colors` so cells can be highlighted with specific colors.
- 2024/08/05:
  - Add `save_expr_cluster_rds` to `run()` so expression data for clustering can be saved prior to be overwritten by denoised values.
