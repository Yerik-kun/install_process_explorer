# Ansible Playbook: Install Process Explorer

Этот репозиторий содержит Ansible playbook для автоматической установки Process Explorer на Windows-хосты через Ansible AWX или CLI.

## Описание

Playbook `install_process_explorer.yml` автоматизирует процесс скачивания и установки Process Explorer — популярного инструмента для мониторинга процессов в Windows. Это упрощает настройку и обеспечивает единообразие при работе с несколькими машинами.

Основные шаги playbook:
- Создание временной директории на целевом хосте.
- Скачивание архива Process Explorer с официального сайта Microsoft.
- Распаковка и установка приложения.
- Очистка временных файлов.

## Требования

- Ansible версии 2.9 и выше с установленной коллекцией `ansible.windows`  
- Настроенный WinRM на целевых Windows-хостах  
- Python с пакетом `pywinrm` на управляющей машине

## Использование

1. Клонируйте репозиторий:  https://github.com/yerik-kun/install_process_explorer.git
