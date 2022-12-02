# flashburn-rewrite
Flashloan contract to pay off debt on Synthetix by selling collateral unlocked via flash loan.

Based off of https://github.com/snxgrants/flashburn, updated to support aave and 1inch v4 on optimism mainnet.

Accessible through flashburn-ui.vercel.app

---
Important notes:
- Doesn't work when you're locked out of burning due to the one week lock.
- Can't burn escrowed SNX. You need to burn enough debt to both unstake your escrow and sell enough SNX to cover the total debt of unstaked SNX, otherwise the flash loan can't be repaid and the transaction will fail.

