Migration from the previous smart contract : <a href="https://0xcatether.github.io/0xcate/migrate.html">Migrate</a> 

Telegram : <https://t.me/joinchat/G0Ya5ErA1rGcFaDFbtcBJA>

Discord : <https://discord.gg/6TgMteD>
# Welcome to 0xCATE website

CatEther introduces a new mechanic: "Proof of Use"

To understand the concept proof of use we can expose a practical use case: the token reward from transfer is meant to cover the gas fee for transaction, aiming to make it free or lower transaction cost rewarding the sender with 0xcate token.

Each time you successfully make a transaction it will create 1 token, sending 0.5 to your address and the other 0.5 to an address of your choice.
You can just send a transaction of 0 CATE and this will create 1 token.

If the Donation Address is not set it will be lost by default.

You can also override the default donation address by calling a specific function : "transferAndDonateTo".

## General Information

## MINING SPECIFICATION

There is no limit to the coin supply
Reward follow more or less the same emission rate as dogecoin
```python
FUNCTION GETMININGREWARD() PUBLIC CONSTANT RETURNS (UINT) {
        BYTES32 DIGEST = SOLUTIONFORCHALLENGE[CHALLENGENUMBER];
        IF(EPOCHCOUNT > 160000) RETURN (50000   * 10**UINT(DECIMALS) );//  14.4 M/DAY 
        IF(EPOCHCOUNT > 140000) RETURN (75000   * 10**UINT(DECIMALS) ); //  21.6 M/DAY
        IF(EPOCHCOUNT > 120000) RETURN (125000  * 10**UINT(DECIMALS) ); //  36.0 M/DAY
        IF(EPOCHCOUNT > 100000) RETURN (250000  * 10**UINT(DECIMALS) ); //  72.0 M/DAY
        IF(EPOCHCOUNT > 80000) RETURN  (500000  * 10**UINT(DECIMALS) ); // 144.0 M/DAY
        IF(EPOCHCOUNT > 60000) RETURN  (1000000 * 10**UINT(DECIMALS) ); // 288.0 M/DAY
        IF(EPOCHCOUNT > 40000) RETURN  ((UINT256(KECCAK256(DIGEST)) % 2500000) * 10**UINT(DECIMALS) );   // 360.0 M/DAY
        IF(EPOCHCOUNT > 20000) RETURN  ((UINT256(KECCAK256(DIGEST)) % 3500000) * 10**UINT(DECIMALS) );   // 504.0 M/DAY
                               RETURN  ((UINT256(KECCAK256(DIGEST)) % 5000000) * 10**UINT(DECIMALS) );   // 720
```                               

0xCATE is a mineable token on ethereum. 

<script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
