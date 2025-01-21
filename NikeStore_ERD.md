```mermaid

erDiagram

"Nike Entity Relationship Diagram"

    Product ||--o{ Customer :"take customer information"
    Product ||--o{ Inventory :"Take note of inventory you picked up"
    Product{
        string NikePegasus
        string NikeDunkLowRetro
        string NikeLunarRoam
        string NikeVaporEdgeSpeed
    }
    
    Customer ||--o{ Sale :"sell item"
    Customer{
        string CustomerID
        string Name
        float PhoneNumber
        string Email
        address Address
    }
    
    Sale ||--o{ Inventory :"Adjust inventory after sale"
    Sale{
        float ProductPerformance
        string PriceOptimization
        string PersonalizedRecommendations
        int ProductCost
    }
    
    Inventory{
        int StockLevel
        string SalesHistory
        string MarketTrends
    }

```