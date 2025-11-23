## HomeWork ([Colab.google.com](https://colab.research.google.com/drive/1-CGnenm9zSckXJ0oyk-ok2MKdAPndqk6))
# Домашняя работа по деревьям

graph TB
    %% Основные компоненты системы
    UI[Внешний интерфейс<br/>Web-приложение]
    DB[(База данных<br/>Экспериментов)]
    ML[Модель ML<br/>Прогнозирования]
    CALC[Программа вычисления<br/>упругих характеристик]
    
    %% Взаимосвязи
    UI --> DB
    UI --> ML
    UI --> CALC
    
    CALC --> DB
    ML --> DB
    
    DB --> ML
    DB --> UI
    
    %% Стили
    classDef interface fill:#e1f5fe,stroke:#01579b,stroke-width:2px
    classDef database fill:#f3e5f5,stroke:#4a148c,stroke-width:2px
    classDef ml fill:#e8f5e8,stroke:#1b5e20,stroke-width:2px
    classDef calc fill:#fff3e0,stroke:#e65100,stroke-width:2px
    
    class UI interface
    class DB database
    class ML ml
    class CALC calc
