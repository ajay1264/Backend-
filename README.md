#backend creation

first command: npm init 
then create a .gitignore file 
then go to gitignore generator and search node then cv it 
then create three files app constants and index.js 
then add "type": "module",  in your package.json
then run nodemon for the file reload easily the cmd is npm i -d nodemon
then replace "test" to "dev": "nodemon src/index.js 
then we have to create folder in the src file to create at one [controllers, db, middleware, models, routes, utils]
"controllers", "db", "middlewares", "models", "routes", "utils" | ForEach-Object { New-Item -Path . -Name $_ -ItemType Directory }
then run the prettier cmd that is npm i -d 
then create a file .prettierrc and add the rules you have to follow :
{
"singleQoute": false,
"bracketSpacing": true,
"tabWidth": 2,
"trailingComa": "es5",
"semi": true

}
then again create a new file .prettierignore and add what not to prettier 
/.vscode
/node_modules
./dist

*.env
.env
.env.*