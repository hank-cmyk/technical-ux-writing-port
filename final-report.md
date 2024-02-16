# Recipeasy Final Report

- Project Group: Gray Guava
- Team Members: Hanna Kang (hak63), Yulu Cao (yc758), Simrin Kapoor (sk2422), and Jason Zheng (jz449)
- Project summary: ***Recipeasy***, a mobile app that facilitates the recipe finding process

## Table of Contents 
- [Recipeasy URL](#recipeasy-url)
- [Discovery and planning](#discovery-and-planning)
    - [User interviews](#user-interviews)
    - [Affinity diagramming](#affinity-diagramming)
    - [Summary of interviews and card sort](#summary-of-interviews-and-card-sort)
    - [Key problems](#key-problems)
    - [Value propositions](#value-propositions)
    - [Scenarios](#scenarios)
    - [Persona](#persona)
    - [Project themes](#project-themes)
- [Design and evaluation](#design-and-evaluation)
    - [Brainstorming](#brainstorming)
    - [Sketches](#sketches)
    - [Final sketch](#final-sketch)
    - [Rationale for design](#rationale-for-design)
- [High-fidelity app prototype planning](#app-prototype-planning)
- [App prototype evaluation](#app-prototype-evaluation)
    - [User testing questions](#user-testing-questions)
    - [Debrief of user testing](#debrief-of-user-testing)
    - [Issues discovered from user testing](#issues-discovered-from-user-testing)
- [Future improvements](#future-improvements)

## Appendix
- [Interview notes](interview-notes.md)
- [Affinity diagram/card sorting](card-sorting.md)
- [User testing notes](user-testing-notes.md)

## Recipeasy url
- https://gray-guava-project.herokuapp.com/

## Discovery and Planning

### Users 
Our users are college students who cook on a consistent basis and want a more efficient cooking process.

### Methods & Justifications
- 7 semi-structured interviews with our interviewees. 
- Semi-structured interviews were the best way to gather data from users because in field studies, they may have felt more pressure completing everyday cooking tasks under our gazes. We also wanted to gather data from non-Cornell students, and as such, field studies wouldn't have been possible. 

### User interviews
#### Interview questions
General question: Tell me about your entire cooking process, from choosing what you want to eat, go grocery shopping, to the end of the cooking process/from beginning to the end.
1. How do you describe your cooking skill? (novice, intermediate, or expert)
2. In a week, how many meals/how often do you cook?
   - Are you cooking for yourself or for others as well?
3. What obstacles do you face when cooking?
4. What do you think could help you make the cooking process better/easier?
5. What kinds of ingredients do you most often cook with?
6. Do you look for recipes before cooking?
   - If so, how?
   - Why?
7. Can you recall a time when you looked up a recipe? Tell me about it.
8. Do you have a collection of recipes?
   - If so, how do you store them/organize them?
In addition to this, we will also ask any other questions, follow-up or otherwise, that come up during our interviews
- [Interview notes](interview-notes.md)

### Affinity Diagramming
- We took the findings and notes taken during our user interviews and analyzed them to determine the needs of our users. We grouped them by common categories and issues and found the following key points of the users' goals. 
- [Affinity diagram/card sorting](card-sorting.md)

### Summary of interviews and card sort
- Users want instructions that are easy to follow, clear, and also step-by-step
- Users want to store recipes in convenient and easy to access ways
- Users want to look up recipes without too much effort, and find recipes that are based on reasons such as cravings, ingredients they have, or techniques
- User want to stay organized and tidy throughout the cooking process

### Key problems
1. Users have trouble following recipes that are too complicated, or don't have step-by-step or clear instructions
2. Users keep making the same kinds of meals with the same ingredients, and sometimes are not satisfied with the limited variety 

### Value Propositions
- This app enables a more organized, clear way for users to find and follow recipes step-by-step, from the ingredient gathering process to plating
- The app enables complicated recipes to be broken down into simple, timeable steps
- The app suggests new recipes based upon the users’ favorite recipes

### Scenarios
- Jon is an Information Science student who is planning to make dinner after his last class of the day, which ends at around 5:00pm. He knows that he has tomatoes in his kitchen, and he'd like to make an interesting yet simple meal with them before they spoil, but he doesn't know what he will make yet. Jon does know, however, that he wants to make it under an hour, as he has a lot of homework. When he goes onto the app, he searches up "tomato" so that he could find a recipe, and finds one for soup that would take ~30min. He follows this tomato soup recipe through to the finish. 
- Audrey is a Math student with limited cooking skills, and is planning to hold a barbecue this weekend for her friends, as a celebration for finishing their prelims. She wants to make sure she has enough time to start cooking on Saturday morning, so that she is ready for the evening gathering. Through the app, Audrey looks at the time it will take to cook cheese burgers, a recipe that she knows her friends love, and finds out how long it till take so she knows exactly when to start cooking. 
- Isabel is an English student, and she loves to cook dinner for herself and her roommates after class. She usually likes to cook grilled cheeses, because cheese is her favorite ingredient to cook with, and it's also comforting, warm, and filling for her and her roommates. However, Isabel and her roommates have gotten kind of tired of all the grilled cheese, so they are looking for a new recipe that still includes cheese in some capacity, and will still be filling and comforting. When opening the app, Isabel sees that theres a recipe that is suggested for her. She thinks this is perfect, because it still includes cheese, and will also be filling and enjoyed by everyone.

### Persona
Gary is a senior studying Computer Science at Cornell. He loves taking walks between classes and whenever he has free time, and finds himself eating lunches at Mattin's a lot, both because it's very convenient as an engineer, but also because he likes the food options there and knows that he'll find whatever he orders delicious. He lives in Collegetown by himself, and he enjoys cooking himself meals at least once a day. Gary doesn't always have enough time to go grocery shopping or search across the entire Internet for varying recipes, so he ends up ordering the same ingredients many times and making the same meals. Because he is looking at a screen all day, he doesn't enjoy reading very large amounts of text, especially after days with many classes. 

### Project Themes
- Mobile app - The app will be designed for mobile use, as this is convenient and accessible for users. This will also allow us to focus on a more vertical (mobile) design, and work with the smaller space. 
- Concise, less text - The app will have a larger focus on concise text, and also include images. Recipes will be displayed with images next to a simple title and the time needed for making the recipe, and the instructions for the recipes themselves will be split up into separate screens, to deter from very long and sometimes overwhelming blocks of text in a row. 
- Timeable step-by-step instructions - Each step for the recipe will include a feature for a timer, which would be counting down as the user completes the step. This will help them to manage their time better, and to alleviate any pressure from timing, the timer will also include a pause button, a play button, and a refresh timer button. 
- Smart suggestions - The app will include recipe suggestions based on the recipes that the user has favorited. This will allow them to get more variety in what they make, while also being tailored towards them. This will likely not be fully developed and coded as part of the final prototype. 

## Design and evaluation

### Brainstorming
Below is our brainstorming for initial possibilities of our app. We took our persona, Gary, and tried to come up with design ideas based on him. We also tried sketching out some ideas for the screens we want to create.
- Brainstorming ideas for Gary ![Brainstorming with Gary](images/brainstorm1.jpg)
- Brainstorming screen ideas ![Brainstorming screen ideas](images/brainstorm2.jpg)

### Sketches
Below is our first version of sketches for the screens we would like to include in our app. The first version has a bar at the bottom, with icons for other screens: homepage, favorites, search, A-Z. The homepage includes a welcoming message, and also a few randomized recipes that are in the app. The favorites page includes recipes that the user "favorited," and this screen would let them access all of these recipes. The search screen would let users search for recipes based on ingredients/specific recipe names, and also has filters that they can filter by. The A-Z page would have a list of all recipes in the app, alphabetized. The recipe pages are what would display if the user selected a recipe to make. It includes a checklist of ingredients, and provides a very step-by-step process of the recipe. The recipe would also be timeable, so Gary would be able to manage his time better when cooking.
- Screens iteration 1 ![Iteration 1 of screens](images/sketch1.jpg)

Below is our second version of sketches for the screens we would like to include. They are more or less the same, with notable differences being that we have taken the favorites page out of the bottom bar. We decided that the favorites page would probably be better to be accessed at the top corner of the homepage, because if the user didn't have any "favorited" recipes at all, an entire section of the bar at the bottom would have no use. In addition, the favorites page button would be very visible at the top corner, moreso than in the bottom bar. The bottom bar is also simpler with only 3 icons rather than 4.
- Screens iteration 2 - home screen ![Iteration 2 of screens](images/sketch2.jpg)
- Screens iteration 2 - all other screens ![Iteration 2 of screens](images/sketch2B.jpg)

Below is our third iteration of sketches for the screens. Notable differences include more detailed cards on the homescreen, favorites page, search page, and all recipes page. These cards are of variable size, but all consist of a picture of the dish, name of the dish, and time to cook. Furthermore, we fleshed out the recipe directions page to include a timer component alongside the actual step instructions. This will allow Gary to keep track of how approximately how much time he has to finish a step in the recipe process.
- Screens iteration 3 ![Iteration 3 of screens](images/sketch3.png)

### Final sketch
This is our final sketched design for our app.
- Final sketch ![Final sketches](images/finalsketch.png)

### Rationale for design
- Screens
    - Home screen
        - The home screen lists a suggested “recipe of the day” for the user based on their favorite recipes.

    - Search screen 
        - The search screen enables the user to find a recipe of their choosing by inputting a specific ingredient into the search bar.

    - Recipe screen
        - The recipe screen is actually a series of screens that guides a user through a specific recipe.
        - At each step in the recipe, the screen will display instructions and also a timer associated with the specific step.

    - Favorites screen 
        - The favorites screen contains the recipes that a user has favorited in the past.
        - This allows for quick access to certain recipes that the user wants to save for future use.

- Key problems
    - users have trouble following recipes that are too complicated (or do not have step-by-step or clear instructions)
    - users keep making the same kinds of meals with the same ingredients and are sometimes not satisfied with the limited variety

- Key problems solutions
    - providing a simple means for users to follow a recipe of their choice step-by-step
    - our design provides a clear, guided process for users to cook recipes that they want to try
    - our design also influences user behavior through the timer feature in that it encourages users to spend the correct amount of time on each step of the recipe
    - our design lists each step of the recipe one at a time, which helps users focus on the current step of the cooking process
        - this enables the user’s mind to be at ease and easily implement a specific recipe. 

In our first scenario of Milestone 2, we described the user as needing to follow a recipe containing tomatoes step-by-step. In our design, the user will follow these steps:

- Open the app
- Go to the “search” screen
- Search for “tomato” in the search bar
- Select a tomato recipe from the listed choices
- Make your way through the guided cooking process until completion

Through this description, our app design effectively communicates with the user and meets their goals:
- our design provides a clear, step-by-step process for the user to efficiently cook a recipe from the ingredient gathering process to plating. 
    - this enables complicated recipes to be broken down into simple steps for the user to follow. 
- also, our design contains a timer feature, so the user spends the correct amount of time at each step in the recipe.
- our design suggests new recipes based on the users’ favorited recipes. 

## App prototype planning
Below is some of the planning we did for the app's organization and modularity. It includes the views we think we may need, as well as the components and also the start of planning for JSON mock data. 
- Planning app organization ![Planning app organization](images/m4planning.png)

- Four branches: 
    - home screen branch
    - search branch (includes search screens 1 and 2)
    - favorites screen branch
    - recipe branch (includes recipe screens 1-4)

## App prototype evaluation

### User testing questions
1. You are a student who is planning to make dinner after your last class. You know you have tomatoes that are going spoil and would like to make a meal with them, and you have enough time to cook something that would take longer than half an hour. Find a recipe and follow it step-by-step through to the end.
2. You are a student with limited cooking skills who has a lot of time to make a long recipe for a grilling barbecue with friends this weekend. You want to make sure that you have enough time, so you pick a recipe and note down how long the full cooking process would take.
3. You are a student who cooks dinner for you and your roommates a lot after classes are done for the day. You often make the same cheesy foods because you and your friends love cheese. You know that you've made several cheesy recipes before that you loved. Locate at least one of previously cooked beloved cheesy recipes.

### User testing notes
- [User testing notes](user-testing-notes.md)

### Debrief of user testing
In general, our users were able to complete the tasks with relative ease; however, they had some issues and confusion. To begin, most of our users commented on the timer component during our first scenario since it was not yet implemented. The lack of functionality contributed to a bit of miscommunication in the conversation between the user and the UI. 

In the second scenario, even though our users were able to complete the task, they did so in a longer amount of time than expected. This was because they would either search up a recipe by the time it would take to make, or by the occasion (i.e. "barbecue", "grill") and could not find any results. Some of them ended up just looking at all the recipes listed on the search page, and found one manually. 

In the third and final task, our users either clicked on the suggested recipe card on the home screen, or navigated to the Favorites page. The main issue users encountered was that the icons next to each recipe card were not filled in, leading to some confusion.

### Issues discovered from user testing
1. Recipe checkboxes are confusing: does not display which ingredients are required
2. Timer component is not interactive, even though it is a core functionality of our app
3. Bottom navigation needs to be make sense on a couple screens (e.g finish page should not have finish button, next button should be labeled "finish" on last step, redundant buttons on the finish page)
4. The recipes listed on the "Favorites" page should already be starred.
5. User could not get the desired result by searching keywords. Need a way to filter by occasion/meal type.

## Future improvements
- If we had more time, we would like to fully implement the the "suggested for you" feature on the homescreen of our app. This feature would take into account previous recipes cooked and/or favorited by users, and suggest them recipes that they might like to try. 
- We would also have liked to have a feature that would allow users to add in new recipes, so that other users that used the app would be able to have an even larger pool of recipes to choose from
