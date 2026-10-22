# CS 3780/5780 Fall 2026 — Pokéwars!

Student dataset for predicting a battle advantage score from two noisy Pokémon images. Scores range from 0 to 10; lower scores favor the second Pokémon, higher scores favor the first, and scores near 5 indicate an even matchup.

## Files

- `train.csv`: 264,000 labeled matchups; both anonymous identity labels are present on 70% of rows.
- `test.csv`: 80,000 matchups with image paths; identities and targets are blank.
- `sample_submission.csv`: submission columns `row_id,result`.
- `images/train/`: 229,600 training images.
- `images/test/`: 160,000 test images.
- `attribution/`: image credits.

Images are 32 × 32 grayscale PNGs. There are 1,025 anonymous identities; identity labels are not Pokédex numbers.

## Paths

CSV image paths are relative to this repository root, for example `images/train/<filename>.png`. Run your code from the repository root or join these paths to your dataset directory. Do not add `train_images/` or `test_images/` prefixes.

Download the repository using **Code → Download ZIP**, then extract it and use the extracted repository folder as the dataset root.

## Submissions

Preserve the row IDs from `sample_submission.csv` and replace its placeholder `result` values with finite predictions in [0, 10]. Decimal scores are allowed.

No hidden solutions, organizer files, or baseline predictions are included.
