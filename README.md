# verse-dex-tokens

This is a community-sourced token list used to power the [Verse DEX](https://verse.bitcoin.com/).

# How to add your token / liquidity pool to [verse.bitcoin.com](https://verse.bitcoin.com)
1. Open a pull request on this repo containing the following:
    - Add your token config to [tokens.json](https://github.com/bitcoin-portal/verse-dex-tokens/blob/trunk/config/tokens.json). Include any liquidity pairs you'd like to list under `pairs` e.g. :
    ```javascript
        {
            "abbr": "FLEX",
            "value": "FLEX",
            "protocol": "SEP20_PROTOCOL",
            "blockchain": "BCH",
            "label": "FLEX",
            "ticker": "flex",
            "explorer": "https://www.smartscan.cash/tx/",
            "token": "0x98Dd7eC28FB43b3C4c770AE532417015fa939Dd3",
            "decimals": 18,
            "pairs": ["BCH", "flexUSD"] // this will add the FLEX/BCH and FLEX/flexUSD to the list of liquidity pools
        }
    ```
    - A 64x64 png of the token icon to the /icons directory
    - A wallet address from which you will provide the initial liquidity for the pool
2. Our team will review your PR and merge it. You will then be able to view and add initial liquidity to the new pools on the Verse DEX using your provided wallet address.
