# Dynasty Warriors 5 Tools

**Python tools for reading, editing, and analyzing data from Dynasty Warriors 5, XL, and Empires.**

This collection includes scripts to extract game data, edit unit stats, and explore binary formats used by the game’s resource files. The goal is to support modders and researchers working with DW5 file formats.

---

## Screenshots

Example Mod (turns Zhao Yun into a Tiger with the needed data to function properly):  
<img src="https://github.com/user-attachments/assets/f6e2c003-6445-4c22-8999-e5cecb137c81" width="800" />

Tool Overview Screenshot:  
<img src="https://github.com/user-attachments/assets/1f7b97c1-82a4-4190-8df6-2f647ad6c219" width="800" />

---

## Features

- Tools for extracting and repacking data files  
- Unit data editors (GUI and CLI)  
- Support for multiple DW5 versions (Base, XL, Empires)  
- Pure Python; no compiled dependencies  

---

## Prerequisites

1. Python 3.10 or later  
   Check your version with:
   ```sh
   python --version
   ```

2. Optional virtual environment (recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate   # macOS/Linux
   .\venv\Scripts\activate    # Windows
   ```

---

## Installation

Clone the repository:
```sh
git clone https://github.com/Luvvydev/Dynasty-Warriors-5-Tools.git
cd Dynasty-Warriors-5-Tools
```

Install dependencies:
```sh
pip install -r requirements.txt
```

If there is no `requirements.txt`, install dependencies as needed by the tool you run.

---

## Usage

### Extract LZP2 Files

Unpack compressed game assets (works on multiple language versions):
```sh
python lzp2Extract.py /path/to/input.lzp2 /path/to/output_dir
```

### Unit Data Editor

Start the GUI editor:
```sh
python DW5XLE_UNITTOOL.pyw
```

Load the game’s data directory when prompted. Edit values and save files back when done.

---

## Supported Game Versions

- Dynasty Warriors 5 (Base)  
- Dynasty Warriors 5 XL  
- Dynasty Warriors 5 Empires

The tools are tested with PC versions; functionality on console dumps may vary.

---

## Troubleshooting

Python script not found or permission denied  
Ensure you are in the correct working directory and Python is installed and on your PATH.

Tool crashes on certain files  
Some file formats are reverse-engineered. If a format isn’t supported, the script may fail. Consider opening an issue with sample data so support can be improved.

---

## Contributing

Contributions are welcome. Please follow these steps:

1. Fork the repository.  
2. Create a feature branch:
   ```sh
   git checkout -b feature-name
   ```
3. Commit your changes.
4. Push to your fork:
   ```sh
   git push origin feature-name
   ```
5. Open a Pull Request against this repository’s `main` branch.

Before submitting a Pull Request, make sure:
- Your code is well documented.
- You update the README if the interface changed.

---

## License

This project uses the MIT License (or whatever license is present in the repository). See the `LICENSE` file for details.

---

## Acknowledgments

- Based on original tools and reverse engineering efforts from the community.  
- Credits to all contributors who improved file format support.
