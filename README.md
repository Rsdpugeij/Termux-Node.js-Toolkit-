# **Termux-Node.js Toolkit** 📱⚡  
**Run Node.js servers, bots, and scripts natively on Android via Termux with zero setup.**  

## **✨ Key Features**  

- **One-Command Setup**  

  ```bash
  curl -sL https://git.io/termux-node | bash
  ```

  - **Pre-Configured for Android**
 
      - ARM-optimized builds of Node.js (v18+/LTS)
   
      - Fixes for filesystem/permission issues in Termux
   
      - Background service management (`termux-job-scheduler`)

     **Batteries Included**

      - Pre-installed: `express`, `socket.io`, `node-fetch`, `termux-api`
   
          - Android-specific modules:
       
          - SMS/call handling (`termux-sms-listener`)
       
          - Device sensors (GPS, accelerometer via `termux-sensor`)
       
          - Notifications (`termux-notification`)

### **🚀 Use Cases**  

- Host local dev servers on your phone

- Build Android automation scripts (e.g., auto-reply bots)

- IoT gateway using your phone’s sensors

- Offline-first apps with Termux’s isolated environment

### **📦 Quick Start**  

1. Install:  
   ```bash
   pkg install git -y && git clone https://github.com/your-repo/termux-node.git  
   cd termux-node && ./install.sh
   ```

2. Run a demo:  
   ```bash
   node examples/http-server.js  # Serves on localhost:3000
   ```

### **🛠️ Compatibility**  

- **Termux** (F-Droid build recommended)

- **Node.js** v16+ (ARM64/ARMv7)

- **Android 9+** (no root required)

---
### **🌟 Why Developers Love This**  

- **No Emulation**: Native ARM builds = better performance than Docker/QEMU.

- **Android Integration**:  
  ```javascript
  const termux = require('termux-api');
  termux.vibrate({ duration: 100 });  // Vibrate phone via JS!
  ```

  - **Zero Config**: Fixes common Termux issues (e.g., `ENOENT` errors).


---

### **🤝 Contributing** 

PRs welcome for:  

- More Android API wrappers

- Performance benchmarks

- Termux-X11 GUI examples

**Star ⭐ if you’ve used this to hack something cool on mobile!**  

--- 
