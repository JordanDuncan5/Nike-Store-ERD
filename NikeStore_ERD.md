```mermaid

erDiagram

"Nike Entity Relationship Diagram"

    Product ||--o{ Customer :next
    Product{
        string NikePegasus
        string NikeDunkLowRetro
        string NikeLunarRoam
        string NikeVaporEdgeSpeed
    }
    Customer ||--o{ Sale :next
    Customer{
        string customerID
        string customerName
        float customerPhoneNumber
        address customerAddress
    }
    Sale ||--o{ Inventory :next
    Sale{
        float productPerformance
        string priceOptimization
        string personalizedRecommendations
        float productCost
    }
    
    Inventory{
        float stockLevel
        string salesHistory
        string marketTrends
    }

```