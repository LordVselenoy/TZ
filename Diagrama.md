gantt
    title План разработки GitRepoManager
    dateFormat  YYYY-MM-DD
    axisFormat  %d.%m

    section Подготовка
    Проектирование архитектуры       :a1, 2025-07-01, 3d
    UI-макетирование                 :a2, after a1, 2d

    section Интерфейс
    Реализация UI без логики         :b1, after a2, 5d
    Drag-and-drop функционал         :b2, after b1, 2d

    section Git-интеграция
    Внедрение libgit2sharp           :c1, after b2, 5d
    Поддержка базовых Git-операций   :c2, after c1, 3d
    Работа с ветками и конфликтами   :c3, after c2, 3d

    section Интеграция API
    Подключение GitHub API           :d1, after c3, 3d
    Подключение GitVerse API         :d2, after d1, 2d
    Подключение GitFlic API          :d3, after d2, 2d

    section Локализация и настройки
    Реализация настроек              :e1, after d3, 2d
    Локализация интерфейса           :e2, after e1, 1d

    section Финализация
    Кросс-платформенное тестирование :f1, after e2, 4d
    Сборка под Windows               :f2, after f1, 1d
    Сборка под Linux                 :f3, after f2, 1d
    Документация                     :f4, after f3, 2d