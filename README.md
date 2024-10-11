
# EN
**GenShellFinder** is a high-performance, multi-threaded tool designed to scan web servers for known vulnerable shell files. It automates the process of finding common web shells by searching through various paths. The tool is optimized for parallel execution using Python's multiprocessing capabilities, allowing for efficient scanning of multiple targets.

## Features
- **Multi-threading:** Efficiently scan multiple URLs simultaneously.
- **Extensive Shell Path List:** Built-in list of known vulnerable shell paths for detection.
- **Customizable:** Easily edit the list of shell paths to adapt to new vulnerabilities.
- **Cross-platform:** Works on both Windows and Linux systems.
- **Color-coded Output:** Provides a clear and colorful console output for better readability.

## Installation

```bash
# Clone the repository
git clone https://github.com/geniuszly/GenShellFinder

# Navigate to the project directory
cd GenShellFinder

# Install dependencies
pip install -r requirements.txt
```

## Usage

1. Prepare a list of target websites in a text file (one URL per line).
2. Run the scanner using the following command:

```bash
python GenShellFinder.py
```

You will be prompted to:
- Provide the path to the file with the list of websites.
- Specify the number of threads to use for scanning.

## Example
```bash
Website List: targets.txt
Threads: 10
```

```
--------------------------------------------------
 Добро пожаловать в GenShellFinder!
 Программа поможет найти уязвимые пути к шеллам.
--------------------------------------------------

Введите путь к файлу со списком сайтов: targets.txt
Введите количество потоков: 10

[*] >> = http://example.com/uploads/shell.php
[*] >> = http://another-example.com/admin/leaf.php
[*] >> = http://test-website.com/priv.php
[*] >> = http://example-test.com/c99.php

[!] 10 URLs просканировано.
[+] 4 шелла найдено.
```

The results will be displayed directly in the console. Found shells will be logged in the `found_shells.txt` file.

## Requirements
- Python 3.x
- Required libraries:
  - `requests`
  - `colorama`
  - `multiprocessing`


# RU
**GenShellFinder** — это высокопроизводительный многопоточный инструмент для сканирования веб-серверов на предмет известных уязвимых файлов шеллов. Программа автоматизирует процесс поиска общих веб-оболочек, сканируя различные пути. Инструмент оптимизирован для параллельного выполнения с использованием возможностей многопроцессорности Python, что позволяет эффективно сканировать несколько целей.

## Особенности
- **Многопоточность:** Эффективное сканирование нескольких URL одновременно.
- **Обширный список путей шеллов:** Встроенный список известных уязвимых путей шеллов для обнаружения.
- **Настраиваемость:** Легко редактировать список путей для адаптации к новым уязвимостям.
- **Кроссплатформенность:** Работает как на Windows, так и на Linux.
- **Цветной вывод:** Обеспечивает четкий и цветной вывод в консоли для улучшения читаемости.

## Установка

```bash
# Клонируйте репозиторий
git clone https://github.com/geniuszly/GenShellFinder

# Перейдите в директорию проекта
cd GenShellFinder

# Установите зависимости
pip install -r requirements.txt
```

## Использование

1. Подготовьте список целевых сайтов в текстовом файле (один URL на строку).
2. Запустите сканер с помощью следующей команды:

```bash
python GenShellScanner.py
```

Программа запросит:
- Путь к файлу со списком сайтов.
- Количество потоков для сканирования.

## Пример
```bash
Website List: targets.txt
Threads: 10
```

```
--------------------------------------------------
 Добро пожаловать в GenShellFinder!
 Программа поможет найти уязвимые пути к шеллам.
--------------------------------------------------

Введите путь к файлу со списком сайтов: targets.txt
Введите количество потоков: 10

[*] >> = http://example.com/uploads/shell.php
[*] >> = http://another-example.com/admin/leaf.php
[*] >> = http://test-website.com/priv.php
[*] >> = http://example-test.com/c99.php

[!] 10 URLs просканировано.
[+] 4 шелла найдено.
```

Результаты будут отображены прямо в консоли. Найденные шеллы будут записаны в файл `found_shells.txt`.

## Требования
- Python 3.x
- Необходимые библиотеки:
  - `requests`
  - `colorama`
  - `multiprocessing`

