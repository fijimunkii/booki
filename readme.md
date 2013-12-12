Booki
=====

booki.me

The ultimate reservation app.

Think open table but for every kind of business that takes reservations.



User Stories
============

As an unregistered user,

* I want to see available times for businesses, so that I can make an appointment

* I want to filter by location, so that I can see what is around me

* I want to filter by category, so I can find what is interesting to me at the moment.

* I want to register, so I can make a booking.

As a registered user

* I want to set my name, so businesses can know my name.

* I want to set my location, so I can see nearby listings.

* I want to register a business, so I can make listings

* I want to make a booking, so I can schedule a service.

* I want to favorite a business or a user in a business, so I can stay updated of their listings.

* I want to become friends with other users, so we can recommend listings to each other.

As a registered user with a business

* I want to make a listing, so people can book it.

* I want to set a category for my business, so users can find it easily.

* I want to set location for my business, so users can find it easily.

* I want to set a phone number for my business, so users can contact me.

* I want to set an email for my business, so users can contact me.

* I want to set a description for my business, so users know what to expect.

* I want to set my business to private so it does not sure up normally.

As a registered user with a business and a listing

* I want to put a price on the listing, if there is a set price.

* I want to put a date on the listing, so it's available on a day.

* I want to put a time on the listing, so it's available at a certain time.

* I want to set the duration of the listing.

* I want to set the listing to be recurring an interval, so I can set it and forget it.

* I want to edit the time of the listing

* I want to edit the date of the listing

* I want to edit the duration of the listing

* I want to edit the description of the listing

* I want to edit the price of the listing


As a registered user with a private business

* I want to invite a user to see my listings


As a registered user with a business and booked listings

* I want to mark the booking as a no-show if the customer does not show up

* I want to write notes on the booking so I can recall the info on future bookings

As a user with booked listings

* I want to write notes on the booking so I can recall the info on future bookings

* I want to make a rating on the booking, so I can encourage or discourage future bookings

As a user with favorites

* I want to see all listings from that favorite

* I want to see all available listings from that favorite

* I want to set a category on that favorite so I can see what applies to me

As a user with a friendship

* I want to recommend a listing to a friend



Data Models
===========


users

* email
* password_digest
* name
* location
* description

businesses

* owner_id
* name
* location
* phone
* website
* email
* description
* is_private

businesses_users

* business_id
* user_id

private_accessors

* business_id
* user_id

friendships

* user_id
* related_user_id

favorites

* user_id
* related_user_id
* business_id
* category_id

listings

* business_id
* name
* date
* time
* duration
* description
* user_id

bookings

* listing_id
* user_id
* no_show
* rating
* user_notes
* business_notes

categories

* name

categories_listings

* category_id
* listing_id

businesses_categories

* business_id
* category_id

categories_users

* category_id
* user_id














