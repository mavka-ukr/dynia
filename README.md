# Диня

Проста файлова база даних для Мавки. Зберігає у форматі Дід.

## Підключення

```мавка
взяти "хмарний.пак.укр/диня"
```

## Структура

```мавка
структура Диня
  шлях текст = "~/.данідині/спільне"
  тип щось = словник

  покласти(значення щось, місце текст або список) ніщо
  отримати(місце щось) щось
  видалити(місце щось) ніщо
кінець
```

## Використання

```мавка
взяти "хмарний.пак.укр/диня"

користувачі = диня.Диня("~/.данідині/спільне", словник)

леся = (
  місце=1,
  імʼя="Лариса",
  прізвище="Косач"
)

;; покласти значення в бд з ключем "1"
користувачі.покласти(леся)

;; отримати значення з бд за ключем "1"
леся_з_бд = користувачі.отримати(леся.місце)

;; видалити значення з бд за ключем "1"
користувачі.видалити(леся.місце)
```
