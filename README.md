# create-react-app

This package includes the global command for [Create React App](https://github.com/facebook/create-react-app).<br>
Please refer to its documentation:

- [Getting Started](https://facebook.github.io/create-react-app/docs/getting-started) – How to create a new app.
- [User Guide](https://facebook.github.io/create-react-app/) – How to develop apps bootstrapped with Create React App.

Documentation for changes to create-react-app

The changes to package.json has been done to do following task 
1. when npm install is done , a message is given to take backup of package.json whenever npm audit fix --force is done
this is done to safeguard updates to package.json by audit fix command ( as not all developers may be using github )

2. whenever user gives the command npm audit fix or npm audit fix --force , a backup gets created in the project folder for package.json before update by audit fix or audit fix --version.


since dependencies are version oriented it is better to inform developer such changes may impact his development effort and logic

3. similar logic needs to be implemented for create-react-app with vite as well

