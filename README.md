### Pyblish Tray

Pyblish accessible as a tray icon.

![untitled](https://cloud.githubusercontent.com/assets/2152766/10945772/d8da3474-8316-11e5-8eb0-8eb09e2321c0.gif)

<br>
<br>

### Usage

Tray is meant to be wrapped up into an executable and launched via a launcher native to the OS, such as double-clicking on its icon on Windows.

To run it as-is, such as for development, you can run it as an executable Python package.

```bash
$ python -m pyblish_tray
```

<br>
<br>

### Hotkeys

| Key      | Function
|:---------|:---------
| Ctrl+C   | Copy
| Ctrl+A   | Select all
| Ctrl+D   | Deselect all


<br>
<br>

### Features

**Current**

- Overall control over the Pyblish process
- Persistent, selectable console output
- Virtual host for testing and debugging

**Planned**

- Timestamp for console output
- Additional virtual host controls
 - Working directory
 - Environment
 - Settings
- Listing and manipulation of currently active hosts
- Listing of prior events
- Notification of events, via balloon popup

<br>
<br>

### Code Organisation

This project is written in Python 2.7, PyQt5 and QML and is organised as follows.

| Path                                | Description
|:------------------------------------|:---------------
| /pyblish_tray                       | Primary Python Package
| /pyblish_tray/app.py                | Main application
| /pyblish_tray/icon.ico              | Application icon
| /pyblish_tray/console.py            | Helpers for the visual console
| /pyblish_tray/virtual_host.py       | Helpers for the visual virtual host
| /pyblish_tray/qml                   | QML files
| /pyblish_tray/qml/Library           | User interface module for Tray
