# Тестовый проект

## Знакомство с Markdown

Markdown - это специальный **язык разметки**.

1. Для того, чтобы было комфортнее узнать о проекте;
2. Придание красоты в оформлении файла README

Вот [пример](https://github.com/git/git/blob/master/README.md "Я пример!")

### Пример кода Python

```Python
def encrypt(s, n):
    result = ""
    for c in s:
        if 65 <= ord(c) <= 90:
            result += chr((ord(c) + n - 65) % 26 + 65)
        elif 97 <= ord(c) <= 122:
            result += chr((ord(c) + n - 97) % 26 + 97)
        elif 1040 <= ord(c) <= 1071:
            result += chr((ord(c) + n - 1040) % 32 + 1040)
        elif 1072 <= ord(c) <= 1103:
            result += chr((ord(c) + n - 1072) % 32 + 1072)
        else:
            result += c
    return result
```