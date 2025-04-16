# About
This code is a **basic keylogger** that records all keystrokes typed by the user and logs them into a file (`keylog.txt`). It uses the `pynput` library to listen for both standard and special key presses.

---

## Risk
The script poses a significant **security and privacy risk**:
- It captures **all keystrokes**, including passwords, credit card details, and sensitive information.
- The logged data is stored in plaintext (`keylog.txt`), making it easily accessible to an attacker.
- Keyloggers are commonly used in cyberattacks, including credential theft and espionage.

---

## Code Block
### Key Components That Enable Keystroke Logging:
1. **`on_press(key)`**  
   - Captures each keystroke as it is pressed.  
   - Logs alphanumeric characters directly.  
   - Handles special keys separately (e.g., `Enter`, `Shift`, `Ctrl`).  

2. **`on_release(key)`**  
   - Detects when a key is released.  
   - Terminates logging when the `Escape (ESC)` key is pressed.  

3. **`Listener` from `pynput.keyboard`**  
   - Runs in the background, continuously recording keypresses.  
   - Starts listening when the script is executed and stops upon `ESC`.  

---

## Notes
This script is for **educational and ethical research purposes only**. Unauthorized use of keyloggers **violates privacy laws** and **can lead to legal consequences**. If used in penetration testing, ensure that you have explicit permissions from the target.

Extreme caution is advised when using or modifying this code.
