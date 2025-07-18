# Evil-Droid Framework v0.4 - Enhanced Edition
**Author:** Mascerano Bachir [dev-labs]  
**Enhanced by:** Tech Sky - Security Research Team  
**Version:** 0.4 (Enhanced)

## 🔒 Legal Disclaimer
The author and contributors do not hold any responsibility for the bad use of this tool. This framework is intended **ONLY FOR EDUCATIONAL PURPOSES** and authorized penetration testing. Users are solely responsible for compliance with applicable laws and regulations.

## 📋 Description
Evil-Droid is an advanced framework designed to create, generate, and embed APK payloads for Android penetration testing. This enhanced version (v0.4) includes improved dependency management, better error handling, enhanced AV evasion techniques, and robust APK signing capabilities.

## 🖼️ Screenshots
![Evil-Droid Main Interface](https://i.imgur.com/LczO636.png)
![APK Generation Process](https://i.imgur.com/mhXxb5Q.png)

## ✨ New Features in v0.4
- **Enhanced Dependency Management**: Automatic installation with fallback packages
- **Improved APK Signing**: Modern apksigner integration with debug keystore generation
- **Better Error Handling**: Comprehensive error checking and graceful exits
- **AV Evasion Enhancements**: Advanced payload obfuscation techniques
- **Robust Package Detection**: Improved original APK analysis and injection
- **Service Management**: Automatic Apache2 and PostgreSQL service handling
- **Progress Indicators**: Visual feedback for all operations
- **Enhanced Cleanup**: Thorough temporary file management

## 🛠️ Dependencies
### Core Requirements
1. **metasploit-framework** - Payload generation engine
2. **xterm** - Terminal emulator for operations
3. **zenity** - GUI dialog interface
4. **aapt** - Android Asset Packaging Tool
5. **apktool** - APK reverse engineering tool
6. **zipalign** - APK optimization tool

### Enhanced Dependencies (v0.4)
7. **apksigner** - Modern APK signing tool
8. **keytool** - Java keystore management (JDK)
9. **wget** - Website cloning utility
10. **curl** - HTTP client for downloads
11. **unzip** - Archive extraction utility

### Alternative Packages Supported
- `android-sdk-platform-tools-common`, `android-framework-res` (for aapt)
- `android-sdk-build-tools` (for zipalign/apksigner)
- `default-jdk`, `openjdk-11-jdk`, `openjdk-8-jdk` (for keytool)

## 📥 Installation & Setup

### 1. Download the Framework
```bash
git clone https://github.com/TechSky-EH/Evil-Droid.git
cd Evil-Droid
```

### 2. Set Execution Permissions
```bash
chmod +x evil-droid
```

### 3. Run Evil-Droid Framework
```bash
sudo ./evil-droid
```
**Note:** Root privileges required for service management and dependency installation.

## 🚀 Usage Options

### Main Menu Options
1. **APK MSF** - Generate standalone Metasploit payload APK
2. **BACKDOOR APK ORIGINAL (OLD)** - Legacy embedding method
3. **BACKDOOR APK ORIGINAL (NEW)** - Enhanced embedding with advanced injection
4. **BYPASS AV APK (ICON CHANGE)** - AV evasion with custom icons
5. **START LISTENER** - Launch Metasploit multi-handler
6. **CLEAN** - Remove all generated files
7. **QUIT** - Exit framework

### Advanced Features
- **Attack Vector Mode**: Website cloning with automatic APK delivery (soon)
- **Multi-Handler Integration**: Seamless listener setup
- **Custom Icon Support**: PNG icon replacement for stealth
- **Payload Obfuscation**: Variable renaming and signature evasion

## 🔧 Technical Enhancements (v0.4)

### Dependency Management
```bash
# Automatic package installation with alternatives
install_package "primary-package" "Display Name" "alternative1" "alternative2"
```

### APK Signing Process
```bash
# Modern signing workflow
keytool -genkey → zipalign → apksigner → verification
```

### Error Handling
- Comprehensive exit codes
- Service cleanup on interruption
- Graceful failure recovery
- User-friendly error messages

### AV Evasion Techniques
- Dynamic class/method renaming
- Package structure obfuscation
- Permission randomization
- Signature scrubbing

## 📊 Supported Payloads
- `android/shell/reverse_tcp`
- `android/shell/reverse_http`
- `android/shell/reverse_https`
- `android/meterpreter/reverse_tcp`
- `android/meterpreter/reverse_http`
- `android/meterpreter/reverse_https`
- `android/meterpreter_reverse_tcp`
- `android/meterpreter_reverse_http`
- `android/meterpreter_reverse_https`

## 🎯 Use Cases
- **Penetration Testing**: Authorized Android security assessments
- **Red Team Operations**: Social engineering campaigns
- **Security Research**: Malware analysis and defense testing
- **Educational Purposes**: Learning Android security concepts

## 🔍 System Requirements
- **Operating System**: Linux (Ubuntu/Debian/Kali recommended)
- **Architecture**: x86_64
- **Memory**: Minimum 2GB RAM
- **Storage**: 5GB free space
- **Network**: Internet connection for dependencies
- **Privileges**: Root access required

## 🐛 Troubleshooting

### Common Issues
1. **Java not found**: Install JDK (`apt install default-jdk`)
2. **Apktool errors**: Update to latest version
3. **Signing failures**: Check keystore permissions
4. **Build failures**: Verify APK format and permissions

### Debug Mode
```bash
# Run with verbose output
export EVIL_DROID_DEBUG=1
./evil-droid
```

## 📜 Changelog

### Version 0.4 (Enhanced - Current)
- ✅ Enhanced dependency management with automatic installation
- ✅ Modern APK signing with apksigner integration
- ✅ Improved error handling and service management
- ✅ Advanced AV evasion techniques
- ✅ Better progress indicators and user feedback
- ✅ Comprehensive cleanup functionality
- ✅ Enhanced payload obfuscation methods

### Version 0.3 (Previous)
- Install zipalign dependency
- Detect errors and terminate services with exit mode
- Fix section bypass AV + change icon APK
- Add new method backdoor + autodetect Smali
- Fix apktool build packages APK
- Adding mode running payload in the background

## 👥 Credits & Contributors

### Original Author
- **Mascerano Bachir** - Original developer and framework creator

### Enhanced Version (v0.4)
- **Tech Sky - Security Research Team** - Framework enhancements and improvements

### Special Thanks
- **MrPedroubuntu** - Testing and feedback
- **Kader Achraf** - Code optimization suggestions
- **Youcef Yahia** - Security analysis
- **Mohammed Yacine** - Documentation improvements

## 📄 License
This is an open-source tool. If you modify or add features, please contribute back to the community.

## ⚠️ Ethical Usage
This framework is designed for:
- ✅ Authorized penetration testing
- ✅ Educational research
- ✅ Security awareness training
- ✅ Red team exercises with proper authorization

**DO NOT USE FOR:**
- ❌ Unauthorized access to devices
- ❌ Malicious activities
- ❌ Privacy violations
- ❌ Illegal purposes

## 🤝 Contributing
We welcome contributions! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request with detailed description
4. Follow coding standards and include documentation

## 📞 Support & Contact
- **Issues**: Create GitHub issues for bugs and feature requests
- **Community**: Join our security research discussions
- **Updates**: Watch the repository for latest releases

---
**Remember**: Use this tool responsibly and only on systems you own or have explicit permission to test.