```mermaid
---
Nike Entity Relationship Diagram
---
erDiagram
    Product ||--o{ Customer :next
    Product{
        string name
        string name
        string name
        string name
    }
    Customer ||--o{ Sale :next
    Customer{
        string marketing strategies
        string personalized service
        string optimize customer experience
    }
    Sale ||--o{ Inventory :next
    Sale{
        string product performance analysis
        string price optimization
        string customer segementation
        string personalized recommendations
        float product cost
    }
    
    Inventory{
        string inventory management software
        string stock-levels
    }

```