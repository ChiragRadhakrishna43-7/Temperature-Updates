# Temperature-Updates

<p align="justify"> Temperature/Weather updates for a particular place using Node JS</p>

## Description

<p align="justify">The Node.js application creates a simple weather application using the Express Framework. It listens for incoming requests on port 3000 and responds accordingly.</p>

## Steps Involved
<p align="justify"> <br/><b>1. Set up the server to listen on port 3000:</b><br/>
app.listen(3000, function() { ... });: This line starts the server and listens on port 3000. When the server is up and running, it prints "Server is running on Port 3000" to the console.</p>
<p align="justify"> <br/><b>2. Required Modules</b><br/>
<b>express</b>: A web application framework for Node.js.<br/>
<b>https</b>: A module to make HTTP requests.<br/>
<b>body-parser</b>: Middleware to parse incoming request bodies.<br/> </p>
<p align="justify"> <br/><b>3. Create an Express app:</b><br/>
const app = express();: Initialize the Express application.</p>
<p align="justify"> <br/><b>4. Set up middleware for body parsing:</b><br/>
<b>app.use(bodyParser.urlencoded({extended: true}));</b>: This line configures the app to use body-parser middleware to parse URL-encoded data and make it available in req.body.</p>
<p align="justify"> <br/><b>5. Define a route for the root URL ("/"):</b><br/>
app.get("/", function(req, res) { ... });: When a GET request is made to the root URL, the server responds by sending the "index.html" file.</p>
<p align="justify"> <br/><b>6. Define a route for handling form submissions (POST requests to the root URL):</b><br/>
app.post("/", function(req, res) { ... });: When a POST request is made to the root URL, the server extracts the city name from the request body and uses it to construct a URL to the OpenWeatherMap API. The weather information is then displayed on the webpage using the response object.</p>
<p align="justify"> <br/><b>7. Start the server and listen on port 3000:</b><br/>
app.listen(3000, function() { ... });: The server is started and listens on port 3000. When the server is up and running, the message "Server is running on Port 3000" is printed to the console.</p>

<p><i>A front end HTML File is required for executing the application. A basic front-end is designed using HTML which allows the user to enter the preferred city name and get the corresponding updates.</i></p>
