Title of App: Stitch Works

Link to Live App: 

<img width="1257" alt="Screen Shot 2020-12-09 at 11 24 56" src="https://user-images.githubusercontent.com/55896961/101677851-fd181100-3a11-11eb-961f-a54e4d42781c.png">

<img width="1269" alt="Screen Shot 2020-12-09 at 11 26 04" src="https://user-images.githubusercontent.com/55896961/101677963-2173ed80-3a12-11eb-8786-3ddf4cf87bde.png">

<img width="1274" alt="Screen Shot 2020-12-09 at 11 25 45" src="https://user-images.githubusercontent.com/55896961/101678123-5f711180-3a12-11eb-94ab-e16d540fa1ac.png">

API Summary: This API has a number of different protected routes making it easy for a logged in user to submit an order as well as give a user with proper admin credentials access to change, add, and delete orders or products. This API securely stores login credentials to MonogoDB and retrieves the user's email and password from the database. Within the project I have integrated the PayPal API as well. This allows the user to connect their PayPal account to the application to make purchases easier for the user. There are also endpoints integrated into the project specifically for filtering products in a number of different ways.

Endpoints: 

Orders:

@route GET api/order @desc Get a list of orders @access Private

@route GET api/order/:id @desc Get a list of orders by ID @access Private

@route DELETE api/order/:id @desc Delete an order by ID @access Private

@route POST api/order @desc Create a new order @access Private

@route PUT api/order/pay @desc Find an order an edit by ID @access Private

Products:

@route GET api/product @desc Get all products @access Public

@route GET api/product/:id @desc Get product by ID @access Public

@route PUT api/product/:id @desc Edit and change products @access Private

@route DELETE api/product/:id @desc Delete a product by ID @access Private

@route POST api/product @desc Post a new product @access Private

Users:

@route PUT api/user/:id @desc Update a user's information @access Private

@route POST api/user/signin @desc Sign in to application @access Public

@route POST api/user/register @desc Register a new user @access Public

@route GET api/user/createadmin @desc Get a list of admins @access Private 


