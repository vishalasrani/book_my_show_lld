# Design Pattern in BMS

## Factory Design Pattern

### 1. Creating Theatre
    - TheatreFactory
    -- IMAX
    -- SingleScreen
    -- Multiplex

### 2. Creating Movie
    - MovieFactory
    -- ComedyMovie
    -- ActionMovie
    -- ThrillerMovie
    -- etc


## Observer Design Pattern

### Subject 1: Book Ticket
    Publisher: System

    Subscribers: Customer, Theatre

### Subject 2: New Movie Launch
    Publisher: System

    Subscribers: All registered Theatres

### Subject 3: New Movie in a Theatre
    Publisher: Theatre

    Subscribers: All Customer who had add a movie in their wishlist for that theatre

### Subject 4: Promotion
    Publisher: System or Theatre

    Subscribers: Customers

### Subject 5: New Theatre Launch
    Publisher: System

    Subscribers: All customers of the city where theatre is opening

### Subject 6: Favourite Actor/Actress Movie Release
    Publisher: System

    Subscriber: All users who have added new movie's actor/actoress as his/her favourite


## Singleton Design Pattern

    DB Connection
    Logging
    Config

## Strategy Design Pattern

### Search Movie
    1. Search by Rating
    2. Search by Actor/Actress
    3. Search by Date
    4. Search by Theatre type
    5. Search by City
    6. Search by Availability
    
### Search Theatre
    1. Search by Theatre Type
    2. Search by distance
    3. Search theatre by movie