Objective:
Build a website for the purpose of buying and/or selling old books.
A very common use case, is in colleges, where students sell old books to their juniors.
This website should have a backend API written in NodeJS, using Sequelize as an ORM
(not using an ORM and writing manual SQL queries is acceptable too)
The backend should expose a REST API, that will be consumed by the frontend.
The frontend must be built using Angular. (v5 or v6 is acceptable to be used).



Data Entities

Users
Name
Email Address
College
Address
Phone Number
... other details you feel necessary

Listings
Seller (foreign key to user)
Book Name
Author Name
Image of item
Price
Condition (enum: New, Almost New, Slight Damage, Worn)


Pages (Screens/Routes)

Signup
User creates new accounts here

Login
User enters email/password here to login

All Listings
(This is also home page after login)
Eg: /listings
On this page user can see all the listings made by everyone
There should filters here
• Filter by price
• Filter by condition
• Search by name of book
• Search by author
Each listing should have a “Add to Wishlist” option

View Single Listing
Eg. /listings/{listingId}
When clicking a listing from ‘all listings’ page, user goes to individual listing page for that
particular listing.
The “Add to Wishlist” option should be here.
Also there should be an option to “Contact the seller” which would allow the user to send
a message to the seller of the item.

Add Listing
Eg. /listings/add
On this page user can add a new listing

Wishlist
Eg. /wishlist
User can add items to their wishlist
Wish list page should show all the books added by a user into his/her own wishlist.

Messages
Eg. /messages
Users can see messages they have received on the listings that they have created here
Submission Process


Deadline: Sunday 8th July, 11:59 PM


Deploying

Deploy your projects to Heroku (or similar platform that supports running a backend
along with a SQL Database). Your submission email should be a link to your project.
SQL on Heroku
You can use either PostgreSQL or MySQL database for free on Heroku.
How to use Postgres ?
https://devcenter.heroku.com/articles/heroku-postgresql
How to use MySQL ? (See any one)
https://devcenter.heroku.com/articles/jawsdb
https://devcenter.heroku.com/articles/cleardb
https://selimsalihovic.github.io/2016-02-07-using-mysql-on-heroku/