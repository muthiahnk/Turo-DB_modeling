# Turo-DB_modeling
Implementation of a Database for an Online Car-Rental Marketplace

## About Turo
Turo is a car rental marketplace where travelers can rent any car they want, wherever they want it, from a vibrant community of local car owners. Travelers choose from a unique selection of nearby cars, while car owners earn extra money and help fuel their adventures. It connects the Owners with Guests. Owners are people who list their cars on the website. Guests are people who rent the cars. To read more on how it works, visit https://turo.com/how-turo-works

## Analysis
Typically, a database design project starts with requirements. First, I analyze the requirements to identify the business rules, entities, and relationships. However, in this case I am using snapshots from a functional website ( www.turo.com ) to understand the entities and business rules so that I can reverse engineer the database design.

## Assumptions
* A user can sign up via Facebook, Google or via email and create an account
* An Owner can be a Guest too.
* You must capture the details of the listed cars in your design.
* The Owner can let Turo come up with an estimate of the rental or set a price himself/herself
* The Owner gets a share of the trip amount. The database design should track the results of the pricing and payment for each Owner.
* A Guest can browse for cars based on makes and model to find the car he/she prefers to rent.
* The Guest can request to book a car by looking up the location and date for which he/she wishes to rent the car (if its available) or book a car instantly.
* The Guest can meet the Owner at the location to get the keys or make a request to have the car delivered to a specified location
* A Host (when listing a car) provides information such as – license plate number, issuing country, state, photos of the car, location of the car, year, make, model, transmission, odometer, owner’s photo, owner’s date of birth, details of car availability, car description and car features.
* A guest can search for a car based on relevance, price, distance, instant booking, delivery, vehicle type, vehicle make, features, category, vehicle years, vehicle colors, transmission and distance included. The guest can also mention the location, date and time (duration) for when the car is needed.
* Guests could select area using the map feature available on the website. You should translate that into the Zip codes the cars are available in.
* The guest can leave reviews for the car after the trip.
* The guest can select the car from the list/map and make a request to book/book instantly
* The system keeps track of the car availability based on what’s booked and the timeframe selected
* The system should keep track of the transaction details every time a booking is made
