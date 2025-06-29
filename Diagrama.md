```mermaid
gantt
    title План разработки GitRepoManager
    dateFormat  YYYY-MM-DD
    axisFormat  %d.%m
    todayMarker off

    section Подготовка
    Проектирование архитектуры         :a1, 2025-07-01, 3d
    UI-макетирование                   :a2, after a1, 2d

    section Реализация интерфейса
    Базовый UI (дерево репозиториев)   :b1, after a2, 3d
    Drag-and-drop функционал           :b2, after b1, 2d
    Панели управления Git-операциями   :b3, after b1, 2d

    section Git-интеграция
    Внедрение libgit2sharp             :c1, after b3, 3d
    Базовые операции (commit/push)     :c2, after c1, 2d
    Управление ветками и конфликтами   :c3, after c2, 2d

    section Интеграция API
    Подключение GitHub API             :d1, after c3, 2d
    Подключение GitVerse API           :d2, after d1, 1d
    Подключение GitFlic API            :d3, after d2, 1d
    Система авторизации                :d4, after d1, 2d

    section Тестирование
    Юнит-тесты                        :e1, after c1, 3d
    Интеграционное тестирование       :e2, after d4, 4d

    section Финализация
    Локализация (русский)             :f1, after e2, 2d
    Сборка под Windows                 :f2, after f1, 2d
    Сборка под Linux                   :f3, after f1, 2d