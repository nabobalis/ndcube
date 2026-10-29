Slicing an `~ndcube.NDMeta`, and so an `~ndcube.NDCube`, `~ndcube.NDCubeSequence` or `~ndcube.NDCollection` that holds one, no longer deep-copies its values that are not axis-aware: the slice shares them with the original, as it shares a `dict` meta.
This makes slicing a cube whose `~ndcube.NDMeta` holds a large FITS header about 15 times faster.
