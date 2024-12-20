# Подготовка данных для модели обнаружения отходов

|  [English](README_en.md)  |  Русский  |

Этот модуль отвечает за подготовку и предварительную обработку данных для обучения модели обнаружения отходов на конвейерной ленте.

### Основные функции 

1. **Установка и импорт библиотек**
   - Установка необходимых пакетов (opencv-python, pyyaml, albumentations)
   - Импорт всех требуемых библиотек для работы с данными

2. **Загрузка и анализ данных**
   - Создание структуры директорий для организации данных
   - Загрузка обучающего (train.csv) и тестового (test.csv) наборов данных
   - Анализ распределения классов в данных
   - Визуализация распределения классов

3. **Функции обработки данных**
   - Реализация функций для oversampling несбалансированных классов
   - Функции для аугментации изображений (изменение яркости, контраста, размытие)

4. **Подготовка и сохранение данных**
   - Применение oversampling для балансировки классов
   - Аугментация изображений для увеличения разнообразия данных
   - Сохранение обработанных изображений и аннотаций

5. **Архивация данных**
   - Создание архива с подготовленным датасетом
   - Сохранение архива для дальнейшего использования

### Используемые библиотеки

- `pandas`: обработка структурированных данных
- `matplotlib`: визуализация данных
- `random`: генерация случайных чисел
- `cv2` (opencv-python): обработка изображений
- `os`: работа с файловой системой
- `ast`: обработка Python литералов
- `numpy`: численные вычисления
- `sklearn.model_selection`: разделение данных на train/test
- `shutil`: операции с файлами и директориями
- `pathlib`: работа с путями файловой системы
- `albumentations`: аугментация данных
- `zipfile`: работа с ZIP архивами

### Установка библиотек 

```bash
pip install opencv-python
pip install pyyaml
pip install albumentations
pip install -r requirements.txt
```

### Использование

1. Убедитесь, что все необходимые библиотеки установлены:
   ```bash
   pip install -r requirements.txt
   ```

2. Откройте ноутбук `load-data.ipynb` в Jupyter Notebook или JupyterLab

3. Следуйте инструкциям в ноутбуке для:
   - Настройки путей к данным
   - Выполнения предварительной обработки
   - Анализа распределения данных

### Структура данных 

```
├── load-data.ipynb      # основной ноутбук для обработки данных
├── requirements.txt     # список зависимостей проекта
├── README_en.md         # документация на английском языке
└── README_ru.md         # документация на русском языке (этот файл) 

*Примечание: Исходный датасет и обработанные данные не включены в репозиторий.*
```

### Примечания

- Убедитесь, что пути к данным настроены правильно
- Рекомендуется использовать GPU для ускорения обработки
- При добавлении новых данных, следуйте той же структуре организации файлов
