# 🔍 Light Audit – ERC20 PumpDaddy Token

**Auditor:** Febri Nirwana  
**Date:** July 2025  
**Contract Address:** 0x29FfAEfB147C57dB2B787766eD9bb5b0fDbA3ff8
**Network:** Ethereum (Mainnet/Testnet)  
**Repo:** pumpdaddy-erc20-audit

---

## 📄 PDF Report

🔗 [Download Full Report](./PumpDaddy_Audit_FebriNirwana_July2025.pdf)

---

## 🐞 Summary of Findings

| No | Severity | Issue Description                              |
|----|----------|--------------------------------------------------|
| 1  | Medium   | Public setter for private variable `var_SeHBuB()` |
| 2  | Medium   | Custom ERC20 logic without standard libraries    |
| 3  | Low      | Unused function `add_NnuxW()` writing to storage |
| 4  | Neutral  | No ownership or control functions implemented    |

---

## 🛠️ Recommendations

- Restrict or remove `update_var_SeHBuB()` to prevent unintended data manipulation
- Replace manual ERC20 logic with OpenZeppelin standard
- Delete unused function `add_NnuxW()` to save gas and reduce confusion
- Add access control if future logic is planned

---

## 🧠 Notes

This contract appears to be a minimal ERC20 token with no active transactions besides deployment.  
However, the presence of obfuscated variable names and publicly writable storage raises red flags and could indicate honeypot behavior or hidden trap logic.

---

> Audit by [Febri Nirwana](https://github.com/febrinirwana)  
> For educational and portfolio purposes only. No guarantees are made regarding the safety of the contract.

