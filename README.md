# Project6
## national parks api assignment 

** Why **
An assignment on Thinkful's curriculum. 

** What **
Client-side asynchronous web app
Display a list of national state parks, based on the state and number of results user wishes to see.
Include Park name, a short description about the park, and the url to the park's official website.

** How ** 
Note: you may have to refresh the page in order to do a separate search


** The Insides **
* fetch to NPS API parks endpoint to access list of states available (this will go into the drop-down menu
* within first promise, the loadDropDown function is called which accesses the states to be dipslayed into dropdown menu for user to select
* Once the submit button is clicked, after selecting a state, and a number of results the user wishes to dislplay, the submitButton function is called, which collects the user input data and passes it into the callParksApi function to be called. 
* Once the callParksApi function has been called the appropriate input values are then passed into the fetch url as query parameters to return the parks API data based on the specific state selected and number of results wished to be displayed
* this data then calls for the appropriate results to be displayed
* displayResults function is then run with that given data, and the park names, description, and url can now be accessed using a for loop, to loop through each of the parks and display the amount of parks requested
