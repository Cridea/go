Небольшое RESTful API для управления списком задач (ToDo). 
API позволяет создавать, читать, обновлять и удалять задачи. Каждая задача содержит следующие поля:

ID (уникальный идентификатор)
Title (название задачи)
Description (описание задачи)
Completed (статус выполнения задачи, булево значение)

API

Эндпоинты

### GET /tasks
Возвращает все задачи.

### GET /tasks/{id}
Возвращает задачу по ID.

### POST /tasks
Создает новую задачу. Пример тела запроса:
{
  "title": "Новая задача",
  "description": "Описание задачи",
  "completed": false
}

### PUT /tasks/{id}
Обновляет задачу по ID. Пример тела запроса:

json
{
  "title": "Обновленная задача",
  "description": "Обновленное описание",
  "completed": true
}
### DELETE /tasks/{id}
Удаляет задачу по ID.
