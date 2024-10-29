Live Demo: https://yusuf-tosin-lendsqr-fe-test.vercel.app/ This project was bootstrapped with Create React App - Typescript

Tools and packages used
React JS, Typescript, SCSS and Day JS To lauch the app on local environment run git clone https://github.com/Tosinyusuf/lendsqr-fe-test.git npm install npm start

State Management
Context Api was used to manage this App.

Log in
After starting the app the login page comes up first users can either login with a random email and password or use one of the email of the users comming from the mock api e.g yusuftosco@gmail.com with a random password. Login with the user from the mock Api gives an extral user avatar on the the dashboard.

Dashboard
After login user can view different page on the side nav. There is however only one route with enough data which is the USERS routes.

User Page
After login user can view different page on the side nav. There is however only one route with enough data which is the USERS route. On the user page, users will be able to see the users table which connsists of some informations about all sellers. user can filter based on username, organization, email and status.

Pagination was also implmented, user can also see the overview data of all users. the overview data includes: 1, Users: This was generated by counting the number of users coming from the mock endpoint. 2, Active users: This was generated by counting users which thier creation date come before thier last updated date. 3, Users with loan: This was generated by counting users where loan repayment is greater than balance. 4, User with savings: This was generated by counting users where thier balance is greater than thier loan repayement.

Status
The status column was not provided by the Api, But was generated by assigning INACTIVE to users that thier last updated is greater than thier created. PENDING is assigned to other users which thier created date come before thier last updated.

Table Action
User can change the status of a user by clicking on the action button. User can also view the user details.
