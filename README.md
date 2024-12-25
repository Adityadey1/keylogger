# Keylogger using Python

This keylogger script logs all keystrokes typed by the user into a text file (keyfile11.txt). It leverages the pynput library to monitor keyboard input in real time.

How it works:
    1. Keyboard Listener:
    The program uses the keyboard.Listener class from the pynput module to detect and record every keypress.

    2. Key Logging:
    Each keypress is passed to the keyPressed function, which:
        Prints the key to the console for debugging purposes.
        Attempts to log the key's character into the file keyfile11.txt.
        Handles errors gracefully when a key doesn't have a character representation (e.g., special keys like Shift or Enter).

    3. Output File:
    The logged keystrokes are stored in the file keyfile11.txt in append mode. This ensures that no previous data is overwritten.

    4. Run the Program:
    The script starts the listener in the main block and waits for user input to keep running.
