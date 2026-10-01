# Lab 04 - Windows Event Viewer

## Цель
Научиться искать и фильтровать события Windows.

## Что сделал
- Открыл Event Viewer
- Изучил System и Application logs
- Создал тестовое событие через eventcreate
- Отфильтровал журнал по Event ID
- Нашел события через PowerShell
- Использовал Get-WinEvent

# Команды
- eventcreate /T INFORMATION /ID 100 /L APPLICATION /SO AdminLab /D "Day 4 test event"
- Get-WinEvent -LogName Application -MaxEvents 10
- Get-WinEvent -FilterHashtable @{LogName='Application'; Id=100}

# Что понял
Event Viewer помогает связать проблему со временем, источником события и конкретной ошибкой.