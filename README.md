# Certificate normalizer

Нормализатор сертификата электронной подписи (далее ЭП) в формате base64

Скрипт приводит содержимое сертификата ЭП в нормализованный вид.  
Добавляет `-----BEGIN CERTIFICATE-----` в начало файла и `-----END CERTIFICATE-----` в конец файла.  
Добавляет отступы каждые 65 символов для читаемости.

## Зависимости

Для реализации CLI интерфейса используется [typer](https://typer.tiangolo.com/)


## Установка модуля

```shell
pip install cert-normalizer
```

## Использование

```shell
python -m cert_normalizer path/to/cert.cer
```

Можно также указывать путь до директории. В таком случае скрипт будет искать все файлы сертификатов, заканчивающиеся на `.cer` и будет пытаться нормализовать их.
