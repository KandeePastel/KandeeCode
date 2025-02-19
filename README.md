# PBXProj Syntax Highlighter for VS Code (OSX Instructions)

A **VS Code extension** that provides **syntax highlighting** for `.pbxproj` files, which are Xcode project configuration files

---

## ✨ Features

✅ **Syntax Highlighting for PBXProj Files**
- Recognizes **keywords**, **constants**, **booleans**, **comments**, and **variables**
- Supports **uppercase constants**, **camel case identifiers**, and **dot-separated names**

✅ **Supported Highlighting Rules**
- **Comments**: `//` and `/* __BLOCK__ COMMENTS__ */`
- **Keywords**: `isa`, `objects`, `buildSettings`, `files`, `name`, `path`
- **Booleans**: `true`, `false`, `yes`, `no` (case-insensitive)
- **Uppercase Constants**: `ENABLE_FEATURE_X`, `DEBUG_MODE`
- **CamelCase Identifiers**: `PBXProject`, `UIComponent`
- **Dot-Separated Names**: `com.example.project.module`

✅ **Customizable Colors**
- Works with **VS Code themes** (adjustable in `settings.json`)

---

## 📦 Pre-Installation

#### **Install: Homebrew (brew)**
  ```sh
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```
> [Homebrew Homepage - https://brew.sh/](https://brew.sh/)

#### **Install: NPM**
  ```sh
  brew install node
  ```

#### **Install: VSCE**
  ```sh
  npm install -g vsce
  ```

---

## 📦 Installation

#### **Install from VSIX**
1. Download the `.vsix` file from **Releases** folder
2. Open VS Code and run:
   ```sh
   code --install-extension releases/kandee-code.visx
3. Restart VS Code and open a .pbxproj file

#### **Install from VS Code**
1. Open VS code
2. Open the Extensions Side-Bar (shift+cmd+x || shift+ctrl+x)
3. Click the `...` in the top-right of the Extensions Side-Bar
4. Click `Install from VSIX...`
5. Select the `*.visx` in the `releases` folder

#### **Install from Source**
1. Clone this repository:
   ```sh
   git clone https://github.com/KandeePastel/KandeeCode.git
2. Open the folder in VS Code:
   ```sh
   cd pbxproj-syntax
   code .
3. Press F5 to launch a new VS Code window with the extension loaded

---

## ⚙️ Customizing Colors
To adjust colors for specific tokens, add this to your VS Code settings.json:
  ```json
  "editor.tokenColorCustomizations": {
  	"textMateRules": [
  		{
  			"scope": "constant.language.boolean.pbxproj",
  			"settings": {
  				"foreground": "#FF5733"
  			}
  		},{
  			"scope": "variable.other.constant.pbxproj",
  			"settings": {
  				"foreground": "#3498db"
  			}
  		}
  	]
  }
```
🎨 Change the hex codes to match your preferred theme

---

## Packaging
To package the VSIX, type:
  ```sh
  vsce package --out releases/kandee-code.visx
```

---

## 🛠 Contributing
👋 Contributions are welcome!
To add new features or improve syntax rules:

1. Fork the repo & create a new branch
2. Modify File: `syntaxes/pbxproj.tmLanguage.json`
3. Press `F5` to test in VS Code
4. Submit a pull request

---

## 📜 License
This extension is licensed under the MIT License
🚀 Enjoy coding in PBXProj format with clean syntax highlighting!

---

#### **🔥 What’s Included?**
- **Project Name & Description**
- **Feature List** (what it highlights)
- **Installation Guide** (`vsix` & manual)
- **Custom Color Adjustments**
- **Contribution Guidelines**
- **License**

Let me know if you'd like any tweaks! 🚀💡
