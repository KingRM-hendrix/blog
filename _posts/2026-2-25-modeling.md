---
layout: post
author: KingRM-hendrix
title: "Database Modeling"
comments: true
---
To convert the scenario given into a data-modeling framework, I wrote down user stories to break down what what was needed to be done. I assumed that after making the user stories, I could go straight to modeling. Here are the user stories I made with the description I was given:

* As an owner, I can list items for sale.
  * I give this size about a 3 because this is an admin based story and requires the access to go to a specific person.
  * Since this is an isolated story with the owner, there are no connections to other stories.
* As a customer, I can register an account so I can purchase items.
  * This is given a size of 5 because it require input to be fed into the database.
  * This connects with other stories such as selecting items, starting an order, and finalizing order delivery date as an account is required for all three.
* As a customer, I can start an order so the items can get items from the store.
  * The size rating is 4 because of the simplicity making an order, such as adding to cart.
  * It connects to selecting what food to get because that is needed to make an order.
* As a customer, I can select what food is on sale so I can purchase it.
  * The size of this story I gave is a 6 for giving recommendations of food on sale and the list of the items given.
  * This connects to starting an order because of a need for a specific item within the store.
* As a customer, I can finalize my order with a specific date so I can plan my availability in getting the items.
  * I give a size rating of 2 because I believe the input of date and time would be simple.
  * This connects to making an order as the final part of it.

With the user stories made, I went to modeling the relations of the customer, the items they want, and the orders they place.

![My Alt Text]({{ '/assets/images/ERDLucid.png' | relative_url }})
![My Alt Text]({{ '/assets/images/SQLDiagram.png' | relative_url }})

Looking at my diagrams, I would say that they came out decent. The complications in the implementations within the models is whether I should have used the crows-feet Information Engineering style relationships on the attributes. Since I was also new to Redgate, I also had a small issue on how to make Primary Keys and Foreign Keys appear. I am also unaware if there should be more foreign keys on the order table. If there is a problem or confusion with my diagrams, please let me know, as I am just learning how to use databases.