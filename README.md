# SeedCash: A Specialized Device for Managing Bitcoin Cash

## General Description
SeedCash is an specialized device for ultimate security and control over your Bitcoin Cash (BCH). It empowers users to **be their own bank**, offering complete control over private keys and funds while remaining isolated from potential threats. SeedCash focuses exclusively on **BCH security**, providing a reliable, auditable, and user-friendly solution.  

---

## Security Measures
SeedCash implements multiple layers of security:  

- **Air-gapped operation**: The device works offline, reducing exposure to online attack vectors.  
- **Amnesia / No memory**: The device does **not store any private keys or any data** in memory after use.
- **Source Available code**: Publicly auditable to ensure trust and transparency.
- **GPG-signed images**: Each SeedCash .img file includes a digital signature for authenticity verification.
  
---

## Features
- **Generate Seed**: Securely create private keys.   
  - **BIP-39**: 12 words  
  - **BIP-39**: 15 words  
  - **BIP-39**: 18 words  
  - **BIP-39**: 21 words  
  - **BIP-39**: 24 words
  - **SLIP-39**: 20 words  
  - **SLIP-39**: 33 words

- **Load Seed**: Securely introduce private keys.   
  - **BIP-39**: 12 words  
  - **BIP-39**: 15 words  
  - **BIP-39**: 18 words  
  - **BIP-39**: 21 words  
  - **BIP-39**: 24 words
  - **SLIP-39**: 20 words  
  - **SLIP-39**: 33 words

- **Generate XPUB**: Export extended public keys for watch-only wallets.  

- **Generate XPRIV**: Export extended private keys.  

- **Generate BCH Addresses**: Supports both Cashaddr and Legacy formats.  

- **Sign Transactions**: Feature still in development.  

- **Educational Articles Collection**: Step-by-step guidance and resources for safe BCH management.

  
## Project Structure

```
src/
├── main.py                   
└── seedcash/
    ├── controller.py          
    ├── gui/                    
    │   ├── components.py      
    │   ├── keyboard.py       
    │   ├── renderer.py        
    │   ├── toast.py           
    │   └── screens/           
    ├── hardware/              
    │   ├── buttons.py         
    │   ├── camera.py         
    │   ├── microsd.py        
    │   └── displays/          
    ├── models/                
    │   ├── btc_functions.py   
    │   ├── seed.py           
    │   ├── wallet.py         
    │   ├── scheme.py         
    │   └── settings.py       
    ├── helper/               
    │   └── shamir_mnemonic/  
    ├── resources/          
    │   ├── fonts/            
    │   ├── img/            
    │   ├── bip39.txt       
    │   └── slip39.txt       
    └── views/                
        ├── generate_seed_views.py
        ├── load_seed_views.py
        ├── wallet_views.py
        └── setting_views.py
```


---

## Software
### SeedCash versions

| Version of SeedCash | Find File |
|----------------------|------|
| v1.1.0 | [seedcash_v1.1.0.img](https://seedcash.cash/resources) |

### Image Verification for SeedCash
SeedCash provides GPG-signed images to ensure the authenticity and security of each .img file. 
You can download the latest image [here](https://seedcash.cash/resources). The following commands guide you through verifying the downloaded image on Mac/Linux and Windows.


#### MAC / LINUX

- Open a terminal in the directory containing the downloaded folder.

- Import SeedCash public key
```bash
gpg --fetch-keys https://keybase.io/seedcash/pgp_keys.asc 
```
<img width="1291" height="210" alt="1" src="https://github.com/user-attachments/assets/102c0641-134b-4b7a-83b7-47b849bea63d" />

- Verify SeedCash public key fingerprint 
```bash
gpg --fingerprint
```
<img width="561" height="108" alt="2" src="https://github.com/user-attachments/assets/b24d84a6-6e71-4df0-8dfb-9229068d78f9" />

To verify that the public key you imported is correct, you should compare the public key fingerprint  you see locally with the public key fingerprint you find [here](https://keybase.io/seedcash) (keybase.io/seedcash).
If they match exactly, then you have the correct key from the official source. If there’s any difference — even one character — you should consider it unsafe and re‑import/verify from the official source.

<img width="846" height="549" alt="6" src="https://github.com/user-attachments/assets/95b890c7-16fb-4f49-87a0-aee645e2108b" />
<img width="993" height="608" alt="7" src="https://github.com/user-attachments/assets/d2372004-068d-4549-b3b7-b359385bb374" />


- Verify compatibility between the downloaded image and its signature
```bash
gpg --verify seedcash_v.1.1.0.img.sig seedcash_v.1.1.0.img
```
<img width="1282" height="209" alt="3" src="https://github.com/user-attachments/assets/f06e6050-1982-4531-b225-4214e30d8f62" />


#### WINDOWS

- Open a terminal in the directory containing the downloaded folder.

- Import SeedCash public key
```bash
gpg --fetch-keys https://keybase.io/seedcash/pgp_keys.asc
```
<img width="909" height="98" alt="4" src="https://github.com/user-attachments/assets/75e583f4-f2d2-4357-bced-9c4a7cc3a1ea" />

- Verify SeedCash public key fingerprint
```bash
gpg --fingerprint
```
<img width="615" height="136" alt="5" src="https://github.com/user-attachments/assets/6cc46e3e-c1b8-408e-a112-13394dff9547" />

To verify that the public key you imported is correct, you should compare the public key fingerprint  you see locally with the public key fingerprint you find [here](https://keybase.io/seedcash) (keybase.io/seedcash).
If they match exactly, then you have the correct key from the official source. If there’s any difference — even one character — you should consider it unsafe and re‑import/verify from the official source.

<img width="846" height="549" alt="6" src="https://github.com/user-attachments/assets/95b890c7-16fb-4f49-87a0-aee645e2108b" />
<img width="993" height="608" alt="7" src="https://github.com/user-attachments/assets/d2372004-068d-4549-b3b7-b359385bb374" />

- Verify compatibility between the downloaded image and its signature
```bash
gpg --verify seedcash_v.1.1.0.img.sig seedcash_v.1.1.0.img
```
<img width="956" height="100" alt="8" src="https://github.com/user-attachments/assets/0879d52b-b37f-4bb2-999f-0a96f70e6413" />


---

## Contact & Community
- **Telegram**: [SeedCash Telegram](https://t.me/+tdY1ioshyPZkOGFk)  
- **Twitter**: [@seedcash_](https://twitter.com/seedcash_)  
- **Website**: [seedcash.cash](https://seedcash.cash)

---

© 2025 SeedCash. All rights reserved.  
*"In code we trust"*




