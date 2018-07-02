# Doug's Garage: Fitness Equipment Shop

The goal of this project is to generate a store-front to allow users to browse products, add them to a shopping cart and check out.  
Administrators will be able to create and edit products and reference customer orders.

## Navbar Component
* Reusable navigation bar component.  Bootstrap styling.
* Drop-down menu that populates additional links for administrators to manage orders and products.
* Log-in link is hidden once a user is logged in. Their username will then appear.

## Log-in/Log-out and Admin privileges
* Uses Google accounts for login and are stored as logged-in using FireBase localStorage
* Users are redirected when they log in.
* Administrator routes are protected through an authorization Service leveraging FireBase's auth Service

## Product Management
* Admins may create, edit, and delete products which are then stored/altered on the FireBase server.
* Validations are in place so fields may not be left empty.  Price requires a number and imageUrl requires a valid URL.
* Product list is attractive and enjoys pagination and sorting
* Search functions are in place to live-search existing products

## Product Catalog
* Display and filter products displayed on the homepage by category, or all, using query parameters inserted into and extracted from the URL
* Bootstrap the category filter menu so it sticks to the top of the page when scrolling

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.
