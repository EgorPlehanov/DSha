# Теория Демпстера-Шейфера — прототип практической реализации

[![Python](https://img.shields.io/badge/Python-3.13.5-blue)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## RU

### Статус

**Прототип / активная исследовательская разработка**.

### О проекте

Этот репозиторий содержит исследовательский прототип консольного приложения по теории Демпстера‑Шейфера на основе примеров из книги Л.В. Уткина «Анализ риска и принятие решений при неполной информации».

Реализованы:

- базовые вероятностные назначения (BPA);
- функции доверия (Bel) и правдоподобия (Pl);
- правило комбинирования Демпстера;
- правило комбинирования Ягера;
- визуализация результатов.

### Авторы и роли

- **Основной разработчик:** Егор Сергеевич Плеханов, студент магистратуры.
- **Вторичный разработчик и научный руководитель:** Владимир Андреевич Пархоменко, старший преподаватель.
- **Аффилиация:** Федеральное государственное автономное образовательное учреждение высшего образования «Санкт-Петербургский политехнический университет Петра Великого», Институт компьютерных наук и кибербезопасности, Санкт-Петербург, Россия.

### Отказ от ответственности

Репозиторий содержит исследовательский прототип.
Программное обеспечение предоставляется «как есть» ("as is") без каких-либо явных или подразумеваемых гарантий,
включая, но не ограничиваясь, гарантиями коммерческой пригодности, пригодности для конкретной цели
и отсутствия нарушений прав. Авторы не несут ответственности за любые претензии, ущерб
или иные последствия, возникшие при использовании программного обеспечения.

### Быстрый старт

1. **Клонируйте репозиторий:**

```bash
git clone https://github.com/your-username/dempster-shafer-theory.git
cd dempster-shafer-theory
```

2. **Создайте виртуальное окружение:**

```bash
python -m venv dempster_venv
```

3. **Активируйте окружение:**

- Windows:

```bash
dempster_venv\Scripts\Activate
```

- Linux/Mac:

```bash
source dempster_venv/bin/activate
```

4. **Установите зависимости:**

```bash
pip install -r requirements.txt
```

5. **Запустите программу:**

```bash
python main.py
```

### Реализованные примеры

- **Пример 2.1:** кандидаты на должность (базовые BPA/Bel/Pl и визуализация интервалов неопределенности).
- **Пример 2.2:** прогноз цен акций (работа с интервальными данными и дискретизация непрерывной области).
- **Пример 2.6:** комбинирование свидетельств (правило Демпстера и коэффициент конфликта).
- **Пример 2.8:** правило Ягера (альтернативный подход к комбинированию).

### Структура проекта

- `main.py` — главный файл приложения и консольное меню.
- `dempster_core.py` — ядро вычислений теории Демпстера‑Шейфера.
- `examples.py` — сценарии примеров из учебного материала.
- `visualizer.py` — построение графиков и визуализация результатов.
- `data_adapters/` — адаптеры для загрузки входных данных (CSV/JSON и др.).
- `data/` — данные примеров и конфигурации выбора источников.
- `tests/` — тесты адаптеров данных и скрипт запуска тестов.
- `document/` — сопроводительные материалы (текст и презентация).
- `SETUP.md` — дополнительная инструкция по настройке окружения.

### Технологии

- Python 3.13.5
- Matplotlib
- NumPy
- Pandas
- Seaborn

### Теоретическая основа

Проект основан на материалах главы 2 книги:
**Л.В. Уткин «Анализ риска и принятие решений при неполной информации»**.

### Лицензия

Проект распространяется под лицензией **MIT**. Полный текст лицензии находится в файле [LICENSE](LICENSE).

---

## EN

### Status

**Prototype / In active research**.

### About

This repository contains a research prototype of a command-line application for Dempster–Shafer theory, based on examples from L.V. Utkin’s book on risk analysis and decision-making under incomplete information.

Implemented features:

- basic probability assignments (BPA);
- belief (Bel) and plausibility (Pl) functions;
- Dempster’s combination rule;
- Yager’s combination rule;
- result visualization.

### Authors and roles

- **Main developer:** Egor Sergeevich Plekhanov, master’s student.
- **Secondary developer and supervisor:** Vladimir Andreevich Parkhomenko, senior lecturer.
- **Affiliation:** Peter the Great St. Petersburg Polytechnic University, Institute of Computer Science and Cybersecurity, Saint Petersburg, Russia.

### Disclaimer

Disclaimer: This repository contains a research prototype.
The software is provided "as is", without warranty of any kind, express or implied,
including but not limited to the warranties of merchantability, fitness for a particular
purpose, and noninfringement. The authors are not liable for any claim, damages,
or other liability arising from the use of the software.

### Quick start

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/dempster-shafer-theory.git
cd dempster-shafer-theory
```

2. **Create a virtual environment:**

```bash
python -m venv dempster_venv
```

3. **Activate the environment:**

- Windows:

```bash
dempster_venv\Scripts\Activate
```

- Linux/Mac:

```bash
source dempster_venv/bin/activate
```

4. **Install dependencies:**

```bash
pip install -r requirements.txt
```

5. **Run the application:**

```bash
python main.py
```

### Implemented examples

- **Example 2.1:** job candidates (basic BPA/Bel/Pl and uncertainty interval plots).
- **Example 2.2:** stock price forecast (interval data processing and discretization of a continuous domain).
- **Example 2.6:** evidence combination (Dempster’s rule and conflict coefficient).
- **Example 2.8:** Yager’s rule (alternative combination approach).

### Project structure

- `main.py` — application entry point and console menu.
- `dempster_core.py` — core Dempster–Shafer computations.
- `examples.py` — runnable scenarios from the learning material.
- `visualizer.py` — plotting and visualization utilities.
- `data_adapters/` — input adapters (CSV/JSON, etc.).
- `data/` — example datasets and source selection configuration.
- `tests/` — adapter tests and test runner.
- `document/` — supporting documents (text and slides).
- `SETUP.md` — additional environment setup instructions.

### Technologies

- Python 3.13.5
- Matplotlib
- NumPy
- Pandas
- Seaborn

### Theoretical foundation

The project is based on Chapter 2 of:
**L.V. Utkin, “Risk Analysis and Decision Making under Incomplete Information.”**

### License

This project is distributed under the **MIT** License. See [LICENSE](LICENSE) for the full text.
