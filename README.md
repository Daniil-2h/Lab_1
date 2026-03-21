# Лаб. работа 1: 
Веб-приложение на **Flask**, которое возвращает количество дней до Нового года.  
# 1. Клонирование репозитория
```bash
git clone https://github.com/Daniil-2h/Lab_1.git
cd <папка-проекта>
```

# 2. Сборка образа
```bash
docker build -t lab_1 .
```

# 3. Запуск контейнера
```bash
docker run -p 4200:4200 lab_1
```

После запуска приложение будет доступно по адресу `http://localhost:4200`.
# 4. Проверка работы
```bash
curl --location 'http://localhost:4200/info'
```

Пример ответа:
```JSON
{
  "days_before_new_year": 285
}
```