# SimpleLogs
SimpleLogs is a lightweight and easy-to-use open-source library for creating logs with customizable colors in Python. Ideal for developers looking to simplify tracking and debugging in their projects.

- Colored log messages.
- Different log levels (`INFO`, `WARNING`, `ERROR`, `TRACE`).
- Optional: Display the line of code where the message was generated.

## Installation
First, clone this repository and add SimpleLogs to your project:

```bash
git clone https://github.com/Pabl0VC/simpleLogs.git
# /simpleLogs/ Add this folder to your project. Ideally in /modules/
```
If you are using a virtual environment, make sure to activate it and install the requirements:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Basic Usage
Import SimpleLogs into your project:
```python
from simpleLogs import info, warning, error, trace

info("Information message")
warning("Warning message")
error("Error message")
trace("Debug message")
```

If you want to include information about the line where the message was generated, use the functions with the L suffix:

```python
from simpleLogs import infoL, warningL, errorL, traceL

infoL("Information with line number")
```

## Features
- Customizable colors: Each log level has a unique color for easier visual identification.
- Enriched format: Displays the date, time, and optionally the line of origin.
- Lightweight and easy to integrate: Ideal for both large and small projects.
- Support for advanced levels: Includes traceability (trace) for detailed debugging.
- Easy integration: Designed to be a quick and simple replacement for print().

## Supported Log Levels
SimpleLogs supports the following log levels, each with custom colors for better visibility:

| Level      | Description                              | Variants               |
|------------|------------------------------------------|-------------------------|
| **INFO**   | Informational messages.                  | `info`, `infoL`         |
| **WARNING**| Warnings about potential issues.   | `warning`, `warningL`   |
| **ERROR**  | Critical error messages.             | `error`, `errorL`       |
| **TRACE**  | Detailed debugging messages.      | `trace`, `traceL`       |

## Images
![alt text](/examples/example_terminal.png)

### Real Examples
![alt text](/examples/real_ex.png)

## Requirements
- Python 3.7 or higher
- colorama

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
Created by Pablo Vega Castro. If you have any questions or suggestions, feel free to contact me at pablovegac.93@gmail.com.