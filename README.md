# React-NET-CORE

## Description

>This App is a proof of concept to show the interaction of React with a .NET MVC Backend.
>This solution implements the tutorial: 
[Tutorial: Create an ASP.NET Core app with React in Visual Studio](https://learn.microsoft.com/en-us/visualstudio/javascript/tutorial-asp-net-core-with-react?view=vs-2022)

## Built With

- React JS 
- .NET C#
- HTML 
- CSS

## Project Set up

Clone Repository using

`git clone https://github.com/NeckerFree/React-NET-CORE`

Move into project directory

`cd React-NET-CORE`

Open app the app Visual Studio 2022

### Set the statup project

1. In Solution Explorer, right-click the solution name and select Set Startup Project. Change the startup project from Single startup project to Multiple startup projects. Select Start for each project’s action.

2. Next, select the backend project and move it above the frontend, so that it starts up first.

- The app ask to select a different port:
    - Something is already running on port 3000
    - Would you like to run the app on another port instead? » (y/n)
- Enter `Y` and the app open in the browser in next free port, for example:
- `http://localhost:3001`

### Start the project
1. Before you start the project, make sure that the port numbers match. Go to the launchSettings.json file in your ASP.NET Core project (in the Properties folder). Get the port number from the applicationUrl property.

If there are multiple applicationUrl properties, look for one using an https endpoint. It should look similar to https://localhost:7049.

2. Then, go to the setupProxy.js file for your React project (look in the src folder). Update the target property to match the applicationUrl property in launchSettings.json. When you update it, that value should look similar to this:

target: 'https://localhost:7049',
To start the project, press F5 or select the Start button at the top of the window. You will see two command prompts appear:

The ASP.NET Core API project running
npm running the react-scripts start command

You should see a React app appear, that is populated via the API.

## Authors:

👤 **Elio Cortés**

- GitHub: [@NeckerFree](https://github.com/NeckerFree)
- Twitter: [@ElioCortesM](https://twitter.com/ElioCortesM)
- LinkedIn: [elionelsoncortes](https://www.linkedin.com/in/elionelsoncortes/)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

Feel free to check the [Issues page](https://github.com/NeckerFree/React-NET-CORE/issues).

## Show your support

Give a ⭐️ if you like this project!

## 📝 License

This project is [MIT](./LICENSE) licensed.