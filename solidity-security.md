# 🛡️ Smart Contract Security Questions (Solidity)

This section covers **Solidity security interview questions**, including attack types, common vulnerabilities, secure coding patterns, and real-world incidents. A must-know for smart contract developers and auditors.

---

## 📁 General Security Concepts

1. What are the most common smart contract vulnerabilities?  
2. What is reentrancy, and how do you prevent it?  
3. What is the checks-effects-interactions pattern?  
4. What is integer overflow/underflow? How is it mitigated in Solidity 0.8+?  
5. What is the difference between `call`, `delegatecall`, and `staticcall`?  
6. What is a fallback function and how can it be exploited?  
7. What are the risks of using `tx.origin` for authorization?  
8. How do front-running attacks occur and how can they be mitigated?  
9. What is DoS (Denial of Service) in smart contracts?  
10. What is gas griefing and how can you prevent it?

---

## 📁 Deep Dive Vulnerabilities

11. What is a delegatecall attack (e.g., Parity Wallet)?  
12. Explain the DAO hack. What vulnerability was exploited?  
13. What is storage collision and how can it occur?  
14. What is the danger of `selfdestruct` in contracts?  
15. What are flash loan attacks and how do they exploit DeFi protocols?  
16. What is a sandwich attack in MEV?  
17. What is unbounded loop vulnerability and how can it be abused?  
18. What is the issue with random number generation in Solidity?  
19. What is an approval front-run and how can it be avoided?  
20. How do you secure smart contracts against oracle manipulation?

---

## 📁 Secure Design & Best Practices

21. How does OpenZeppelin help secure your contracts?  
22. Why should you prefer `pull over push` payment models?  
23. Why is access control important and how do you implement it securely?  
24. What is circuit breaker pattern and how is it used in DeFi?  
25. What is upgradeable contract risk and how does proxy pattern mitigate it?  
26. What are the security considerations with `immutable` and `constant` variables?  
27. How do modifiers help enforce safety?  
28. How do you handle critical logic in multi-sig setups?  
29. How should you handle Ether transfers safely?  
30. What tools are used for auditing smart contracts?

---

## 📁 Tools, Audits, and Bug Bounties

31. What is Slither and how does it help in auditing?  
32. How does MythX work?  
33. What is Echidna and what type of testing does it do?  
34. What is a formal verification and when is it required?  
35. What is a bug bounty and how can you participate in one?  
36. What is a Certora specification?  
37. What’s the difference between static analysis and fuzzing?  
38. How do you conduct a manual audit of a smart contract?  
39. What is the purpose of a security audit checklist?  
40. What is a honeypot smart contract?

---

## 📁 Real-World Exploits (Case Study Style)

41. The DAO Hack (2016) – Reentrancy  
42. Parity Multisig Wallet Hack – delegatecall & uninitialized contract  
43. bZx Flash Loan Attack – oracle manipulation  
44. Poly Network Hack – private key compromise  
45. Ronin Network Exploit – validator compromise  
46. Compound Protocol Bug – duplicate reward minting  
47. Curve reentrancy exploit – DeFi pool imbalance  
48. Yearn Finance hack – misuse of vault accounting  
49. Wormhole Bridge Hack – missing signature verification  
50. Bad randomness in Fomo3D and other gambling contracts

---

---

## 🔐 Authorization & Access Control

51. What is the risk of improper access modifiers in Solidity?  
52. Why is `onlyOwner` not always sufficient?  
53. How do you implement role-based access control securely?  
54. What is `Ownable` and how is it commonly misused?  
55. How can you secure privileged functions like `mint`, `pause`, or `upgrade`?

---

## 🔄 Upgradeable Contracts & Proxy Security

56. What is the proxy pattern and why is it used?  
57. What are storage slot collisions in proxies?  
58. How does `UUPS` differ from `Transparent` proxy?  
59. How do you securely upgrade smart contracts without bricking logic?  
60. What are the risks of using `delegatecall` in proxy contracts?

---

## 🔢 Logic & Math Vulnerabilities

61. What is the impact of using uninitialized variables?  
62. What is the danger of floating point math in Solidity?  
63. Why are loops with unbounded iteration dangerous?  
64. How does SafeMath prevent overflows/underflows?  
65. What is the risk of using external contracts inside loops?

---

## 🕸 MEV, Oracles, Flash Loans (continued)

66. What is the impact of MEV on DeFi contracts?  
67. What are sandwich attacks and how do they work in AMMs?  
68. How can you mitigate price manipulation in on-chain DEXes?  
69. How do TWAP and VWAP help against flash loan exploits?  
70. How can you secure your contract from oracle timestamp manipulation?

---

## 🧠 Security Patterns & Anti-Patterns

71. What is the "pull-over-push" pattern in Solidity payments?  
72. Why should Ether transfers be limited or opt-in only?  
73. How do time locks improve protocol security?  
74. What is the "checks-effects-interactions" pattern and why is it vital?  
75. What is a trapdoor function in Solidity, and is it safe?

---

## 🧪 Auditing, Testing & Formal Verification

76. What tools are used for fuzzing Solidity contracts?  
77. What is Echidna and when should you use it?  
78. How does formal verification work in smart contract development?  
79. How do you audit access control logic in contracts?  
80. What is invariant testing and how does it differ from unit testing?

---

## 🔍 External Integration Risks

81. What are the dangers of calling unknown external contracts?  
82. What is reentrancy via ERC-777 `tokensReceived`?  
83. Why must you be cautious with `transfer()` vs `call()`?  
84. What is the difference between low-level and high-level calls?  
85. What is the impact of reentrancy on proxy upgrade contracts?

---

## 📚 Real-World Case Studies (continued)

86. SushiSwap approval bug – insufficient authorization  
87. Harvest Finance – price manipulation using flash loans  
88. Cream Finance – reentrancy + oracle exploit  
89. SafeMoon – misuse of liquidity pool accounting  
90. YAM Finance – failed rebasing logic  
91. Axie Infinity Ronin hack – validator key leak  
92. Compound rewards bug – duplicate COMP minting  
93. Mango Markets – undercollateralized flash loan manipulation  
94. Beanstalk – governance exploit via flash loans  
95. Euler Finance exploit – cross-protocol reentrancy

---

## 🔒 Bonus – General Web3 Security Hygiene

96. What are best practices for deploying contracts on mainnet?  
97. Why is testnet testing not enough for production launch?  
98. How can multi-sig wallets enhance protocol governance?  
99. What are the risks of using third-party libraries in Solidity?  
100. How can a public GitHub repo lead to private key leaks?

---


