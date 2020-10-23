# nGAS Driller

       // Info of each user.
    struct UserInfo {
        uint256 amount;     // How many LP tokens the user has provided.
        uint256 rewardDebt; // Reward debt. See explanation below.
        //
        // We do some fancy math here. Basically, any point in time, the amount of nGAS
        // entitled to a user but is pending to be distributed is:
        //
        //   pending reward = (user.amount * pool.accNgasPerShare) - user.rewardDebt
        //
        // Whenever a user deposits or withdraws LP tokens to a pool. Here's what happens:
        //   1. The pool's `accNgasPerShare` (and `lastRewardBlock`) gets updated.
        //   2. User receives the pending reward sent to his/her address.
        //   3. User's `amount` gets updated.
        //   4. User's `rewardDebt` gets updated.
    }

## Features / settings
    uint256 burnAmount = (amount.mul(30)).div(1000); //3% will be burned every tx
TotalSupply = 1M


## Deployed Contracts
1. nGASToken.sol (0xFE86EA039f2A37fDFdD1B97a5fCa4CABC80B01B8)
2. nGASAdmin.sol (0xc0Aed4f533825C2fa1202268991D43597101395a)
3. nGASDriller.sol (0x)

        nGASDriller.sol calls
        _NGAS = 0xFE86EA039f2A37fDFdD1B97a5fCa4CABC80B01B8 //nGASToken
        _DEVADDR = 0xe817A9B11e6BF7c1dD6eFFdaFf348D581fB832fD //nGAS Deployer
        _NGASPERBLOCK = 10000000000000000000 //not defined yet!
        _STARTBLOCK = 11121337 //not defined yet! 
        _BONUSENDBLOCK = 99999999
