# Transak Payment Widget — QA Manual Testing Report

📋 Manual QA testing of [Transak.io](https://global.transak.com) fiat-to-crypto widget.  
Tested flows for USD and MWK currencies → ETH purchase simulation.

---

## ✅ Tested Blocks

### 💵 USD → ETH

#### 💰 Amount Input
- ✅ Accepts valid value
- ✅ Blocks letters and symbols
- ✅ Shows correct rate and fees
📸 Screenshot:  
![usd-valid-sum](screenshots/usd-valid-sum.png)

#### 🔁 Invalid Inputs
- 🔴 Letters, symbols: rejected
![usd-invalid-sum](screenshots/usd-invalid-sum.png)
- 🔴 Negative: rejected  
![usd-negative-sum](screenshots/usd-negative-sum.png)

#### 👛 Wallet Address
- ✅ Valid ETH passes  
![usd-wallet-valid](screenshots/usd-wallet-valid.png)
- 🔴 Invalid is blocked  
![usd-wallet-invalid](screenshots/usd-wallet-invalid.png)

#### 📧 Email Field
- 🔴 Invalid email: error  
![usd-invalid-email](screenshots/usd-invalid-email.png)
- 🔴 Empty email  
![usd-empty-email](screenshots/usd-empty-email.png)
- ✅ Valid email passes  
![usd-valid-email](screenshots/usd-valid-email.png)

---

### 🌍 MWK (Malawi) → ETH

#### 🔽 MWK selected  
![mwk-select](screenshots/mwk-select.png)

#### 💰 Amount input
- ✅ Valid amount with rate/fees  
![mwk-valid-sum](screenshots/mwk-valid-sum.png)
- 🔴 Below minimum rejected  
![mwk-min-limit-error](screenshots/mwk-min-limit-error.png)

#### 👛 Wallet Address
- ✅ Valid ETH address  
![mwk-wallet-valid](screenshots/mwk-wallet-valid.png)
- 🔴 Invalid: error  
![mwk-wallet-invalid](screenshots/mwk-wallet-invalid.png)

---

## 🔍 Summary

| Area                 | Result     |
|----------------------|------------|
| Amount validation    | ✅ Passed  |
| Wallet validation    | ✅ Passed  |
| Email validation     | ✅ Passed  |
| Multi-currency test  | ✅ Passed  |
| UX feedback & errors | ✅ Clear   |

---

## 📌 Notes

- Tests performed on **15 May 2025**
- No funds were used — simulation only
- This is a QA case study, not development work
