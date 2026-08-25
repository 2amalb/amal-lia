# amal-lia.com — трекеры курса лечения

Статический сайт для GitHub Pages:

```
index.html        — главная (выбор: Амал / Лия)
amal/index.html   — трекер Амала  → amal-lia.com/amal
lia/index.html    — трекер Лии   → amal-lia.com/lia
CNAME             — привязка домена amal-lia.com
```

Отметки о приёме хранятся в localStorage браузера — у каждого устройства свои
(на телефоне Амала — его, на телефоне Лии — её). Бэкенд не нужен.

## Деплой (GitHub Pages)

1. Создать репозиторий (например `amal-lia`) и залить содержимое этой папки в корень ветки `main`.
2. В репозитории: **Settings → Pages → Source: Deploy from a branch → main / (root)**.
3. Там же в поле **Custom domain** вписать `amal-lia.com` (файл CNAME уже в репо) и включить **Enforce HTTPS** после выпуска сертификата.

## DNS у регистратора домена

| Тип   | Имя | Значение                |
|-------|-----|-------------------------|
| A     | @   | 185.199.108.153         |
| A     | @   | 185.199.109.153         |
| A     | @   | 185.199.110.153         |
| A     | @   | 185.199.111.153         |
| CNAME | www | `<username>.github.io`  |

После обновления DNS (до нескольких часов) сайт откроется по адресам
`amal-lia.com`, `amal-lia.com/amal`, `amal-lia.com/lia`.
