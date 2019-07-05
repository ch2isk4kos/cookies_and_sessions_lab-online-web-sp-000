# *Rails* Cookies and Sessions Lab

#session
The Rails #session method gives us access to the Rails session.

The session is a *datastore* implemented with cookies.

You can store simple data structures in the session.

ActiveRecord models, no.
Arrays of strings or numbers, yes.

Basically, stick to *data literals*
* numbers, strings, hashes, and arrays.

You're going to use this to implement a shopping site

#Here's how the site will work:
* The root page of the app has an input box on it
(within a form of course).

* The user types in the item they want and clicks add to cart.

* The item is added to their cart.

* The page shows everything in the user's cart.



**Instructions**
1. Create the #cart method in ApplicationController#cart

   this method should return an array of the items stored in the cart (utilizing the Rails session method).

2. Create a Products controller with two actions, index and add.

3. Create the routes for the application, we only need two routes, one to display the Products#index (the root route) and one to post the products to add them to the cart.

4. Create views using the feature tests as your guide. The page should have, at a minimum: a text box where the user can enter the name of a product, a submit button that adds it to their cart, and a display of what's in the cart.

#For this lab, there is no need...
to create tables and models and store the products in the database.

#You'll be using cookies...
via the Rails session method, along with your cart helper method to persist the products to the cart and to display them in the view.