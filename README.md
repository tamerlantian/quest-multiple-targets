# Multiple Targets

## Quest Details 
#### title: Multiple Targets
#### level: Advanced
#### skills: Frontend, Backend, Database
#### dependencies: docker_localsetup


## Overview 

This quest is about implementing a new feature to allow customers to select and delete multiple items with a single click.  


## Outline
Describe each step in the quest. 
- Step 1 [create_api_endpoint]: Implement a new API endpoint that can receive requests to delete items and validate that the user who sent the request is the same user who uploaded the items.
- Step 2 [design_ui_selection]: Each item should have a checkbox, but it should only be visible on the user's profile page.
- step 3 [connect_to_redux_store]: It's time to connect it to the Redux store and keep track of which items have been checked or unchecked.
- step 4 [integrate_backend_and_frontend]: Create a button component whose main function is to trigger a request to delete the checked items."


## Textbook solution
For each step, describe all actions the user needs to perform to complete the step, including links to PRs as they would need to be written to pass checks. 
Before submitting your quest for review, test your quest in snack and check the instructions you wrote. Make sure that by following these instructions, you are able to successfully complete the quest.  
### Instructions for completing the quest: 
#### Step 1 [create_api_endpoint]: 
- Learning Objective: Creating an API endpoint and perform validations.
- Narrative: The senior developer explains why implementing a feature to delete multiple items with a single click can improve the customer experience, and requested that a new endpoint be added with proper validations.
- Instructions: Create an endpoint to handle an array of items and validate the seller ID property of each item against the user's ID who sent the request.
- How do users pass to the next step: Open a PR after completing the task
- Hints:

 
#### Step 2 [design_ui_selection]:
- Learning Objective: Checking the user path with React Router DOM and perform conditional rendering 
- Narrative: The senior developer requests that the checkbox be rendered inside each item only on the profile page.
- Instructions: Render each item alongside a checkbox and check if the user is in the profile path.
- How do users pass to the next step: Open a PR after completing the task
- Hints:

#### Step 3 [connect_to_redux_store]:
- Learning Objectives: Learning redux ecosystem 
- Narrative: The senior developer requests that we need keep track of selected items, enabling the removal or addition of items. 
- Instructions:  Add proper actions types, reducer cases, and dispatch actions.   
- How do users pass to the next step: Open a PR after completing the task
- Hints:

#### Step 4 [integrate_backend_and_frontend]:
- Learning Objectives: Integrating frontend and backend, and component creation
- Narrative: The senior developer requests now to create a button component to trigger the deletion of selected items.
- Instructions: Create a button in the list item with the id attribute 'delete-selected'. Also, add a new reducer case to remove selected items and send a request to the recently created endpoint.
- How do users pass to the next step: Open a PR after completing the task
- Hints
