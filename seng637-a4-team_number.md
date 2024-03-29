**SENG 637 - Dependability and Reliability of Software Systems**

**Lab. Report \#4 – Mutation Testing and Web app testing**

| Group \#:      |     |
| -------------- | --- |
| Student Names: |     |
|                |     |
|                |     |
|                |     |

# Introduction

# Analysis of 10 Mutants of the Range class 

# Report all the statistics and the mutation score for each test class

# Analysis drawn on the effectiveness of each of the test classes

# A discussion on the effect of equivalent mutants on mutation score accuracy

# A discussion of what could have been done to improve the mutation score of the test suites

# Why do we need mutation testing? Advantages and disadvantages of mutation testing

# Explain your SELENUIM test case design process
6. Update Quantity in Cart
      Objective: Ensure that the user can update the quantity of an item in the cart and that the cart updates correctly.
      Steps: Add an item to the cart, navigate to the cart, update the quantity of the item, and confirm the update.
      Expected Result: The quantity of the item updates correctly, and the cart reflects the new quantity and total price.
7. Switch Lanuage from English to French
      Objective: Ensure that the website correctly switches the interface language from English to French upon user selection
      Steps: Find the lanuage seletion option and select "French" from the available options
      Expected Result: The website content, like navigation menus switches to French
8. Change store location 
       Objective: Ensure that users can successfully change their default store location on the website.
       Steps: Navigate to the store selection area, select a new store, confirm the selection and then verify the change.
       Expected Result: Verify that the display name of the store (often found at the top of the webpage or within the store selection area) updates to reflect the newly selected store.
9. Navigate to a Specific Department
     Objective: Ensure the user can navigate to a specific department from the homepage.
     Steps: From the homepage, click on a department category (e.g., "Appliances").
     Expected Result: The website redirects to the selected department page showing relevant products and categories.
10. Use the Site Search with a Blank Query
     Objective: Ensure the search functionality handles blank queries gracefully.
     Steps: Go to the search bar, enter nothing (leave it blank), and press enter or click the search icon.
     Expected Result: The website either prompts the user to enter a search term or displays a message indicating no search term was entered.
# Explain the use of assertions and checkpoints
## For the "Update Quantity in Cart" objective
1. Verify Item Quantity Updates for 
   After updating the quantity of an item in the cart, assert that the displayed quantity matches the new amount. This verifies that the input for quantity change is correctly processed and displayed. "assert text" was used as the assertion command
2. Check for Correct Cart State
   After updating the quantity of an item in the cart, assert that the displayed quantity of the amount of items in the cart refelct correctly. This verifies that the input for quantity change is correctly processed and displayed. "assert text" was used as the assertion command
## For the "Switch Lanuage from English to French" objective
1. Check Navigation Menu Text
   After changing from English to french verify if the main page title changes once you click any department. The command used was "assert text"
2. Validate English option is available
   After French is selection, a user should have the option to switch back to English right away. The command used was "assert text"
## For the "Use site search with a blank query objective"
1. Check if the Front page title changes
   With the home depot website, if a blank query is sent no change happens. So we used an "assert text" to see if any changes were made on the front made
## For the "Changing the default store location"
1. Store Name Update: Verify the display name of the store is the newly selected store using 'assert text'
2. Selection is consistent across sessions/pages: Verify that if you navigate to different pages or refreshing the pages keeps the new store selection. This would use 'assert text'

## For the "Navigating to a specfic department"
1. Validate Specfic department name
   Once the page has been changed to a new department use 'assert text' to check if the name has been updated correctly. 

# how did you test each functionaity with different test data
1. Update Quantity in Cart
For this test case, we played with different quanitites to update the cart with such as 3 and to see if this was correctly being reflected

2. Switch Language from English to French
Here, the variation in test data could involve switching to different languages supported by the website, not just French. So instead of French we could have pickd Spanish, Arabic etc however HomeDepot website did not support other lanuages. 

3. Change Store Location
The test case aimed at verifying the "Change Store Location" functionality encountered challenges that led to its incompletion, primarily revolving around the dynamic nature of content changes upon selecting different store locations.

4. Navigate to a Specific Department
Testing navigation to different departments ensures that all sections of the website are accessible and load correctly.

5. Use the Site Search with a Blank Query
Another good test would be valid search term or invalid search terms or special characters. The test was not completed as dynamic id's was used for the search box. Some web applications generate dynamic IDs for their elements. A dynamic ID changes every time the page is loaded, which means hardcoding the ID in your test will lead to inconsistencies and failures.

# How the team work/effort was divided and managed

# Difficulties encountered, challenges overcome, and lessons learned
Dynamic Content Handling: One of the significant challenges was dealing with dynamic content changes, such as inventory updates or location-specific information, which required adaptive testing strategies.
Element Locators Stability: Finding stable element locators was challenging, especially when dealing with dynamic IDs and classes that change with each session or are affected by the page's state.
# Comments/feedback on the assignment itself
