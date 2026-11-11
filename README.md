# strands-a1b-data

A1b v19 reproduction cross-job data channel. Written only by the campaign
coordinator; consumed by JY jobs as a pinned workspace repo.

- `data/teacher_v19.jsonl` — 12,909 regenerated teacher rows (frozen
  Qwen3.5-4B), interleaved from 6 row-shards, unshifted indices.
- `data/teacher_v19_train.jsonl` — same rows with indices shifted past
  train_v5's 100,449 rows (what `configs/train-parent.yaml`'s teacher_file
  expects).

sha256 (teacher_v19.jsonl / teacher_v19_train.jsonl) are recorded in each
commit message and on the MLflow contract run.
