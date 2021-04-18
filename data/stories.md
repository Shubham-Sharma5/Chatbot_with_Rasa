## Complete Path 1 - With Valid email
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "delhi"}
	- slot{"location": "delhi"}
 	- action_validate_location
 	- slot{"location": "delhi"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
	- slot{"cuisine": "North Indian"}
    - action_validate_cuisine
 	- slot{"cuisine": "North Indian"}
	- utter_ask_budget
* restaurant_search{"budget": "Lesser than Rs 300"}
    - slot{"budget": "Lesser than Rs 300"}
	- utter_top_restaurant
	- action_search_restaurants
 	- utter_ask_about_emailing
* affirm
    - utter_ask_email_id
* send_email{"email": "prateek.bipul0907@gmail.com"}
 	- slot{"email": "prateek.bipul0907@gmail.com"}
 	- action_validate_email
 	- slot{"email": "prateek.bipul0907@gmail.com"}
 	- action_email
 	- utter_goodbye
    - action_restarted

## Complete Path 2 - Without Email Id
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "delhi"}
	- slot{"location": "delhi"}
 	- action_validate_location
 	- slot{"location": "delhi"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
	- slot{"cuisine": "North Indian"}
    - action_validate_cuisine
 	- slot{"cuisine": "North Indian"}
	- utter_ask_budget
* restaurant_search{"budget": "Lesser than Rs 300"}
    - slot{"budget": "Lesser than Rs 300"}
	- utter_top_restaurant
	- action_search_restaurants
 	- utter_ask_about_emailing
* deny
    - utter_goodbye
    - action_restarted


## Complete Path 3 - Unknown city (Not in Tier 1 or Tier 2).
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Vijaipur"}
	- slot{"location": "Vijaipur"}
    - action_validate_location
* restaurant_search{"location": "Allahabad"}
	- slot{"location": "Allahabad"}
 	- action_validate_location
 	- slot{"location": "Allahabad"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
	- slot{"cuisine": "North Indian"}
    - action_validate_cuisine
 	- slot{"cuisine": "North Indian"}
	- utter_ask_budget
* restaurant_search{"budget": "Lesser than Rs 300"}
    - slot{"budget": "Lesser than Rs 300"}
	- utter_top_restaurant
	- action_search_restaurants
 	- utter_ask_about_emailing
* affirm
    - utter_ask_email_id
* send_email{"email": "prateek.bipul0907@gmail.com"}
 	- slot{"email": "prateek.bipul0907@gmail.com"}
 	- action_validate_email
 	- slot{"email": "prateek.bipul0907@gmail.com"}
 	- action_email
 	- utter_goodbye
    - action_restarted

## User provided Location Initially
* greet
    - utter_greet
* restaurant_search{"location": "delhi"}
	- slot{"location": "delhi"}
 	- action_validate_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
	- slot{"cuisine": "North Indian"}
    - action_validate_cuisine
	- utter_ask_budget
* restaurant_search{"budget": "Lesser than Rs 300"}
    - slot{"budget": "Lesser than Rs 300"}
	- utter_top_restaurant
	- action_search_restaurants
 	- utter_ask_about_emailing
* affirm
    - utter_ask_email_id
* send_email{"email": "prateek.bipul0907@gmail.com"}
 	- slot{"email": "prateek.bipul0907@gmail.com"}
 	- action_validate_email
 	- action_email
 	- utter_goodbye
    - action_restarted

## User doesnot need help (Deny)
* greet
    - utter_greet
* deny
    - utter_default
* deny
    - utter_goodbye
	- action_restarted
## interactive_story_1
* greet
    - utter_greet
* restaurant_search

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Kolkata"}
    - slot{"location": "Kolkata"}
    - action_validate_location
    - slot{"location": "Kolkata"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - action_validate_cuisine
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs 300 to 700"}
    - slot{"budget": "Rs 300 to 700"}
    - utter_top_restaurant
    - action_search_restaurants
    - slot{"budget": "Rs 300 to 700"}
    - utter_ask_about_emailing
* send_email{"email": "shubhamsharma23nov@gmail.com"}
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_validate_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - utter_goodbye
    - action_restarted

## interactive_story_2
* greet
    - utter_greet
* restaurant_search{"location": "Delhi"}
    - slot{"location": "Delhi"}
    - action_validate_location
    - slot{"location": "Delhi"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_validate_cuisine
    - slot{"cuisine": "chinese"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - utter_top_restaurant
    - action_search_restaurants
    - slot{"budget": "More than 700"}
    - utter_ask_about_emailing
* send_email{"email": "shubhamsharma23nov@gmail.com"}
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_validate_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - utter_goodbye
    - action_restarted

## interactive_story_3
* greet
    - utter_greet
* restaurant_search{"location": "Rishikesh", "cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - slot{"location": "Rishikesh"}
    - action_validate_location
    - slot{"location": null}
    - utter_ask_location
* restaurant_search{"location": "Mumbai"}
    - slot{"location": "Mumbai"}
    - action_validate_location
    - slot{"location": "Mumbai"}
    - action_validate_cuisine
    - slot{"cuisine": "North Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs 300 to 700"}
    - slot{"budget": "Rs 300 to 700"}
    - utter_top_restaurant
    - action_search_restaurants
    - slot{"budget": "Rs 300 to 700"}
    - utter_ask_about_emailing
* affirm
    - utter_ask_email_id
* send_email{"email": "shubhamsharma23nov@gmail"}
    - slot{"email": "shubhamsharma23nov@gmail"}
    - action_validate_email
    - slot{"email": null}
    - utter_ask_email_id
* send_email{"email": "shubhamsharma23nov@gmail.com"}
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_validate_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - utter_goodbye
    - action_restarted

## interactive_story_4
    - utter_greet
* restaurant_search{"cuisine": "south indian", "location": "Chennai"}
    - slot{"cuisine": "south indian"}
    - slot{"location": "Chennai"}
    - action_validate_location
    - slot{"location": "Chennai"}
    - action_validate_cuisine
    - slot{"cuisine": "south indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - utter_top_restaurant
    - action_search_restaurants
    - slot{"budget": "More than 700"}
    - utter_ask_about_emailing
* affirm
    - utter_ask_email_id
* send_email{"email": "prateek.bipultest@gmail.com"}
    - slot{"email": "prateek.bipultest@gmail.com"}
    - action_validate_email
    - slot{"email": "prateek.bipultest@gmail.com"}
    - action_email
    - slot{"email": "prateek.bipultest@gmail.com"}
    - utter_goodbye
    - action_restarted

## interactive_story_5
    - utter_greet
* restaurant_search{"cuisine": "North indian", "location": "Kanpur"}
    - slot{"cuisine": "North indian"}
    - slot{"location": "Kanpur"}
    - action_validate_location
    - slot{"location": "Kanpur"}
    - action_validate_cuisine
    - slot{"cuisine": "North indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - utter_top_restaurant
    - action_search_restaurants
    - slot{"budget": "More than 700"}
    - utter_ask_about_emailing
* deny
    - utter_goodbye
	
## interactive_story_6
* greet
    - utter_greet
* restaurant_search{"location": "Vijaipur", "cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"location": "Vijaipur"}
    - action_validate_location
    - slot{"location": null}
    - utter_ask_location
* restaurant_search{"location": "Mumbai"}
    - slot{"location": "Mumbai"}
    - action_validate_location
    - slot{"location": "Mumbai"}
    - action_validate_cuisine
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs 300 to 700"}
    - slot{"budget": "Rs 300 to 700"}
    - utter_top_restaurant
    - action_search_restaurants
    - slot{"budget": "Rs 300 to 700"}
    - utter_ask_about_emailing
* affirm
    - utter_ask_email_id
* send_email{"email": "shubhamsharma23nov@gmail"}
    - slot{"email": "shubhamsharma23nov@gmail"}
    - action_validate_email
    - slot{"email": null}
    - utter_ask_email_id
* send_email{"email": "shubhamsharma23nov@gmail.com"}
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_validate_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - action_email
    - slot{"email": "shubhamsharma23nov@gmail.com"}
    - utter_goodbye
    - action_restarted
	
## interactive_story_7
    - utter_greet
* restaurant_search{"cuisine": "North indian", "location": "Pune"}
    - slot{"cuisine": "North indian"}
    - slot{"location": "Pune"}
    - action_validate_location
    - slot{"location": "Pune"}
    - action_validate_cuisine
    - slot{"cuisine": "North indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - utter_top_restaurant
    - action_search_restaurants
    - slot{"budget": "More than 700"}
    - utter_ask_about_emailing
* deny
    - utter_goodbye
