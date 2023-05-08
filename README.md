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
- Step 1 [design_ui_selection]: Each item should have a checkbox, but it should only be visible on the user's profile page.
- step 2 [manage_selected_items_state]: It's time to connect it to the Redux store and keep track of which items have been checked or unchecked.
- step 3 [delete_button_to_update_state]: Create a button component which will update the state and render only if there are items selected.
- step 4 [delete_button_to_trigger_request]: Now modify the button to trigger a request to an endpoint and send the selected items.
- Step 5 [create_api_endpoint]: Implement a new API endpoint that can receive requests to delete items and validate that the user who sent the request is the same user who uploaded the items.


## Textbook solution
For each step, describe all actions the user needs to perform to complete the step, including links to PRs as they would need to be written to pass checks. 
Before submitting your quest for review, test your quest in snack and check the instructions you wrote. Make sure that by following these instructions, you are able to successfully complete the quest.  
### Instructions for completing the quest: 
#### Step 1 [design_ui_selection]:
- Learning Objective: Checking the user path with React Router DOM and perform conditional rendering 
- Narrative: The senior developer explains why implementing a feature to delete multiple items with a single click can improve customer experience and requests to add checkboxes to be rendered inside each item only on the profile page.
- Instructions: Render each item alongside a checkbox and check if the user is in the profile path.
- How do users pass to the next step: Open a PR after completing the task
- Hints:

#### Step 2 [manage_selected_items_state]:
- Learning Objectives: Adding actions to redux 
- Narrative: The senior developer requests that we need keep track of selected items, enabling the removal or addition of items. 
- Instructions:  Add proper actions types, reducer cases, and dispatch actions.   
- How do users pass to the next step: Open a PR after completing the task
- Hints:

#### Step 3 [delete_button_to_update_state]:
- Learning Objectives: Conditional rendering and adding actions to redux.   
- Narrative: The senior developer requests now to create a button component which can update the redux state and to be visivle only if the user has selected at least one item.
- Instructions: Create a button inside the list item with the ID attribute 'delete-selected'. This button should only be visible if there are selected items, and clicking it should remove those items from the state.
- How do users pass to the next step: Open a PR after completing the task
- Hints

#### Step 4 [delete_button_to_trigger_request]:
- Learning Objectives: Triggering request and component update    
- Narrative: The senior developer requests to add a new function to `agent.js` file in order to send the request to '/items/deleteItems' endpoint and to update the delete button component to trigger the action. 
- Instructions: Create a new function in agent.js that takes an array of selected items as input. Update the delete button component to trigger this function and update the state accordingly.
- How do users pass to the next step: Open a PR after completing the task
- Hints

#### Step 5 [create_api_endpoint]: 
- Learning Objective: Creating an API endpoint and perform validations.
- Narrative: The senior developer explains why implementing a feature to delete multiple items with a single click can improve the customer experience, and requests to add a new enpoint and perform proper validations.
- Instructions: Create an endpoint to handle an array of items and validate the seller ID property of each item against the user's ID who sent the request.
- How do users pass to the next step: Open a PR after completing the task
- Hints:



