# Meta AI Instructions — CryptoLaz SOL/USDC Orca 15M Dataset

This branch is a public research bridge for Meta AI. It is intentionally isolated from the private CryptoLaz AI Trading Co-Pilot repository.

## Dataset location

Repository: `cryptolazsmc/CryptolazSM`
Branch: `research/meta-orca-sol-usdc-15m`
Folder: `research/meta-orca-sol-usdc-15m/data/clean_csv/`

Read these files in strict numeric order:

- `part_01.csv`
- `part_02.csv`
- `part_03.csv`
- `part_04.csv`
- `part_05.csv`
- `part_06.csv`
- `part_07.csv`
- `part_08.csv`
- `part_09.csv`
- `part_10.csv`
- `part_11.csv`
- `part_12.csv`
- `part_13.csv`
- `part_14.csv`
- `part_15.csv`
- `part_16.csv`
- `part_17.csv`

Each part contains the same CSV header. When reconstructing the dataset, keep the header from `part_01.csv` only and append the data rows from all later parts.

The authoritative metadata and checksums are in `data/dataset_manifest.json`.

## Expected validation result

Before any strategy test, independently verify all of the following:

- Market: SOL/USDC
- Source context: Orca / Solana historical OHLCV
- Base timeframe: 15 minutes
- Columns: `timestamp,open,high,low,close,volume`
- Source rows before deduplication: 3000
- Duplicate boundary timestamps in the original three source blocks: `1788255000` and `1787355900`
- Duplicate conflicts: 0
- Unique clean rows: 2998
- First timestamp: `1786456800`
- Last timestamp: `1789154100`
- Every consecutive timestamp delta: exactly 900 seconds
- Gaps greater than 900 seconds: 0
- Invalid OHLCV rows: 0
- SHA-256 of the fully reconstructed clean CSV: `ec7c21859d9292d341768c04c346dfbc2a0936b46af8d861e1644ded49c14b2f`

Do not simply repeat these expected values. Independently calculate them from the CSV parts and report whether each one matches.

## Research safety rules

This dataset is RESEARCH / OBSERVATION ONLY.

Do NOT:

- execute LIVE trading
- connect or use a wallet
- submit Jupiter swaps
- modify Tiny Canary
- modify the canonical CryptoLaz Co-Pilot
- fabricate or interpolate missing candles
- use future information to generate historical signals
- optimize parameters yet
- choose parameters after looking at which settings produce the best backtest

Use only information that would have been available from closed candles at each historical timestamp. No look-ahead.

## Current task for Meta

For this first pass, ONLY reconstruct and validate the dataset.

Report:

1. number of CSV parts successfully read;
2. total data rows reconstructed;
3. unique timestamps;
4. duplicate timestamps in the clean reconstructed dataset;
5. first and last timestamp;
6. distribution of timestamp deltas and whether any gap exceeds 900 seconds;
7. invalid OHLCV rows;
8. reconstructed SHA-256 if your environment supports hashing;
9. PASS or FAIL against the expected validation values above.

STOP after dataset validation.

Do not calculate RSI, MACD, Bollinger Bands, resample 1H/4H, run a backtest, optimize parameters, or generate trading conclusions yet. Those steps require separate authorization after CryptoLaz audits this validation response.
