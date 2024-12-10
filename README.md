# `equalizer-tokens`

A Unified repository containing optimized icons for equalizer cryptocurrency assets.

- Provides teams with ability to manage their token images
- Provides teams with ability to manage their token symbol and name

# Managing token images

## Allowed formats

### File formats

- PNG

  - MUST be a minimum of **400px x 400px** in size.
  - MUST only be placed in a chain root folder `/<chain>/tokens/<your-token-address>.png`
  - Should be Transparent.
  - Should NOT fade on dark background #001337 (navy blue).
  - Should have a circular or rounded edges (5px minimum) background if it is low contrast on dark background.

- SVG

  - SVG are only allowed as a reference if you are having trouble creating a PNG and want the team to help you.

### File Name formats

- Must be the fully qualified **address** of the asset.
  - Note: Native ETH (or BNB/MATIC/FTM etc) should be `0xeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee`.png or .svg
- Must be in **lowercase** if the blockchain is case-insensitive (Ethereum-like chains).
- Must be in exact Check-summed case if blockchain is case-sensitive (Bitcoin-like or Tron-like chains)

## Submitting logos

1. Fork this repository.
2. Add logos in appropriate blockchain's directory
3. Commit your changes and open a **Pull Request** on this repository.
4. Tag someone to review and approve your submission.

### Managing cache

When changing a token image, you will need to clear the auto resized images from our cache.

1. Delete `/<chain>/tokens/<size>/<your-token-address>.png`
2. Repeat for all sizes
3. Commit your changes and open a **Pull Request** on this repository.
4. Tag someone to review and approve your submission.

### Rejections

Your submission will be straight away rejected if it does'nt conform to the [Allowed formats](#Allowed-formats).

# Managing Token symbol and name

DeFi changes rapidly and we provide a method for you to override the default token names and symbols stored on-chain.

1. Add your token to the `/<chain>/tokens.json` file
2. Use the check summed <address> as the key
3. Conform to this object format

```
{
  "<your-token-address>": {
    name: "<your-new-name>"
    symbol: "<your-new-symbol>",
    tags: []
  }
}
```

## Token tags

We provide a default set of tags to categorise tokens, please only use tags in the default set which can be found at `/tokens-tag.json` and be honest, if you are launching a `degen` meme token, do not tag it as a blue-chip or your token submission will be rejected. If a team attempts to trick users then delisting and/or removal of gauges may occur.

