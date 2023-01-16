# verse-dex-tokens

This is a community-sourced token list used to power the [Verse DEX](https://verse.bitcoin.com/).

If you wish to add an SEP-20 or ERC-20 token / liquidity pool to the Verse DEX, follow the instructions below:

# How to add your token / liquidity pool to [verse.bitcoin.com](https://verse.bitcoin.com)
1. Open a pull request on this repo ([example](https://github.com/bitcoin-portal/verse-dex-tokens/pull/2)) containing the following:
    - Add your token config to [tokens.json](https://github.com/bitcoin-portal/verse-dex-tokens/blob/trunk/config/tokens.json). Include any liquidity pairs you'd like to list under `pairs` e.g. :
    ```javascript
        {
            "abbr": "JOY", // token symbol
            "value": "JOY", // same as abbr
            "protocol": "SEP20_PROTOCOL",
            "blockchain": "BCH",
            "label": "JOY", // token display name
            "ticker": "joy",
            "explorer": "https://www.smartscan.cash/tx/",
            "token": "0x6732E55Ac3ECa734F54C26Bd8DF4eED52Fb79a6E", // token contract address
            "decimals": 18,
            "pairs": ["BCH", "TANGO"] // this will add JOY/BCH and JOY/TANGO to the list of liquidity pools
        }
    ```
    - A 64x64 png of the token icon to the /icons directory
    - A wallet address from which you will provide the initial liquidity for the pool
    
2. Our team will review your PR and merge it. You will then be able to view and add initial liquidity to the new pools on the Verse DEX using your provided wallet address.

## Syntax for token pairs ##
- Bitcoin Cash: "BCH"
- Joystick: "JOY"
- TANGO: "TANGO"
- LAW: "LAW"
- Green Ben: "EBEN"
