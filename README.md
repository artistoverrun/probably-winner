# XAUT Tactical Trading Bot

A tactical trading bot for XAUT, built in Python.

---

## ✅ Setup Instructions

### 1. Python Version
- **Recommended:** Python 3.9 or higher

### 2. Create Virtual Environment
```sh
python3 -m venv xaut_env
source xaut_env/bin/activate
```

### 3. Install Dependencies
If no `requirements.txt` exists, run:
```sh
pip install pandas requests schedule python-dotenv openpyxl
pip freeze > requirements.txt
```
Or install directly if file exists:
```sh
pip install -r requirements.txt
```

### 4. Environment Variables
Create a `.env` file in the root directory with necessary values. Example:
```
API_KEY=your_api_key
FOLDER_PATH=/absolute/path/to/input
OUTPUT_PATH=/absolute/path/to/output.xlsx
```

### 5. Directory Setup
Ensure paths referenced in `.env` exist:
- **Input folder** (for data files)
- **Output folder** (for result files or logs)

### 6. Run the Bot
```sh
python xaut_tactical_bot.py
```

### 7. Optional: Background Execution
```sh
nohup python xaut_tactical_bot.py &
```

### 8. Optional: Scheduling (cron example)
```sh
crontab -e
```
Add:
```
0 6 * * * /full/path/to/xaut_env/bin/python /full/path/to/xaut_tactical_bot.py
```

---

## 📂 Project Structure (Example)
```
probably-winner/
├── xaut_tactical_bot.py
├── requirements.txt
├── .env
├── input_folder/
└── output_folder/
```

---

## 🚀 Notes
- Review your `.env` file for accuracy.
- Make sure your input and output directories exist.
- For detailed configuration, see comments in `xaut_tactical_bot.py`.

---

Happy Trading!
