# `crypto-icons`

## 1) What?

A Unified repository containing optimized icons for Cryptocurrency assets.

## 2) Current state
This is a raw copy right now.

### To be deleted soon

- Directories
```
./assets/logo
./assets/svg
```
- Files

All non-conforming files

## Structure


```
./assets
./assets/fantom
./assets/base
```

## Allowed formats

### File formats
- PNG
  - MUST be **400px x 400px** in size.
  - MUST be less than **32 KB**
  - Should be Transparent.
  - Should NOT fade on dark background #001337 (navy blue).
  - Should have a circular or rounded edges (5px minimum) background if it is low contrast on dark background.

- SVG
  - MUST be less than 32KB
  
### File Name formats
- Must be the fully qualified **address** of the asset.
  - Note: Native ETH (or BNB/MATIC/FTM etc) should be `0xeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee`.png or .svg
- Must be in **lowercase** if the blockchain is case-insenstive (Ethereum-like chains).
- Must be in exact Checksummed case if blockchain is case-sensitive (Bitcoin-like or Tron-like chains)

## Submitting logos
1. Fork this repository.
2. Add logos in appropriate blockchain's directory
3. Commit your changes and open a **Pull Request** on this repository.
4. Tag someone to review and approve your submission.

### Rejections
Your submission will be starightaway rejected if it doesnt conform to the [Allowed formats](#Allowed-formats).