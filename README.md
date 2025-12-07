# Eudic Helper – Oxford Lookup & Pronunciation
A powerful Alfred workflow that enhances the Eudic dictionary on macOS by providing ultra-fast **Oxford Advanced Learner_s Dictionary 9th lookup**, **hotkey-based word search**, and **instant American/British pronunciation**.
This project was created with the help of an AI assistant.
Designed for English learners, writers, translators, and anyone who uses **Eudic (欧路词典)** regularly and wants a smooth keyboard-driven workflow.

---

## ✨ Features

### 🔍 1. Fast Oxford Lookup
- Type a keyword (`e yourword`) in Alfred to instantly open Eudic and show the Oxford entry.
- Supports custom keyword.

### ⌨️ 2. Lookup Selected Text
- Select any text in macOS  
- Press a hotkey (⌥⌘E or ??? depending on your setup)  
- Automatically sends the selected word to Eudic and opens the Oxford definition.

### 🔊 3. Instant Pronunciation (AmE & BrE)
- **⌥⌘A** — play American English (AmE) pronunciation of the word you look up in Eudic.
- **⌥⌘D** — play British English (BrE) pronunciation  of the word you look up in Eudic.
- **⌥⌘V** — Works anywhere: browser, PDF, IDE, documents.A way to instantly hear the American English(AmE) pronunciation of a word by selecting it anywhere on the screen.

### ⚡ 4. Fully AppleScript-Based
- Uses both `osascript` and `NSAppleScript` for low-latency interaction.  
- Compatible with the latest Eudic macOS versions.

---

## 📦 Installation

1. Download the latest `.alfredworkflow` file from:  
   👉 **Releases** page of this GitHub repository  

2. Double-click to import into Alfred.  

3. Make sure Alfred has permission to run AppleScript under:  
   **System Settings → Privacy & Security→ Automation**

4. To extract or "unpack" the contents of an MDict .mdd file :

   command example installing the utility:
   `pip install mdict-utils`
   commnad example extracting the resources:
   `mdict -x OALD9EnEn.mdd -d ./mdd` 

5. **"ATTENTION: Configuration is required for the pronunciation audio file path in all four scripts.**

   **Action:** You must **customize** the file path below to match your actual MDD resource location.

   **Line to Change:** `set dictRoot to "/Users/feeling/Library/Eudb_en/Oxford Advanced Learner_s Dictionary 9th_ By Amazon_ 2016.9.27/mdd/media/english/us_pron"`

   **Or Line to Change:** `set dictRoot to "/Users/feeling/Library/Eudb_en/Oxford Advanced Learner_s Dictionary 9th_ By Amazon_ 2016.9.27/mdd/media/english/uk_pron"`

   **Note:** Replace the path above with **your real pronunciation audio path**."

---

## 🧩 Hotkeys (Default)

| Action                  | Hotkey        | Notes                            |
| ----------------------- | ------------- | -------------------------------- |
| Lookup selected word    | ⌥⌘E           | Opens Eudic Oxford               |
| Pronounce selected word | ⌥⌘V           | Hear pronunciation globally      |
| Play AmE pronunciation  | ⌥⌘A           | Reads pronunciation inside Eudic |
| Play BrE pronunciation  | ⌥⌘D           | Reads pronunciation inside Eudic |
| Keyword lookup          | Alfred Hotkey | Type inside Alfred  `e yourword` |

You can customize all hotkeys inside Alfred.Please note that on macOS (including Tahoe or any other version), shortcut conflicts are primarily managed within individual applications and System Settings. Since there is no single tool to list all active global shortcuts, you need a systematic approach to find and fix them. For example, the shortcut Option+Command+D (⌥⌘D) conflicts with the system setting for **Turn Dock hiding on/off** (found under System Settings → Keyboard Shortcuts). To resolve this, simply double-click the conflicting shortcut and enter a new, unique key combination, or remove the shortcut entirely if you don't need it.

---

## 🛠 Requirements
- **macOS** (any modern version)  
- **Alfred 5**  
- **Eudic for Mac**  
- **Automation permission granted for Alfred & Eudic**
