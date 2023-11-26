# Диня

Проста файлова база даних для Мавки. Зберігає у форматі Дід.

## Підключення

```мавка
взяти "диня/0.1.0"
```

## Структура

```мавка
структура Диня
  шлях текст = "~/.данідині/спільне"
  тип щось = словник

  покласти(значення щось, місце текст або список = пусто) ніщо
  отримати(місце щось) щось
  видалити(місце щось) ніщо
кінець
```

## Використання

```мавка
взяти "диня/0.1.0"

користувачі = диня.Диня("./користувачі", словник)

леся = (
  місце=1,
  імʼя="Лариса",
  прізвище="Косач"
)

;; покласти значення в диню на місце "1"
користувачі.покласти(леся)

;; отримати значення з дині за місцем "1"
леся_з_дині = користувачі.отримати(1)
```
