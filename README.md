This is a Responsive COVID-19 Tracking website built with React JS and Material UI and it can be viewed here:
https://covid19bybikashro.netlify.app/

This functioning related Android app is also built by me: https://github.com/BikashBIOS/COVID-19-Tracker-on-Android (Have a Look at it also.)

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

**API USED** : https://covid19.mathdro.id/api

**API Sample:**
{"confirmed":{"value":211921924,"detail":"https://covid19.mathdro.id/api/confirmed"},"recovered":{"value":0,"detail":"https://covid19.mathdro.id/api/recovered"},"deaths":{"value":4433557,"detail":"https://covid19.mathdro.id/api/deaths"},"dailySummary":"https://covid19.mathdro.id/api/daily","dailyTimeSeries":{"pattern":"https://covid19.mathdro.id/api/daily/[dateString]","example":"https://covid19.mathdro.id/api/daily/2-14-2020"},"image":"https://covid19.mathdro.id/api/og","source":"https://github.com/mathdroid/covid19","countries":"https://covid19.mathdro.id/api/countries","countryDetail":{"pattern":"https://covid19.mathdro.id/api/countries/[country]","example":"https://covid19.mathdro.id/api/countries/USA"},"lastUpdate":"2021-08-23T10:21:22.000Z"}

**DEPENDENCIES TO ADD BEFORE STARTING APP:**

1) npm install --save axios   //for making API requests from the API
2) npm install --save react-chartjs-2   //for making charts
3) npm install --save react-countup    // for the increasing numbers animation
4) npm install --save @material-ui/core   //for using material UI in the application
5) npm install --save chart.js    //for using chart

**PROCESS TO CREATE THIS APPLICATION:**

1) Open Visual Studio
2) type npx create-react-app in the CLI.
3) Add Necessary Dependencies.
4) To run the app, type npm start.
5) Create a src folder (delete if any) and create Index.js, App.js and App.module.css file.
6) In index.js, apply ReactDOM and call the App.js with the id as root.
7) Then, create folders Cards, CountryPicker, Charts in the src/components folder.
8) Create separate JSX and Module Css files for the 3 components.  (eg. Cards.module.css  i.e module is used so that the css is applied for that component only and not other).
9) Write basic JS code for all JS components and import them in the App file.
10) To import all the components is the App, just create another index.js file in components folder and export all the components in that file, and you can use the components now in any JS file, by writing only one line of code.
11) Add necessary code in App css file and apply it in your App.js file to style your components.
12) Now create a new folder API in the src and create a index.js file in that folder.
13) fetch data from the api. using "" constant {data: [variables of api] } = await axios.get(url); return {variables of api}; ""
14) In App.js, retrieve the data and fetch data in componentDidMount() and put the data in the props in the components js files.
15) Material UI used for Card - Card, CardCotent, Typography and Grid.
16) Use CountUp tag for number increasing animation.
17) Use Line Chart in Chart Component to make a graph functionality for Infected and Deaths graphs.
18) Use NativeSelect in the CountryPicker.js to create an array of all countries.
19) Pass the Charts, Cards and CountryPicker into App.js.
20) Apply Bar chart in the Charts file and adjust it in the App.js to display the Bar chart for all the Countries Data.
21) Apply Form Control in the required JS files so that it gets adjusted in the Mobile view also.

**Overview:**
1) App contains data and country.
2) async componentDidMount has fetchData.
3) FetchData is a function in api/index.js to get all the attributes in the api which we only require.
4) Now setting it in the app.js using setState().
5) Handling country change in the app.js, requires the function in CountryPicker.
6) Fetching an array of countries from the api and looping it the FormControl and NativeSelect Material ui components to fetch all the countries.
7) Then applying that function in the App.js by setState.
8) In chart.js, fetchDailyData() is a separate function to create a line chart for the daily data only.
9) To print the countries data, bar chart is used. If global is chose, then it is a line chart and if a particular country is chose, then a bar chart is displayed.
10) In Cards.js, data is coming from index by props which is put in the codes to create a card with increasing animation of the data.
11) Finally, in Index.js of Api, it contains all the functions for separate values of api to be used in all the JS files.

**NOTE - This App was made by Me in my 2nd Year of B.Tech**

Copyright Disclaimer Under Section 107 of the Copyright Act 1976, allowance is made for "fair use" for purposes such as criticism, comment, news reporting, teaching, scholarship, and research. Fair use is a use permitted by copyright statute that might otherwise be infringing. Non-profit, educational or personal use tips the balance in favor of fair use.

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
