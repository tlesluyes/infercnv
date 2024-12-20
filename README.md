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
- 2024/09/05:
  - Change the color scheme.
  - Tiny clusters (<1% of all tumor cells) are set to black, allowing other clusters to have distinct colors
- 2024/12/09:
  - Fix a rare issue where some cells seem unassigned to a cluster in `row_groupings` (are `NA`)