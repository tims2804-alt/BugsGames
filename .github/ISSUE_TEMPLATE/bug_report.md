---
name: Bug report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

name: 🐛 Баг в игре
description: Заполни все поля по таблице
title: "[BUG] ID + Краткое описание"
labels: ["bug"]
body:
  - type: textarea
    id: id
    attributes:
      label: ID
      placeholder: "001, 002..."
    validations:
      required: true
  
  - type: textarea
    id: modul
    attributes:
      label: Модуль
      placeholder: "Главное меню, Бой, Инвентарь..."
  
  - type: textarea
    id: kratkoe
    attributes:
      label: Краткое описание
      placeholder: "Кнопка не работает"
  
  - type: textarea
    id: podrobnoe
    attributes:
      label: Подробное описание
      placeholder: "Полное объяснение проблемы..."
  
  - type: textarea
    id: shagi
    attributes:
      label: Шаги по воспроизведению
      render: bash
      placeholder: |
        1. Зайди в игру
        2. Нажми кнопку X
        3. Ошибка Y
  
  - type: dropdown
    id: vosproizvodimost
    attributes:
      label: Воспроизводимость
      options:
        - Всегда
        - Иногда  
        - Редко
        - Один раз
      default: 0
  
  - type: dropdown
    id: prioritet
    attributes:
      label: Приоритет
      options:
        - Критический (блокирует игру)
        - Высокий
        - Средний
        - Низкий
      default: 2
  
  - type: textarea
    id: simptom
    attributes:
      label: Симптом
      placeholder: "Игра крашится / Кнопка не реагирует..."
  
  - type: dropdown
    id: obojti
    attributes:
      label: Возможность обойти
      options:
        - Нет
        - Да (опиши как)
  
  - type: textarea
    id: kommentarii
    attributes:
      label: Комментарий
      placeholder: "Дополнительная инфа..."
  
  - type: textarea
    id: prilozheniya
    attributes:
      label: Приложения
      placeholder: "Скриншоты, логи, видео..."
