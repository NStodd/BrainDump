##### Nate's Capstone Project
## Brain Dump!

_Everyone's got a brain, everyone's gotta dump._


### App Description
  An easy-to-approach interface through which a user can create Brain Dumps. A Brain Dump is a session, containing a list of easily-parsible elements. Each session contains a list of things that the user can input in rapid succession on either a web or native interface.
  A user can review the time, size and sequence of their previous Brain Dumps, as well as review the elements in any of the Brain Dumps they have done.

### Models
  There are two data models for "Brain Dump!"
    1. The Brain Dump (Session) Object - representing each instance of a user creating a list of items.
      1. The time/date that the Session was created. (using the native Time Object)
      1. An Array of Items captured within that particular session. ()
    2. The Item Object
      2. The Item Name (a String, inputted by the user)

### Technologies
  


### List of Routes
  * Backend
    *   Brain Dump Index - GET from '/braindumps/'
    *   Brain Dump Show/Item Index - GET from '/braindumps/:id'
    *   Item Show (might not be its own page) - GET from '/braindumps/:id/:item'
    *   Create Brain Dump - POST to '/braindumps/'
    *   Create Item - POST to '/braindumps/id/'
    *   Delete Brain Dump - DELETE to '/braindumps/:id'
    *   Delete Item - DELETE to '/braindumps/:id/:item'
    *   Update - POST to '/braindumps/:id/:item'
 
  * Frontend
    *   **Home Route**: Route path="/"
    *   **Index Route**: Route path="/aok"
    *   **Show Route**: Route path="aok/:id"
    *   **Create Route**: Route path="create"
    *   **Update Route**: Route path="update/:id"
    *   **Delete Route**: Route path="delete/:id"
        
### React Component Structure

-> App

 	-> Header
		-> Button - To be able to create a new AoK from any view.
	
	-> Outlet
		-> Index
			-> Post - a single AoK, displayed in descending chronological order.
		-> Show 
			-> Button - to navigate to AoK's Update view.
			-> Button - to run the Delete AoK function.
		-> Create
			-> Form - 3 text fields and a submit button
	
		-> Update
			-> Form - same 3 text fields and a submit button


### Mockups!

![Index Mockup](https://i.imgur.com/MJB3LNp.png)
![Show Mockup](https://i.imgur.com/teGcqxp.png)
![Create/Update Mockup](https://i.imgur.com/TIZSBBE.png)

### Reference
[Project 4 Requirements](https://turmeric.seircohort.com/unit-projects/unit-four-project-requirements/)

[Markdown Reference](https://www.seevividly.com/images/Markdown_Reference.png)

[Turmeric Django React Frontend Lecture PDF](https://turmeric.seircohort.com/second-language/week-22/day-2/lecture-materials/react)

[Turmeric Django API Lecture PDF](https://turmeric.seircohort.com/second-language/week-22/day-1/lecture-materials/djangoapi)
