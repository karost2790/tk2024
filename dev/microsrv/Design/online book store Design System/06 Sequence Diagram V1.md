Sure, here's a sequence diagram illustrating the interactions between actors and the system for the main use cases of the online bookstore application:

```
Title: Online Bookstore Sequence Diagram

Customer -> Online Bookstore System: Browse Books
Online Bookstore System -> Database: Retrieve book catalog
Database --> Online Bookstore System: Book catalog data
Online Bookstore System --> Customer: Display book catalog

Customer -> Online Bookstore System: View Book Details
Online Bookstore System -> Database: Retrieve book details
Database --> Online Bookstore System: Book details data
Online Bookstore System --> Customer: Display book details

Customer -> Online Bookstore System: Manage Shopping Cart
Online Bookstore System -> Database: Retrieve shopping cart data
Database --> Online Bookstore System: Shopping cart data
Online Bookstore System -> Database: Update shopping cart
Database --> Online Bookstore System: Updated shopping cart data
Online Bookstore System --> Customer: Display updated shopping cart

Customer -> Online Bookstore System: Checkout Process
Online Bookstore System -> Customer: Prompt for shipping information
Customer -> Online Bookstore System: Provide shipping information
Online Bookstore System -> Customer: Prompt for payment details
Customer -> Online Bookstore System: Provide payment details
Online Bookstore System -> Database: Process payment and create order
Database --> Online Bookstore System: Order confirmation
Online Bookstore System --> Customer: Display order summary

Customer -> Online Bookstore System: User Authentication
Online Bookstore System -> Customer: Display authentication options
Customer -> Online Bookstore System: Select authentication option
Online Bookstore System -> Database: Authenticate user
Database --> Online Bookstore System: User authentication data
Online Bookstore System --> Customer: Allow access to authenticated features

Customer -> Online Bookstore System: View User Profile
Online Bookstore System -> Database: Retrieve user profile data
Database --> Online Bookstore System: User profile data
Online Bookstore System --> Customer: Display user profile
Customer -> Online Bookstore System: Update user profile
Online Bookstore System -> Database: Update user profile data
Database --> Online Bookstore System: Updated user profile data
Online Bookstore System --> Customer: Display updated user profile

Administrator -> Online Bookstore System: Manage Orders
Online Bookstore System -> Database: Retrieve order data
Database --> Online Bookstore System: Order data
Online Bookstore System --> Administrator: Display list of orders
Administrator -> Online Bookstore System: Process order
Online Bookstore System -> Database: Update order status
Database --> Online Bookstore System: Updated order status
Online Bookstore System --> Administrator: Confirm order processing
```

This sequence diagram illustrates the flow of interactions between customers, administrators, and the online bookstore system for the main use cases outlined earlier. Each step in the sequence represents a specific action performed by an actor or the system, providing a visual representation of the system's behavior during different scenarios.