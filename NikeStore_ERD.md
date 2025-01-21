```mermaid
---
title Nike Entity Relationship Diagram
---
erDiagram



    Product ||--o{ Customer :next
    Product{
        string nike-pegasus
        string nike-dunk-low-retro
        string nike-lunar-roam
        string nike-vapor-edge-speed
    }
    Customer ||--o{ Sale :next
    Customer{
        string marketing-strategies
        string personalized-service
        string optimize-customer-experience
    }
    Sale ||--o{ Inventory :next
    Sale{
        string product-performance-analysis
        string price-optimization
        string customer-segementation
        string personalized-recommendations
        float product-cost
    }
    
    Inventory{
        string inventory-management-software
        string stock-levels
    }

```