# Run tests
- forge test

# Run test wih logs
- forge test -vv

# Run Scripts
- forge script script/DeployFundMe.s.sol

# Testing on Sepolia
forge test --match-test testPriceFeedVersionIsAccurate -vvvv --fork-url $SEPOLIA_RPC_URL

# Check code test coverage
- forge coverage --fork-url $SEPOLIA_RPC_URL

# Run test on Sepolia
forge test --fork-url $SEPOLIA_RPC_URL

# chisel - allows us to write Solidity and execute it line by line
- chisel
    !help

# Check gas in an output
forge snapshot

# Optimization
- Stop reading from storage all the time (eg.: in a loop)
- use these modifiers - as in FundMe.sol
    - view - read only
    - pure - read only and does not even access storage


# Foundry devops tool install:
- forge install ChainAccelOrg/foundry-devops --no-commit   
-https://github.com/Cyfrin/foundry-devops


# MakeFile
- deploy to sepolia:
    - make deploy ARGS="--network sepolia"







