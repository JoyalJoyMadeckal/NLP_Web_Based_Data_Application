OneDrive link for the models (Pre-trained Word2Vec Model and Logistic Regression Model) - https://rmiteduau-my.sharepoint.com/:f:/r/personal/s3860476_student_rmit_edu_au/Documents/COSC2820%20Assignement%202%20Web%20Based%20Application?csf=1&web=1&e=FOe2Dp


Web App Documentation

Home Page
	Static UI
		-> Displays "RMIT Job Shop" as heading and its a hyperlink that routes to the home page itself
		-> "Post Jobs" and "Employer Login/Logout" buttons on the right side
		-> Search box is below the buttons and have a placeholder "Enter Search Text".
		-> The different job categories and about page is give below as a navigation list. Each item is a hyperlink that routes to the respective routes
		-> The content consists of two job ads display from each of the job categories including images.
	Functionalities
		-> When user clicks on "RMIT Job Shop" they will be redirected to home page from whichever route user is in
		-> When user clicks on "Post Jobs" they will be routed to login page if not logged in otherwise will be routed to the post jobs page having a form
		-> When user click on "Employer Login" they will be routed to login page.
		-> If the employer has logged in the "Employer Logout" button will be shown and if not logged in "Employer Login" button will be shown.
		-> The design for placing "Employer Login/Logout" and "Post Jobs" side by side is obtained form "EthicalJob.com.au"
		-> User can type text in the search box and press Enter or click on the search icon at the end to enable searching
		-> The items on the navigation list will take the user to respective routes when clicked
		-> The selected item in the navigation list will be highlighted.
		-> User can click on any of the jobs displayed on the home page and it will take the user to the full description of the advertisement.
		
Category Page
	Static UI
		-> User can see the list of jobs in the category he selected with a shorter description,company name, title, image and Job ID.
		-> User can click on any of the job advertisement and it will show the full description of the advertisement including Salary and Company if specified.
		-> User can also see that the current category is highlighted in sky blue colour
	Functionalities
		-> User can click on any of the listed job advertisements and it will take the user to the full description of the advertisement.

Contact Us Page
	Static UI
		-> User can see a set of images indicating how communication can be made - Email, Whatsapp, Call, Location.
	Functionalities
		-> The images show are flip cards.
		-> When user hover over any of the images it will flip and show the information.
		
Login Page
	Static UI
		-> There will be two input text boxes for user name and password
		-> Password will be shown as black dots when the user types the password
		-> A login button at the bottom
	Functionalities
		-> User can type the user name and password.
		-> When user clicks on the login button the data will be validated with some hard coded values and login will happen
		-> If the login is unsuccessful a message will be shown to the user "Username of password is invalid."
		-> If login is successful, user will be redirected to post jobs page

Post New Job Page
	Static UI
		-> The page will have 4 fields - Title (Mandatory), Salary, Company and Description (Mandatory)
		-> The "Classify" button will be below the fields
	Functionalities
		-> When user clicks on "Classify", the predicted category will be shown as a message below "Classify" button and "Post Job" button
		-> Also, there will be a dropdown with the list of categories available.
		-> The dropdown will be set to the predicted category value by default
		-> User can override the predicted category by selecting the category from the dropdown.
		-> Once the user is fine with the category, he can click on the "Post Job" button. The job will be posted and user will be redirected to the job
		-> The backend code will assign a random 5 digit id to the new job
		-> The posted job will be available in the corresponding category and it can also appear in the search results.
		
Search Page
	Static UI
		-> The number of matched advertisements will be displayed as a message
		-> The page will display maximum of 10 advertisements
		-> The list of the advertisements will be shown.
		-> If there are no matching advertisements then proper message will be shown to the user - "No matching advertisements found."
	Functionalities
		-> User can click on the advertisements to see the full description of the advertisement.
		
Error Pages
	-> If the user is giving an invalid URL or if the server encounters any errors proper messages are shown to the user.