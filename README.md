# Diplom_3
# UI tests — Stellar Burgers

## Запуск
```bash
# установка
python -m venv venv
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt

# один браузер
pytest --browser chrome
pytest --browser firefox

# оба браузера
pytest --browser all

# headless
pytest --browser all --headless

# Allure
pytest --browser all --alluredir=allure-results
allure generate allure-results -o allure-report --clean
start allure-report\index.html
