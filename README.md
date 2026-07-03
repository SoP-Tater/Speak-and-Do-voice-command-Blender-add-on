# Speak and Do – Voice Command Add-on for Blender

**Speak and Do** lets you control Blender with your voice. Speak natural words or custom phrases and execute modeling, sculpting, and editing operations instantly. Includes full support for alias mapping, fuzzy phrase recognition, and offline dependency installation.

---

## 🧰 Features

- 🎙️ Execute Blender operators via spoken commands
- 🔁 Record your own custom aliases (in any language or phrasing)
- 🧠 Fuzzy matching allows close-sounding phrases to still trigger the correct action
- 💡 Works across Object Mode, Edit Mode, and Sculpt Mode
- 📁 Filter and scroll through stored voice mappings by category and mode
- 🧩 Includes bundled dependencies—installs without internet access
- 🔄 Mic hotkey support (press semicolon to activate speech input)

---

## 🚀 Installation

1. Download the `.zip` package (do not extract it).
2. In Blender:
   - Go to `Edit → Preferences → Add-ons`
   - Click **Install**
   - Select the `.zip` file and click **Install Add-on**
   - Enable **Speak and Do** in the list
3. Optional: Click **“Load Default Library”** to preload default voice mappings

---

## 🎤 How to Use

### Speak a Command
1. Click the **Speech** button in the panel (or press **`;`**)
2. Speak a phrase like:
   - `"add cube"`
   - `"delete vertices"`
   - `"inset faces"`
3. If a match is found, it executes the corresponding Blender operator

---

## 🧩 Recording Custom Phrases (Aliases)

You can remap any operator to a phrase of your choosing.

### Option 1: **Record a Custom Phrase**
1. In the panel, select a Mode → Subcategory → Operator
2. Click **“Record Custom Phrase”**
3. Speak your phrase
4. The phrase will be stored in the current mode/category

### Option 2: **Manually Add an Alias**
1. Type your alias in the “Manual Alias” field
2. Click **Add**
3. The phrase will now trigger the selected operator

---

## 🔎 Managing Mappings

- Use the **arrow buttons** to scroll through mappings (only when Display Limit is set to a number like 2, 4, etc.)
- If Display Limit is set to **All**, all mappings are shown at once and you can scroll through them 
- If set to **None**, mappings are hidden


---

## 📦 Dependencies

The add-on comes with these prepackaged libraries:

- `speech_recognition` – for voice recognition (requires internet)
- `pyaudio` – for mic input
- `pynput` – for hotkey support
- `setuptools` – required by pip installer

They are automatically installed on first launch (offline-friendly).

---

## 🌐 Internet Usage

> The add-on installs without needing internet, **but** Google’s speech recognition requires a connection to recognize spoken phrases.

---

## 🛠 Troubleshooting

- **Mic not responding?**  
  Ensure your default input device is enabled and available to `pyaudio`.

- **“No phrase recognized” warning?**  
  Check if the mic is active. Try adjusting ambient noise or speaking more clearly.

- **Slow startup?**  
  This can happen during dependency install. Once installed, load time improves.

- **Command not found?**  
  Try recording a custom alias or check if the command is mapped in the current mode.

---

## 📄 Custom Data Files

User mappings are saved to:

user mappings are saved to;
C:\Users<YourName>\AppData\Roaming\Blender Foundation\Blender\4.2\scripts\speak_and_do.json
##If you wish to start with a clean slate then you can delete this file


You can also preload default mappings by clicking **Load Default Library** in the panel.

---

## 👤 Author

- Michael Crouse  

---

## 📜 License

This add-on is licensed under **GPL-3.0-or-later**  
Free to use, modify, and redistribute.
