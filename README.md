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
  Tauri - for creating native app w/ web frontend
  Rust - coding language for core code
  Vue - frontend framework
  Django - backend framework


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
 
  * Frontend - TBD
    *   **Home Route**: Route path="/"
    *   **Index Route**: Route path="/aok"
    *   **Show Route**: Route path="aok/:id"
    *   **Create Route**: Route path="create"
    *   **Update Route**: Route path="update/:id"
    *   **Delete Route**: Route path="delete/:id"
        
### Vue Component Structure

-> App

 	-> Header
		-> Button - To be able to create a new Brain Dump from any view.
	
	-> Outlet
		-> Index
			-> Card - a single Brain Dump, displayed in descending chronological order w/ time created and size.
		-> Show 
			-> Button - to navigate to AoK's Update view.
			-> Button - to run the Delete AoK function.
		-> Create
			-> Form - adds an item and refreshes upon 'submitting'
	
		-> Update - updates timestamp and allows to extend an already-created brain dump.
			-> Single Form - to add one additional item at a time


### Mockups!

![Index Mockup](TBD)
![Show Mockup](TBD)
![Create/Update Mockup](TBD)

### Reference

[Markdown Reference](https://www.seevividly.com/images/Markdown_Reference.png)

[Rust, Tauri, SolidJS Tutorial](https://blog.logrocket.com/rust-solid-js-tauri-desktop-app/)

Link Template
[]()


### Stretch Goals
* Get running on Android
