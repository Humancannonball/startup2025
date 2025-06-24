# Startup 2025: Mixed Reality Robotics Project

## Plug and Play Lithuania Accelerator Application

### Program Information
- **Program**: [Startup Lithuania Accelerator powered by Plug and Play](https://www.startuplithuania.com/publicfund/startup-lithuania-accelerator-powered-by-plug-and-play-5th-batch/) (5th & Final Batch)
- **Application Deadline**: July 4, 2025
- **Program Duration**: September 18 - December 12, 2025, Vilnius
- **Target**: Early-stage tech startups

### Documentation & Guides

| Document | Description |
|----------|-------------|
| [Comprehensive Guide](./startup_guide.md) | Complete program overview, requirements & selection criteria |
| [Полное Руководство](./стартап_гайд.md) | Полный обзор программы, требования и критерии отбора |
| [Application Plan](./application_plan_mixed_reality_robotics.md) | Пошаговая стратегия подачи заявки |

### Source Materials
- **Webinar Video**: [YouTube Link](https://m.youtube.com/watch?v=d8A8wRwTUxQ)
- **Transcript**: Generated from downsub.com subtitles

---

## Наш Проект

Основная задача проекта сделать новый интуитивный интерфейс для программирования мобильных роботов при помощи гарнитуры смешанной реальности.

### Какие плюсы даёт разработка
Может работать пользователь без опыта, быстрое создание карт помещения, визуальное программирование пути робота, визуальная симуляция движения робота в реальном мире для проверки подходит ли модель робота, как он везде проезжает без надобности в реальном, что так же может быть безопасней и дешевле в случае ошибки. Быстрый старт нового робота, карта и путь уже готовы.

### Софт
ROS2, Gazebo simulator, RViz, Nav2. Возможно Unity.

### Железо
Гарнитура смешанной реальности Meta Quest 3, мобильный робот TurtleBot 4 Lite, компы.

### Алгоритм программирования робота
- Пользователь надевает гарнитуру и сканирует помещение при помощи встроенных сенсоров
- Гарнитура отправляет 3D модель на сервер
- Сервер переводит 3D модель в формат URDF понимающий ROS2, Gazebo Simulator
- Проводим симуляцию движения робота по отсканированной 3D модели для получения карты навигации
- С помощью контроллеров Meta Quest указываем точки куда нужно ехать или строим из нескольких точек путь для робота
- Координаты указанных точек тоже отправляются на сервер
- В симуляторе прокладывается маршрут проводится симуляция движения виртуального робота
- Потом карта и путь загружаются в TurtleBot и робот едет по заданному маршруту

### Какие ещё могут быть варианты
Симуляция движения виртуального робота показывается в гарнитуре. Можно управлять виртуальным роботом видя его в реальном мире.
