```mermaid
graph TD
    A[Начало] --> B{i = 0; i < len(set_1)};
    B -- Да --> C{j = 0; j < len(set_2)};
    C -- Да --> D[Тело внутреннего цикла (операции с set_1[i] и set_2[j])];
    D --> E{j = j + 1};
    E -- Да --> C;
    E -- Нет --> F{i = i + 1};
    F -- Да --> B;
    F -- Нет --> G[Конец];
    B -- Нет --> G;
```
