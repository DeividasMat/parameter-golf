This folder packages the best documented `1x H100` result still recoverable from local project notes on the `codex/runpod-2026-03-20-checkpoint` branch.

This is a `non-record` submission package, not a leaderboard attempt:
- hardware: `1x H100`
- wallclock cap: `600s`
- artifact cap respected: `11,219,666` bytes total (`int8+zlib`)
- primary score: `final_int8_zlib_roundtrip_exact val_bpb: 1.37843732`
- secondary score: `final_int8_ttt_lora val_bpb: 1.3908`

Provenance:
- The metric values come from the branch's saved best-result notes in [BEST_RESULTS.md](/Users/deividasmataciunas/Desktop/research/openai_golf/BEST_RESULTS.md).
- The original Runpod `logs/top10_winner_wd04.txt` file is no longer present in this workspace, so this package includes a documented excerpt instead of the raw training log.
- The `train_gpt.py` snapshot in this folder was copied from git commit `b0fd772`, the branch state that documented this result.

Why this is still useful:
- It records the strongest surviving `1x H100` checkpoint we can still trace locally.
- It gives OpenAI reviewers a concrete, runnable script snapshot plus the exact documented score and artifact size.
- It is explicit about what is missing, rather than pretending to be a verified SOTA or 8xH100 leaderboard run.

Documented best excerpt:

```text
- `top10_winner_wd04`
- `final_int8_zlib_roundtrip_exact val_bpb: 1.37843732`
- `final_int8_ttt_lora val_bpb: 1.3908`
- `Total submission size int8+zlib: 11219666 bytes`
```

Included files:
- `train_gpt.py` — branch snapshot nearest to the documented result
- `submission.json` — metadata for this non-record package
- `best_result_excerpt.txt` — exact locally preserved result excerpt

Limitations:
- The raw auto-produced train log is unavailable in this workspace.
- This package should be treated as a documented non-record checkpoint unless the original log is restored.
