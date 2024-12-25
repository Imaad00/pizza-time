# Pizza Time
Internship Project

![Pizza Time preview](https://github.com/catherineisonline/pizza-time-with-react/blob/main/src/assets/images/project-preview.png?raw=true)

Pizza Time: A delicious online experience. I designed and developed an e-commerce platform for this pizza restaurant, featuring an interactive menu with a variety of options including pizza, sushi, and pasta. Simplifying the online ordering process and providing a seamless user experience was the key goal of this project.

An e-commerce platform tailored for the gastronomy industry. I led end-to-end design and development, utilizing technologies like React Icons, React Router DOM, React Alice Carousel, Leaflet Maps, React Paginate, UUID, React Lazy Load, and Framer Motion.

🍕 Dynamic Culinary Hub:
Fictional restaurant featuring an extensive menu including pizzas, sushi, and pasta. Used React components like Icons, Router, and Carousel for easy navigation and user interface.

📍 Spatial Awareness with Leaflet Maps:
Used Leaflet Maps API to provide geographical insights, enhancing user interaction and store location understanding.

🎨 UI Efficiency via Pagination and Motion:
Employed React Paginate for user-friendly menu page division, optimizing exploration. Framer Motion added smooth animations, enhancing visual appeal and interaction.

🆔 Efficient Data Management:
UUID for unique ID generation ensures robust menu item and order identification. React Lazy Load optimizes image/component loading, boosting site performance.

💾 Data Integrity with Turso:
Implemented libSQL client for a reliable database backend, securing transactions and user data. Turso ensures scalable SQLite database operations.

🛒 Streamlined Ordering via Express.js:
Developed Express.js-based ordering system for smooth cart management, item addition/removal, and quantity updates.

👤 Personalized User Interaction:
Enabled user registration, login, and profile management. Users modify and delete profiles, enhancing customization.

📧 Secure Communication via reCAPTCHA:
Integrated Google reCAPTCHA to verify contact form users, curbing spam and ensuring secure communication.

## Getting Started with Create React App <a id="gettingStarted"></a>

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

To get started you need to:

1. Clone the project
2. npm install
3. Install listed dependencies
4. Use available scripts, like npm start

## Instructions <a id="instructions"></a>

- When you fork or download the project install node modules using npm install and then any additional dependencies you don't have from <a id="dependencies">Dependencies</a> list

- Next, you need to create the file name .env located outside the src file

- In the .env file I am using several variables:
1. REACT_APP_TURSO_DB_URL, REACT_APP_TURSO_DB_TOKEN & MYSQL_ATTR_SSL_CA - these variables contain information that will connect you to the Turso database. You can use the following [documentation](https://docs.turso.tech/sdk/ts/quickstart). If you use any other database you need to use the according information to connect to that database. The token can be created after registration.
Note that the table for users in my case is named "users" and contains the following data: id | email | password | fullname | address | number.
2. REACT_APP_USERS_URL - this is a url for Node.js server. First, it's better to run it locally and only then switch to whatever you want. If you want to run the server locally the value of this variable should be http://localhost:3000/users. In this project I set up backend using Vercel. You can google "How to Deploy Your Node.js Backend Project to Vercel" and set up your own backend.
3. REACT_APP_CAPTCHA_URL - the same logic works for this backedn url which this time is used for captcha verification. Locally, the url value should be http://localhost:3000/verify-recaptcha.
4. REACT_APP_CAPTCHA_KEY & REACT_APP_CAPTCHA_SECRET - both values can be found once you create an account for reCaptcha at https://www.google.com/recaptcha/about/. Please use their documentation for better understanding.

- Once you set up the variables, you can run the server on one port, if you use local server and the website on another port. 

## Available Scripts <a id="scripts"></a>

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.


## Database <a id="database"></a>
To use the registration functionality for your own project, you need to use your own database. You can use any SQL database you wish and you adapt it to this project. I am using [Turso](https://turso.tech/) database. To have your own database you need to register and set it up by provided information. I recommend you to use their [documentation](https://docs.turso.tech/sdk/ts/quickstart).


## Used Dependencies <a id="dependencies"></a>

- [React Icons](https://www.npmjs.com/package/react-icons)
- [React Router DOM](https://www.npmjs.com/package/react-router-dom)
- [React Alice Carousel](https://www.npmjs.com/package/react-alice-carousel)
- [Leaflet Maps](https://react-leaflet.js.org/docs/start-installation/)
- [React Paginate](https://www.npmjs.com/package/react-paginate)
- [uuid - Random id generator](https://www.npmjs.com/package/uuid)
- [Tilt](https://micku7zu.github.io/vanilla-tilt.js/)
- [React Lazy Load](https://www.npmjs.com/package/react-lazy-load-image-component)
- [Framer Motion](https://www.framer.com/motion/)
- [MySQL2](https://www.npmjs.com/package/mysql2)
- [libsql](https://www.npmjs.com/package/@libsql/client)

Happy coding!
