# EthOnline

- Cross chain tooling and factory contracts for common DeFi patterns
- Overview: https://medium.com/@chimera_defi/sharedtools-c2fe8e49ba9b
- Check other repos:
- This repo - vetoken voting - UI for vote escrow projects can integrate into
- https://github.com/chimera-defi/veToken-voting
- Website https://www.sharedtools.org/project/sharedstake
- Factory contracts for master chef farming and vote escrow https://github.com/chimera-defi/sharedtools-factory
- Hardhat template for quick descriptive contract deploys https://github.com/chimera-defi/hardhat-template
- Hardhat framework with integration for metis, skale https://github.com/chimera-defi/hardhat-framework

# Vesting + Gauges + Voting
Like sharedstake.org or curve or pickle 

ve-asset and gaugeproxy implementation (can be used to turn SPIRIT into veSPIRIT and then instead of direct emissions with direct multipliers can have users vote on gauges, creates more scarcity and utility for spirit) https://github.com/pickle-finance/contracts


## Concept:


*** won't be covered in this repo, but it should be true for this to be viable
  Project is a farming based protocol
  Users can deposit funds into Vaults and earn TOK as a reward.
***


### Feature 1: Ve-asset:

Project has a token (we call this "TOK")
Users can lock up their TOK for a period and they receive "veTOK" (longer the lock, more veTOK is received)

### Feature 2: Gauges

Gauge weighting is the {total amount of veTOK voting for the gauge} / {total amount of veTOK ~that has voted?~}
The rewarded TOK per Vault is calculated based on "Gauge weighting"
Display the current gauge weighting as well as the pending gauge weighting
Show current reward ratio and pending reward ratio per vault

### Feature 3: Voting

Users can vote for a gauge or multiple gauges using their veTOK

# Thanks

This project is forked from antonell/veToken-voting with many fixes and changes copied over from it's Ruler fork by Alanthecryptodev.  
