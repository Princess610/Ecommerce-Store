# E-Commerce Store

## Technology Stack
- **Frontend**: .NET Web MVC
- **Backend**: .NET
- **Database**: PostgreSQL (Neon.tech)

## Database Schema

### Users Table
- `UserID` (Primary Key)
- `Username`
- `PasswordHash`
- `Email`
- `Role` (e.g., Admin, Customer)

### Products Table
- `ProductID` (Primary Key)
- `ProductName`
- `Description`
- `Price`
- `StockQuantity`
- `ImageURL`

### Orders Table
- `OrderID` (Primary Key)
- `UserID` (Foreign Key to `Users.UserID`)
- `OrderDate`
- `TotalAmount`

### OrderItems Table
- `OrderItemID` (Primary Key)
- `OrderID` (Foreign Key to `Orders.OrderID`)
- `ProductID` (Foreign Key to `Products.ProductID`)
- `Quantity`
- `Price`

## Visual Representation of Database Schema
![Database Schema](path/to/your/schema/image.png)
