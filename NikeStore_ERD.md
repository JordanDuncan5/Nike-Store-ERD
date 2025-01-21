```mermaid

erDiagram

"Nike Entity Relationship Diagram"

    Product ||--o{ Customer :"Take customer information"
    Product ||--o{ Inventory :"Take note of inventory you picked up"
    Product{
        string ProductID PK
        string ShoeSize FK
        string ShoeColor FK
    }
    
    Customer ||--o{ Sale :"Sell item"
    Customer{
        string CustomerID PK, FK
        string Name
        float PhoneNumber FK
        string Email FK
        address Address FK
        int Age FK
    }
    
    Sale ||--o{ Inventory :"Adjust inventory after sale"
    Sale{
        string PriceOptimization
        string PersonalizedRecommendations
        int ProductCost
        int Orders
    }
    
    Inventory{
        int StockLevel
        string SalesHistory 
        string MarketTrends
        float ProductPerformance
    }

```

### Documentation

This is a graphic used to show the process of managing inventory and customer information. You first start with your product and make a sale. During the process of checking out you take down your customer's information. This is to speed up the process if your customer wants to make another purchase. The customer information also helps with personalized marketing, tracking interations, purchasing patterns, etc. After you make a sale you update the items inventory as this keeps track of the inventory level and will build a collection of data for further use. The data you collect will help with noticing purchasing trends and product performance.