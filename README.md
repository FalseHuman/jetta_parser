# Jetta Chemical Parser

Парсер для сбора данных о товарах с сайта Jetta Chemical (https://jetta-chemical.ru).

## Возможности

- Парсинг всех категорий и подкатегорий
- Сбор информации о товарах:
  - Название
  - Цена
  - Валюта
  - Фасовка
  - Минимальный заказ
  - URL
- Автоматическое сохранение данных в Excel файл
- Логирование процесса парсинга

## Требования

- Python 3.8+
- Chrome браузер
- Установленные зависимости из requirements.txt

## Установка

1. Клонируйте репозиторий:
```bash
git clone https://github.com/FalseHuman/jetta_parser.git
cd jetta_parser
```

2. Создайте виртуальное окружение и активируйте его:
```bash
python -m venv venv
source venv/bin/activate  # для Linux/Mac
venv\Scripts\activate     # для Windows
```

3. Установите зависимости:
```bash
pip install -r requirements.txt
```

## Использование

1. Запустите парсер:
```bash
python jetta_parser.py
```

2. Результаты будут сохранены в Excel файл с именем вида `jetta_products_YYYYMMDD_HHMMSS.xlsx`

## Структура проекта

```
jetta_parser/
├── jetta_parser.py    # Основной скрипт парсера
├── requirements.txt   # Зависимости проекта
├── .gitignore        # Игнорируемые файлы Git
└── README.md         # Документация проекта
```

## Логирование

Все действия парсера логируются в консоль и соответствующий файл с указанием времени и уровня сообщения.

## Лицензия

MIT 