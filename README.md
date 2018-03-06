# Web-Starter-Kit
Start your new website project with this package (there is all you need in it). The package contains :
- Bootstrap 4
- Popper.js
To add jQuery, open the terminal and copy and paste this line :
```
npm install jQuery
```
## Getting Started
### Requirements
To use the package, you need to install npm
Follow this link to install npm : https://nodejs.org/en/
### Step 1 : Download the package
Obviously, you need to download the package to start using it... I suppose you already did.
### Step 2 : Create your first pages
I recommend you to create all your files (HTML pages) in the public folder. Create your index.html and import main.css from /public/css.
If you put index.html in the public folder, it must look like this :
```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>My title</title>
	<link rel="stylesheet" type="text/css" href="css/main.css">
</head>
<body>
	
</body>
</html>
```
To add scripts, add a js folder in the public folder to. If you want to use more libraries. Prioritize using npm to install them, it will give you full control on the versions of the libraries.
### Step 3 : Add CSS and modify Bootstrap 4 with SASS
If you want to add more css. Edit the main.scss file in the scss folder. You can import bootstrap in this file and edit the properties of Bootstrap 4. Change the variables of Bootstrap 4 before importing it.<br />
For example, we want to make the primary color become black. your main.scss would look like this :
```scss
$primary = #000000

@import "../node_modules/bootstrap/scss/bootstrap";

#my-element {
  display:block;
}
```
### Step 4 : Compile with Sass
If you just want to compile once, you only need to type :
```
npm build-css
```
If you want it to compile automatically on change of main.scss, just type :
```
npm watch-css
```
Now, everytime you save changes made to main.scss, it will compile automatically and generate the main.css.
