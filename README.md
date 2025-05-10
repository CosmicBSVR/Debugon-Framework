# 🔧 Debugon - In-Game Debug Console for Unity

**Debugon** is a lightweight, extensible in-game debug console for Unity, built to help developers view logs, run commands, and debug gameplay in real time. It's designed to be highly modular and easy to integrate into any Unity project.

---

## ✨ Features

- 📜 **Log Console UI** – View logs in-game with support for rich text, color tags, scroll view, and more.
- ⌨️ **Command Input Field** – Enter custom commands while the game is running.
- 🧱 **Prefab-Based UI** – Easily customizable using a single prefab.
- 🧠 **Smart Logging** – Works with `Debug.Log`, `Debug.LogWarning`, `Debug.LogError`, and the custom `DebugonLogger`.
- 🧩 **Modular Design** – Separated into Console, UI, Events, and Extensions for better maintainability.
- 📦 **No Setup Required** – Add from the Unity Editor menu in seconds.

---

## 🚀 Quick Start

1. ✅ Import the Debugon package into your project.
2. 🧱 Use the Unity top menu:  
   `GameObject > Debugon > CreateFullConsole`
3. 🎮 Press Play and start logging:
```csharp
DebugonLogger.Log("Hello from <color=green>Debugon</color>!");
🧩 Components
DebugonConsole – Handles log history and interaction.

DebugonUI – Manages references to UI elements (Text, InputField, ScrollRect).

DebugonEvents – Extensible event system for registering custom commands.

DebugonFullConsole – Auto-wires everything together using a prefab.

🧠 Rich Text & Colors
TextMeshPro supports rich text, so you can color your logs:
DebugonLogger.Log("<color=yellow>[WARNING]</color> This is a highlighted message!");
📂 Project Structure
Assets/
└── Debugon/
    ├── DebugonCore/
    ├── UI/
    │   └── Debugon_Full_Console.prefab
    └── Scripts/
🛠 Dependencies
Unity 2021.3+ or newer

TextMeshPro (TMP) must be installed and enabled in the project

📄 License
MIT License — free to use in personal or commercial projects.

❤️ Credits
Created with 💡 by [CosmicBSVR].
Feel free to contribute or suggest improvements!