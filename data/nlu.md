## intent:greet
- hey
- howdy
- hey there
- hello
- hi
- good morning
- good evening
- dear sir
- hol
- hOLA
- Hola

## intent:affirm
- yes
- yep
- yeah
- indeed
- that's right
- ok
- great
- right, thank you
- correct
- great choice
- sounds really good
- thanks

## intent:deny
- No
- Nope
- No I am good
- Nah
- Nah I am fine
- No I am fine
- That's all

## intent:goodbye
- bye
- goodbye
- good bye
- stop
- end
- farewell
- Bye bye
- have a good one

## intent:thankyou
- thank you
- thanks have a great day
- gracias

## intent:send_email
- My email id is [prateek.bipul0907@gmail.com](email)
- Email is [prateek.bipul0907@gmail.com](email)
- My email address is [prateek.bipul0907@gmail.com](email)
- email address [prateek.bipul0907@gmail.com](email)
- My email id is [shubhamsharma23nov@gmail.com](email)
- email id is [shubhamsharma23nov@gmail.com](email)
- [shubhamsharma23nov@gmail](email)
- [shubhamsharma23nov@gmail.com](email)
- [prateek.bipultest@gmail.com](email)

## intent:restaurant_search
- i'm looking for a place to eat
- I want to grab lunch
- I am searching for a dinner spot
- I am looking for some restaurants in [Delhi](location).
- I am looking for some restaurants in [Bangalore](location)
- restaurants in [Bengaluru]{"entity": "location", "value": "Bangalore"} 
- restaurants in [Madras]{"entity": "location", "value": "Chennai"}
- restaurants in [Bombay]{"entity": "location", "value": "Mumbai"}
- restaurants in [Calcutta]{"entity": "location", "value": "Kolkata"}
- show me [chinese](cuisine) restaurants
- show me [chines]{"entity": "cuisine", "value": "chinese"} restaurants in the [New Delhi]{"entity": "location", "value": "Delhi"}
- show me a [mexican](cuisine) place in the [centre](location)
- i am looking for an [indian](cuisine) spot called olaolaolaolaolaola
- search for restaurants
- anywhere in the [west](location)
- I am looking for [asian fusion](cuisine) food
- [South Indian](cuisine)
- [North Indian](cuisine)
- [Italian](cuisine)
- [Chinese]{"entity": "cuisine", "value": "chinese"}
- [chinese](cuisine)
- [Lithuania](location)
- Oh, sorry, in [Italy](location)
- in [delhi](location)
- I am looking for some restaurants in [Mumbai](location)
- I am looking for [mexican indian fusion](cuisine)
- can you book a table in [rome](location) in a [Lesser than Rs 300](budget) price range with [british](cuisine) food for two
- can you book a table in [delhi](location) in [Rs 300 to 700](budget) price range with [North Indian](cuisine) food
- find me a restaurant in [Hyderabad](location) with [North Indian](cuisine) food and average cost of two [More than 700](budget)
- [central](location) [indian](cuisine) restaurant
- please help me to find restaurants in [pune](location)
- Please find me a restaurantin [bangalore](location)
- [mumbai](location)
- show me restaurants
- please find me [chinese](cuisine) restaurant in [delhi](location)
- can you find me a [chinese](cuisine) restaurant
- [delhi](location)
- please find me a restaurant in [ahmedabad](location)
- please show me a few [italian](cuisine) restaurants in [bangalore](location)
- find me a restaurant in Kolkara
- find me a restaurant in [Kolkata](location)
- [Rs 300 to 700](budget)
- I am hungry, can you suggest me some good restaurants in [Delhi](location)
- [More than 700](budget)
- Can you please find me a restaurant in [Rishikesh](location) for good [North Indian](cuisine) food
- in [Mumbai](location)
- [Rs 300 to 700](budget)
- Find me some good [South Indian](cuisine) restaurants in [Chennai](location) for [more than 700](budget) price range
- Find me some good [south indian](cuisine) restaurants in [Chennai](location)
- [More than 700](budget)
- Find [North indian](cuisine) restaurants in [Kanpur](location)

## synonym:4
- four

## synonym:Bangalore
- Bengaluru

## synonym:Chennai
- Madras

## synonym:Delhi
- New Delhi

## synonym:Kolkata
- Calcutta

## synonym:Mumbai
- Bombay

## synonym:chinese
- chines
- Chinese
- Chines

## synonym:mid
- moderate

## synonym:vegetarian
- veggie
- vegg

## regex:greet
- hey[^\s]*

## regex:pincode
- [0-9]{6}
