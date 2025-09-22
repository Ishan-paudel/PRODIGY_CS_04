# PRODIGY_CS_04
# Python Keylogger

## Project Overview
This is a simple **Python keylogger** that captures keystrokes and logs them into a text file. It demonstrates fundamental **event handling** and **file I/O** using the `pynput` library. The project is intended strictly for **educational purposes** on devices you own or have explicit permission to use.

## Features
- **Keystroke Logging:** Captures letters, numbers, and special keys like Space, Enter, Shift, and Ctrl.  
- **Persistent Storage:** Appends all logged keys to `log.txt`.  
- **Lightweight and Simple:** Minimal code for understanding basic Python I/O and event handling.  

## Technology Stack
- **Python 3** – Core programming language.  
- **pynput** – Python library to monitor keyboard events.  

## How It Works
1. A `Listener` from `pynput.keyboard` monitors keyboard events.  
2. Each key press triggers the `write_to_file` function.  
3. The key is processed and formatted, replacing special keys (like Space or Enter) with readable characters.  
4. Keystrokes are appended to `log.txt` for persistent storage.  
5. The listener runs continuously until manually stopped, ensuring memory is properly released via Python’s `with` statement.  

## Usage
1. Install dependencies:
   ```bash
   pip install pynput

