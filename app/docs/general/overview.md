# Общее описание Air Pro

## Что такое Air Pro?

Air Pro - это приложение для мониторинга качества воздуха, разработанное для Windows. Оно позволяет отслеживать различные параметры качества воздуха в реальном времени, получая данные от Arduino-устройства.

## Основные возможности

### Мониторинг в реальном времени
- Отображение текущих показателей качества воздуха
- Визуализация данных в виде графиков
- Отслеживание изменений параметров

### Настройка и конфигурация
- Настройка пороговых значений для различных параметров
- Конфигурация профилей мониторинга
- Настройка уведомлений

### Экспорт и интеграция
- Экспорт данных в Excel
- Интеграция с ThingSpeak для хранения данных
- Веб-интерфейс для удаленного доступа к данным

## Технические требования

- Операционная система: Windows 10 или выше
- Python 3.11+
- Arduino-устройство с соответствующими датчиками
- COM-порт для подключения Arduino

## Архитектура

Приложение построено на следующих основных компонентах:
- Главное окно (`main_window.py`) - основной интерфейс приложения
- Окно настроек (`settings_window.py`) - конфигурация параметров
- Монитор качества воздуха (`air_quality_monitor2.py`) - обработка данных
- Интеграция с ThingSpeak (`thingspeak_client.py`, `thingspeak_integration.py`)
- Веб-сервер (`web_server.py`) - удаленный доступ
- Экспорт данных (`export_to_excel.py`)
- Профили качества воздуха (`air_quality_profiles.py`) 