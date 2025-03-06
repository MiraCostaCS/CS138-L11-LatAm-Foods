Latin American Food Flashcards
===================

_Learning Objective: Demonstrate use of dictionaries and file input._

Food is a way to bring people together and celebrate. Latin American dishes are widely known for their incorporation of a variety of spices while also drawing on inspiration from cultures around the world. Each country has a national dish that embodies their cultural heritage. For example, Brazil's national dish is Feijoada, a bean stew mixed with beef or pork. This dish is so loved within Brazil that they dedicate a day to cooking Feijoada. In this lab you will be making a program to learn a little bit more about the national dishes of some Latin American countries.

[National Dishes of Latin America; A Latin American Food Fiesta!](https://youtu.be/p6zzjHm_vVw?si=NhESY8LD4HdbyXgY)

Dictionaries are basically look up tables, like an ordinary dictionary (think a pocket Spanish-English dictionary, Oxford English dictionary, or even the Urban dictionary). There's a key you look up and then a definition and/or translation as the value.

You will be given a text file called **"database.txt"** which has data separated by a particular symbol. This file has a key-value pair you will use to build your dictionary. The first part (the key) is the Latin American country and the second (the value) is its national dish. After making the dictionary, you will iterate through all the pairs by printing the country and then having the user hit "Enter" to see the dish and some facts about it. You should iterate through all the terms. Afterward, allow the user to review by typing in any Latin American country and providing them with the dish and facts. To accomplish this complete program, we will practice decomposing a problem into smaller modular parts.

Step 1: Create a Dictionary
---------------------------
Create a function called `build_dict(file_name)`. It takes a `file_name` string as parameter, and it returns a dictionary object with the file content.

1.  Opens up the file and iterates through each line
2.  For EACH line:
    * Separates the key/value for each line based on a tilde ("`~`")
    * Stores each key and value as appropriate in the dictionary
3.  Returns the dictionary

Step 2: Check the Dictionary
----------------------------
Create a function called `check_dict(key, dictionary)`. It takes in a string text to look up in the dictionary, and it returns the value if found, or "No match found" otherwise.

Pseudocode/Algorithm:
```
IF term is in dictionary
    Return value
ELSE
    Return "No match found"
```
Step 3: Show All Facts
----------------------
Create a function called `show_all(dictionary)` that takes a dictionary as a parameter. The function should iterate through the dictionary and for each key-value pair:

1.  print the key
2.  prompt user to hit "Enter",
3.  after they do, then print the value

Step 4: User Review
-------------------
Create a function called `review(dictionary)` that takes a dictionary as a parameter. While the user does not enter the word "stop", the function should:

1.  prompt the user to type in a country to look up
2.  call the `check_dict` function with the user's entry and print the returned value

Step 5: Create `main`
-------------------
Create `main()` function to:

1.  Build the dictionary by calling `build_dict(fileName)`
2.  Call the `show_all` function
3.  Call the `review` function

Expected User Interaction
-------------------------
```
Let's see the national dishes of some Latin American countries!

Country: Argentina
Press enter/return to see the dish.
National Dish: Asados is generally more of a cooking technique and is similar to a cookout where many assortments of meat are grilled. Asados pays respect to the history of Argentina and the history of gauchos (cowboys), who created the technique of cooking meat over a fire. 
Press enter/return for the next card.

Country: Mexico
Press enter/return to see the dish.
National Dish: Mole is a marinade made from spices and occasionally chocolate may be added to give the marinade a sweet taste. Mole is typically poured on top of chicken and paired with rice.
Press enter/return for the next card.

Country: Bolivia
Press enter/return to see the dish.
National Dish: Salteña is a savory pastry that is similar to an empanada and is filled with meats, raisins, and potatoes. The ability to eat salteña's without any utensil allowed for the dish to grow in popularity as a street food.
Press enter/return for the next card.

Country: Chile
Press enter/return to see the dish.
National Dish: Pastel De Choclo is the national dish of Chile. This dish is a corn pie with ground beef filling, chicken, raisins, and sometimes eggs. Pastel de choclo is well loved because it is a simple dish to make and is often served at large gatherings during the summer. 
Press enter/return for the next card.

Country: Colombia
Press enter/return to see the dish.
National Dish: Bandeja Paisa has a variety of ingredients, the most common ones being ground meat, beans, rice, fried eggs, sausage, morcilla, and chicharrón. Bandeja paisa originated from Antioquia, Columbia and now represents not only that city, but the entire country. 
Press enter/return for the next card.

Country: Costa Rica
Press enter/return to see the dish.
National Dish: Gallo Pinto is known for having numerous variations of how it is served, however, it always has a rice and beans base. Gallo pinto is a reflection of how rice and beans have remained a staple crop within Costa Rica. 
Press enter/return for the next card.

Country: Guatemala
Press enter/return to see the dish.
National Dish: Pepián is a meat based stew that can be customized to the consumers liking. Pepián is a representation of the indigenous foods from Guatemala's colonial past. 
Press enter/return for the next card.

Country: El Salvador
Press enter/return to see the dish.
National Dish: A pupusa is a thick flatbread that can be stuffed with a wide variety of fillings. Pupusas are a household staple that can be served for family dinners 
Press enter/return for the next card.

Country: Cuba
Press enter/return to see the dish.
National Dish: Ropa Vieja is a dish consisting of slowly cooked shredded beef with peppers, onions, tomato sauce, and spices. Ropa vieja represents the ability to turn modest ingredients into a tasteful and fulfilling meal.
Press enter/return for the next card.

That's all the countries in the database. Which would you like to revisit?

Enter country (stop to end): 
Answer: No match found.

Enter country (stop to end): Colombia
Answer: Bandeja Paisa has a variety of ingredients, the most common ones being ground meat, beans, rice, fried eggs, sausage, morcilla, and chicharrón. Bandeja paisa originated from Antioquia, Columbia and now represents not only that city, but the entire country. 

Enter country (stop to end): Costa Rica
Answer: Gallo Pinto is known for having numerous variations of how it is served, however, it always has a rice and beans base. Gallo pinto is a reflection of how rice and beans have remained a staple crop within Costa Rica. 

Enter country (stop to end): stop
End of Program.
```

Test and Submit
---------------
There are automated test for this assignment. Run the tests to determine whether your output matches the expected output. Remember that it checks by comparing characters, so make sure your prompts match those in the instructions above.

As always, stop by student hours, send your instructor an email, check in with a peer, or stop by the Learning Center if you need any assistance.