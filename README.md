seu_merge_V5<- IntegrateLayers(
  object = seurat_PCA,method = CCAIntegration,
  orig.reduction = "pca",new.reduction = "cca",
  verbose = F
)

#and below is the error:

Error in `IntegrateLayers()`:
! None of the features provided are found in this assay
---
Backtrace:
    ▆
 1. └─Seurat::IntegrateLayers(...)
Run rlang::last_trace(drop = FALSE) to see 1 hidden frame.
> rlang::last_trace(drop = FALSE)
<error/rlang_error>
Error in `IntegrateLayers()`:
! None of the features provided are found in this assay
---
Backtrace:
    ▆
 1. └─Seurat::IntegrateLayers(...)
 2.   └─rlang::abort(message = "None of the features provided are found in this assay")#I don't know what's wrong with the "features"
