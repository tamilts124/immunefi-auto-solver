# Immunefi DeFi Bug Bounty Auto-Solver Runner

Autonomous continuous runner orchestrating Claude Autopilot, Anvil state forks, and Foundry exploit verification to detect, exploit, and report high-severity DeFi vulnerabilities on Immunefi.

## Features
- **Immunefi Target Ingestion**: Automatically crawls active high-bounty DeFi programs and identifies in-scope smart contracts.
- **Foundry State Forking**: Runs Anvil forks against live blockchain state (Ethereum, Arbitrum, Base, Optimism, BSC, Polygon).
- **Zero False-Positives**: Generates runnable `Exploit.t.sol` Foundry PoCs; findings are only accepted if `forge test --match-test test_Exploit` successfully drains protocol assets.
- **Immunefi-Standard Disclosures**: Formats verified findings into full reproducible disclosure packages with remediation diffs.

