``copy.copy`` of an `~ndcube.NDMeta` no longer shares its axes, key comments and data shape with the original, so `~ndcube.NDMeta.add` and ``del`` on the copy no longer change the original.
