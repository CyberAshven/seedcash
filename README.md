# SeedCash 

## Features

### Security Features


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

## 🚀 Quick Start

### Prerequisites

- **Python 3.8+**
- **pip** (Python package manager)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/SeedCashOrg/seedcash.git
   cd seedcash
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run SeedCash**
   ```bash
   python src/main.py
   ```

### Dependencies

```
Pillow>=8.0.0          # Image processing
qrcode>=6.1            # QR code generation
cryptography>=3.0     # Encryption
```

## 📱 Usage Guide

### Generating New Seeds

#### BIP-39 Seed Generation

1. Launch SeedCash
2. Select **"Generate Seed"**
3. Choose **"BIP-39"**
4. Select word count (12/24 words)
5. Generate and verify seed
6. Save securely

#### SLIP-39 Seed Generation (v1.1.0+)

1. Select **"Generate SLIP-39"**
2. Configure sharing scheme (M-of-N)
3. Set group parameters
4. Generate shares
5. Distribute shares securely

### Loading Existing Seeds

#### Manual Entry

1. Select **"Load Seed"**
2. Choose **"Manual Entry"**
3. Enter seed words using virtual keyboard
4. Verify and import

#### QR Code Scanning

1. Select **"Scan QR Code"**
2. Position QR code in camera view
3. Automatic detection and import
4. Verify seed integrity

### Backup & Recovery

#### Creating Backups

- **QR Code**: Generate QR codes for easy backup
- **Text File**: Export encrypted text files
- **Print**: Generate printable backup sheets

#### Recovery Process

- **Seed Recovery**: Restore from BIP-39/SLIP-39 phrases
- **Share Recovery**: Reconstruct from SLIP-39 shares
- **File Import**: Load from backup files

## 🔐 Security Best Practices

### ⚠️ Critical Security Guidelines

- ✅ **Always run offline** during seed generation
- ✅ **Verify checksums** before storing seeds
- ✅ **Use multiple backup methods** (paper, metal, encrypted files)
- ✅ **Test recovery procedures** regularly
- ✅ **Store backups in different locations**
- ❌ **Never share seeds digitally** (email, cloud, messaging)
- ❌ **Never photograph seed phrases** with connected devices
- ❌ **Never store seeds in plain text** on computers

### 🛡️ Additional Security Measures

- **Air-Gap Operation**: Disconnect from internet during use
- **Secure Environment**: Use in private, secure locations
- **Multiple Verification**: Double-check all seed entries
- **Secure Disposal**: Properly delete temporary files

## 📊 Version Comparison

| Feature                    | v1.0.0 | v1.1.0 |
| -------------------------- | ------ | ------ |
| BIP-39 Support             | ✅     | ✅     |
| SLIP-39 Support            | ❌     | ✅     |
| Basic Wallet               | ✅     | ✅     |
| Advanced Wallet Management | ❌     | ✅     |
| Shamir Secret Sharing      | ❌     | ✅     |
| Enhanced Security          | ❌     | ✅     |
| QR Code Support            | ✅     | ✅     |
| Multiple Languages         | ✅     | ✅     |

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Development Guidelines

- Follow PEP 8 style guidelines
- Add tests for new features
- Update documentation
- Ensure security best practices

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 🆘 Support & Community

### Getting Help

- 📚 **Documentation**: Check the `/docs` folder
- 🐛 **Issues**: [Report bugs](https://github.com/SeedCashOrg/seedcash/issues)
- 💡 **Feature Requests**: [Suggest improvements](https://github.com/SeedCashOrg/seedcash/issues)
- 💬 **Discussions**: [Community forum](https://github.com/SeedCashOrg/seedcash/discussions)

### Connect With Us

- 🌐 **Website**: [seedcash.org](https://seedcash.org)
- 🐦 **Twitter**: [@SeedCashOrg](https://twitter.com/SeedCashOrg)
- 📧 **Email**: support@seedcash.org

## ⚡ Quick Links

- [📖 Full Documentation](./docs/)
- [🚀 Getting Started Guide](./docs/getting-started.md)
- [🔒 Security Guide](./docs/security.md)
- [🛠️ Development Setup](./docs/development.md)
- [❓ FAQ](./docs/faq.md)

---

<div align="center">

**🔐 SeedCash - Secure Your Bitcoin Cash Seeds**

[![GitHub stars](https://img.shields.io/github/stars/SeedCashOrg/seedcash?style=social)](https://github.com/SeedCashOrg/seedcash/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/SeedCashOrg/seedcash?style=social)](https://github.com/SeedCashOrg/seedcash/network)

_Made with ❤️ for the Bitcoin Cash community_

</div>
