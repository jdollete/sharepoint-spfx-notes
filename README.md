# React-Native notes
Personal notes building SPFX webparts on Sharepoint (on a Apple Mac)

## Dependencies
* NodeJS (Atleast version 6)
* Yeoman
	* `npm install -g yo gulp`
* Yeoman SharePoint generator
	* `npm install -g @microsoft/generator-sharepoint`

## Creating Web Part Project
* Create Folder
	* `mkdir [app-name]`
* Go to root directory
	* `cd [app-name]`
* Run Yeoman Sharepoint Generator
	* `yo @microsoft/sharepoint`
* When Prompted
	* Accept the default [app-name] as your solution name, and then select Enter.
	* Select SharePoint Online only (latest), and select Enter.
	* Select Use the current folder for where to place the files.
	* Select N to require the extension to be installed on each site explicitly when it's being used.
	* Select WebPart as the client-side component type to be created.
	* Accept the default [app-name] as your web part name, and then select Enter.
	* Accept the default [app-name] description as your web part description, and then select Enter.
	* Select "REACT" framework you would like to use, and then select Enter.
* Install the developer certificate
	* `gulp trust-dev-cert`
* Preview Application
	* `gulp serve`
* Correct localhost properties
	* `/config/serve.json`
	* change initial page to `"http://localhost:4321/temp/workbench.html"`

## Libraries
* ESLint
  * npm install --save-dev eslint-config-rallycoding
  * Create .eslintrc file on route directory
  * ` { "presets": ["react-native"] } `
* Firebase
  * npm install --save firebase
* Redux
  * npm install --save redux react-redux
* Redux-Thunk (Used for asynchronous dispatch)
  * npm install --save redux-thunk
* Axios
   * npm install --save axios
* Lodash (Helper method for objects and arrays)
  * npm install --save lodash

## Errors/Troubleshooting
