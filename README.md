# Priv8 Shell by CoupDeGrace

[![PHP](https://img.shields.io/badge/PHP-%3E%3D5.6-blue)](https://php.net)
[![Version](https://img.shields.io/badge/Version-1.0-red)]()

> **Keywords:** php web shell, wso shell, priv8 shell, c99 shell, r99 shell, php backdoor, wordpress shell, joomla shell, drupal shell, file manager shell, php exploit, penetration testing, red team, av safe shell, obfuscated php shell, encrypted shell, php file upload, command execution shell, mysql shell, reverse shell, php reverse shell, web shell github, php web shell 2026, coupdegrace shell, webshell php, php shell login, shell priv8 php, php shell obfuscated, antimalware bypass shell, fud shell php

**Advanced PHP Web Shell — AV-Safe | Obfuscated | Multi-Feature**

### Credentials
```
Username: coupdegrace
Password: haxor2010
```

### Features

| Category | Features |
|----------|----------|
| **File Manager** | Browse, Edit, Delete, Rename, Download, Upload, Create, Chmod, Mkdir, ZIP Download |
| **Console** | Command Execution (passthru) with output buffer |
| **Eval** | Execute arbitrary PHP code |
| **MySQL** | Database query browser (connect, query, results table) |
| **BackConnect** | Reverse shell (bash -i) |
| **Tools** | Base64 Encode/Decode, Hex Encode/Decode |
| **Server Info** | System info, PHP version, SAPI, User, Server software, Limits, open_basedir, disable_functions, loaded extensions, Disk/Memory usage with progress bars |
| **Security** | SelfDestruct, File hash (MD5/SHA1), Recursive search |

### Design
- Dark navy professional theme
- CSS variables, fully responsive
- Tab-based navigation (Files | Console | Upload | Eval | MySQL | Tools | Server | BackConnect)
- No emojis, clean typography (SF Mono / Consolas)
- Professional WSO/r99-style UI

### Obfuscation
- **35 GLOBALS chunk entries** — payload split across superglobal array
- **60+ decoy variables** — fake data to confuse static analysis
- **Character-split decoder** — all function names built via single-char concatenation
- **Double anti-tamper checksum** — modified files self-destruct
- **`__halt_compiler()` trailing junk** — hides real code from text editors
- **5 layers**: gzdeflate → base64 → strrev → gzdeflate → base64 → hex
- **Fake execution traps** (`if(0){...}`) — misleads deobfuscators
- **Dynamic function verification** — checks eval() is actually executing, not being dumped

### Usage

1. Upload `cdg.php` to any writable directory
2. Access via browser: `https://target.com/path/cdg.php`
3. Login with credentials above
4. Use tab navigation for all features

### Disclaimer

This tool is for educational and authorized security testing only. The author is not responsible for any misuse or damage caused by this software.
