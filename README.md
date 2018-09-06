# Задание на машиннное обучение

Дополнительных библиотек не требуется, написано на python 3.7

Параметры train.py:

* `--dir` или `-d` - путь к директории, в которой лежит коллекция документов. Если данный аргумент не задан, считать, что тексты вводятся из stdin.
* `--model` или `-m` - путь к файлу, в который сохраняется модель (в формате .pickle).

Параметры generate.py:

* `--model` или `-m` - путь к файлу, из которого загружается модель.
* `--seed` или `-s` - необязательный аргумент. Начальное слово. Если не указано, выбираем слово случайно из всех слов.
* `--length` или `-l` - длина генерируемой последовательности.

Пример:

python3 train.py --dir files --model main.pickle (обучение)

python3 generate.py --model main.pickle --seed через --lenght 20 (генерация)