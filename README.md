## Virtual Display Driver Python Control GUI

![image](https://github.com/user-attachments/assets/b6666055-ac03-4e88-aeea-3b3a5150593d)


This Python script provides a GUI to send commands to the Virtual Display Driver via a named pipe. It allows users to input and send commands, receive responses, and reconnect to the pipe if needed.

### Features

- **Command Entry:** Send commands to the Virtual Display Driver.
- **Reconnect Button:** Re-establish connection to the named pipe.
- **Log Window:** Displays sent commands and received responses.
- **Error Handling:** Alerts for failed connections and invalid inputs.

---

## Prerequisites

This script requires the following dependencies:

- **Python 3.x**
- **Tkinter** (built-in with Python)
- **pywin32** (for Windows named pipes)

To install pywin32, run:

```sh
pip install pywin32
```

---

## Installation

1. **Ensure dependencies are installed** (see prerequisites).

2. **Run the script**:

   ```sh
   python MTTVirtualDisplayPipe.py
   ```

---

## Usage

### Connecting to the Pipe
Upon launching, the application will attempt to connect to the named pipe:

```plaintext
\\.\pipe\MTTVirtualDisplayPipe
```

If the connection is successful, the log will display:

```plaintext
Connected to the Virtual Display Driver pipe.
```

If it fails, an error message will appear.

### Sending Commands
1. Enter a command in the **Command** field.
2. Click **Send Command** to send it.
3. The log will display the sent command and any response.

### Reconnecting to the Pipe
If the connection is lost:
1. Click **Reconnect** to attempt reconnection.
2. A status message will appear in the log.
