# CryptoLaz SOL/USDC Orca 15M — Meta Dataset Index

Use `META_INSTRUCTIONS.md` first. The files below are the clean, chronological, deduplicated dataset split into ordered CSV parts.

Manifest:
https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/dataset_manifest.json

Instructions:
https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/META_INSTRUCTIONS.md

CSV parts — read in strict numeric order:

01 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_01.csv
02 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_02.csv
03 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_03.csv
04 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_04.csv
05 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_05.csv
06 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_06.csv
07 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_07.csv
08 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_08.csv
09 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_09.csv
10 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_10.csv
11 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_11.csv
12 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_12.csv
13 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_13.csv
14 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_14.csv
15 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_15.csv
16 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_16.csv
17 https://raw.githubusercontent.com/cryptolazsmc/CryptolazSM/refs/heads/research/meta-orca-sol-usdc-15m/research/meta-orca-sol-usdc-15m/data/clean_csv/part_17.csv

Reconstruction rule: keep the CSV header from part_01 only; append only data rows from part_02 through part_17.

Expected reconstructed data rows: 2998.
Expected SHA-256 of the reconstructed clean CSV: ec7c21859d9292d341768c04c346dfbc2a0936b46af8d861e1644ded49c14b2f
