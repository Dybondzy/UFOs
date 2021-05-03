# UFOs

Module 11

Background
Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape.

What You're Creating
This new assignment consists of one technical analysis deliverable and a written report. You will submit the following deliverables:

Deliverable 1: Filter UFO sightings on multiple criteria
Deliverable 2: A written report on the UFO analysis (README.md)
Files
Use the following links to download the Challenge starter code.

Download the starter code. (Links to an external site.)

Deliverable 1: Filter UFO sightings on multiple criteria (80 points)
Deliverable 1 Instructions
Using JavaScript and HTML, you’ll modify the code in your index.html file to create more table filters. In addition to the date filter you created in this module, you’ll add filters for the city, state, country, and shape

Using JavaScript, you’ll replace the handleClick() function in your app.js file with a new function that saves the element, value, and id of the filter that was changed. Then, you’ll create a new function to loop through the dataset and keep only the results that match the search criteria. The webpage will be updated with the search criteria after pressing "Enter".

Follow the instructions below and the numbered comments in the starter code to complete Deliverable 1.

Download the ufo_starterCode.js, rename it app.js, and place it in the js folder of your UFOs GitHub repository. The starter code includes the code used to populate the table from this module.

In the index.html file, remove the list (<li></li>) element that creates the button.
Create four more list elements: city, state, country, and shape. These will be similar to the "Enter Date" list element. Each element should have the same "id" as the object properties in the data.js file.
In Step 1 of the app.js file, create an empty filters variable to keep track of all the elements that change when a search is entered. This variable will be used in Step 5 to store the property “id” and the value that was entered from user input.
Next, you will need to write code for two functions whose names we’ve provided in the starter code, updateFilters() and filterTable().
The updateFilters() function will replace your handleClick() function and update the filters variable you created in Step 1.
The filterTable() function will filter the table data by the value that is entered for the "id" that has changed.
For Step 2, located before the buildTable(tableData) function at the end of the starter code, modify the event listener from this module so that it detects a "change" on each input element and calls the updateFilters() function.
In Step 3, we’ve provided the function, updateFilters(). Inside this function, you’ll write code in Steps 4-5 to update the filters based on user input.
In Step 4a, create a variable that saves the element that was changed using d3.select(this).
In Step 4b, create a variable that saves the value of the changed element’s property.
In Step 4c, create a variable that saves the attribute of the changed element’s id.
In Step 5, write an if-else statement that checks if a value was changed by the user (variable from Step 4b). If a value was changed, add the element’s id (variable from Step 4c) as the property and the value that was changed to the filters variable you created in Step 1. If a value was not entered, then clear the element id from the filters variable.

In Step 6, inside the updateFilters() function, call the filterTable() function that will be used in Step 7.
In the filterTable() function in Step 7, write code to filter the table based on the user input that is stored in the filters variable.
In Step 8, create a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.
In Step 9, loop through the filters object and store the data that matches the filter values in the variable created in Step 8.
In Step 10, rebuild the table with the filtered data by passing the variable created in Step 8.
Deploy the web app on your GitHub pages.
Deliverable 1 Requirements
You will earn a perfect score for Deliverable 1 by completing all requirements below:

The list element that creates the button is removed, and there are five list elements for filtering in the index.html file. (20 pt)
The event listener is modified to detect changes to each filter in the app.js file. (10 pt)
The updateFilters() function saves the element, value, and the id of the filter that was changed. (20 pt)
The filterTable() function loops through all of the filters and keeps any data that matches the filter values. (20 pt)
The webpage filters the table correctly based on user input. (20 pt)
Deliverable 2: A written report on the UFO analysis (README.md) (20 points)
Initialize your repository with a README, and write your analysis of Deliverable 1.

Deliverable 2 Instructions
For your written analysis, be sure to use complete and coherent sentences. Your written analysis should contain three sections, which cover the following:

Overview of Project: Explain the purpose of this analysis.
Results: Describe to Dana how someone might use the new webpage by walking her through the process of using the search criteria. Use images of your webpage during the filtering process to support your explanation.
Summary: In a summary statement, describe one drawback of this new design and two recommendations for further development.
Deliverable 2 Requirements
Structure, Organization, and Formatting (8 points)
The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple paragraphs. (2 pt)
Each paragraph has a heading. (2 pt)
There are subheadings to break up text. (2 pt)
Images are formatted and displayed where appropriate. (2 pt)
Analysis (12 points)
The written analysis has the following:

Overview of the analysis:

The purpose is well defined (2 pt)
Results:

There is a description of how to perform a search, with images. (4 pt)
Summary:

The summary addresses one drawback of this webpage (2 pt)
The summary addresses two additional recommendations for further development (4 pt)
Submission
Once you’re ready to submit, make sure to check your work against the rubric to ensure you are meeting the requirements for this Challenge one final time. It’s easy to overlook items when you’re in the zone!

As a reminder, the deliverables for this Challenge are as follows:

Deliverable 1: Filter UFO sightings on multiple criteria
Deliverable 2: A written report on the UFO analysis (README.md)
Upload the following to your UFOs GitHub repository:

The updated app.js file with the code for the challenge.
The updated index.html file.
The data.js file.
An updated README.md that has your written analysis
To submit your challenge assignment in Canvas, click Submit, then provide the URL of your UFOs GitHub repository for grading.

