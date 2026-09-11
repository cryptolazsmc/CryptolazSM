# CryptoLaz Meta / Orca SOL-USDC 15M Research Dataset

Purpose: public, isolated research bridge for Meta strategy testing using real SOL/USDC Orca 15-minute OHLCV data.

This branch is intentionally separate from the CryptoLaz AI Trading Co-Pilot canonical repository and must not be treated as LIVE, PAPER execution, Tiny Canary, wallet, or production code.

## Intended raw source files

- SOL_USDC_ORCA_15M_BLOCK1.json
- SOL_USDC_ORCA_15M_BLOCK2.json
- SOL_USDC_ORCA_15M_BLOCK3.json

The three source blocks represent one continuous historical series. Boundary timestamps overlap between adjacent blocks, so any consumer must deduplicate strictly by Unix timestamp before analysis.

Research rules:
- observation / research only
- no live trading
- no wallet use
- no Jupiter swaps
- no modification of Tiny Canary
- no modification of canonical Co-Pilot
- no look-ahead
- use only closed candles
- preserve raw source data

Recorded here intentionally so future CryptoLaz work remembers that Meta/Orca research data was placed in `cryptolazsmc/CryptolazSM` on branch `research/meta-orca-sol-usdc-15m`.
