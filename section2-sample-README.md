# ResearchLogger

![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20Windows-lightgrey)

![License](https://img.shields.io/badge/license-MIT-green)

An academic research tool for logging keyboard and mouse activity during writing process studies.

ResearchLogger extends the open-source **PyKeylogger** project and is designed for controlled experimental environments.

> ⚠️ This software is intended strictly for research and academic purposes. Misuse may violate privacy laws in your jurisdiction.

---

## Overview

ResearchLogger captures and records:

- Keyboard activity  
- Mouse clicks  
- Timed screenshots  
- Contextual click-area images  

It is particularly suited for:

- Writing process analysis  
- Translation studies  
- Behavioral research  
- Human-computer interaction experiments  

---

## Features

- Portable execution  
- Detailed keystroke logging  
- Timed screenshot capture  
- Click-area image capture  
- Optional graphical interface (GUI)  
- Structured experiment output  

---

## Project Structure

| Folder | Purpose |
|--------|----------|
| `click_images/` | Screenshots around click events |
| `detailed_log/` | Full keystroke activity log |
| `system_log/` | System errors and activity records |
| `timed_screenshots/` | Periodic full-screen captures |

---

## Installation

### Requirements

- [x] Python 3.x  
- [ ] Linux (Ubuntu/Debian recommended) or Windows XP/7  

---

### Linux Dependencies

```bash
sudo pip install validate
sudo apt-get install python-xlib
sudo apt-get install python-pil
sudo apt-get install python-gtk2
```

---

## Usage

### Run Without GUI

#### Start the keylogger

```bash
python ResearchLogger.py
```

#### Start the translation window only

```bash
python ResearchLoggerInterface.py -d YOUR_CHOSEN_PATH
```

If no directory is specified:

```bash
python ResearchLoggerInterface.py
```

By default, output is saved in the current directory.

---

### Stop the Keylogger

Press:

```text
CTRL (left) + CTRL (right) + F12
```

Then navigate to:

**Actions → Quit**

_Default password: empty_

---

### Run With GUI

Start the interface:

```bash
python ResearchLoggerInterface.py
```

1. Enter subject name  
2. Select experiment source text  
3. Run session  
4. Close window using the `X` button  

#### Screenshots

- Enter the subject name

![Insert Subject](https://github.com/roxana-lafuente/ResearchLogger/raw/master/images/insert_subject_window.png)  

- Select the text of the experiment you are running.

![Load Source Text](https://github.com/roxana-lafuente/ResearchLogger/raw/master/images/load_source_text_window.png)  

- Then the window opens and, once the subject is finished with the task, the window can be closed by using the X button.

![Translation Window](https://github.com/roxana-lafuente/ResearchLogger/raw/master/images/translation_window.png)

---

## Output Details

ResearchLogger generates structured experiment data.

### Generated Data Includes:

- Session start and end timestamps  
- Final produced text  
- Complete keystroke registry  
- Mouse interaction images  
- Timed screenshots  

---

## Important Notes

> The GUI does **not** automatically start the keylogger.

You must run `ResearchLogger.py` separately.

Failure to do so will result in no keystroke logging.

---

## Ethical Considerations

This tool records user input and screen activity.

Before use:

- Obtain informed consent  
- Follow institutional research policies  
- Comply with local data protection laws  

Example of informed consent clause:

> Participants acknowledge that keyboard and mouse activity will be recorded for research purposes.

---

## Example Workflow

1. Start keylogger  
2. Launch GUI  
3. Select subject  
4. Run experiment  
5. Stop session  
6. Export results  

---

## Supported Platforms

- Linux (Ubuntu / Debian)  
- Windows XP / 7  

> Modern Windows/macOS support may require additional configuration.

---

## Research Use Case Example

Water molecule notation: H~2~O  
Einstein equation reference: E = mc^2^  

These formatting examples demonstrate Markdown subscript and superscript rendering.

---

## Version History

### v2.0
- Migrated to Python 3
- Improved logging performance

### v1.0
- Initial academic release
- ~~Python 2.7 support~~ (deprecated)
- ~~Experimental macOS support~~ (removed due to instability)

---

## 📜 License

MIT License © 2026 ResearchLogger Contributors[^1]

[^1]: ResearchLogger builds upon the original PyKeylogger project.