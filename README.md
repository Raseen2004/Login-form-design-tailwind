This document is for setup the tailwindcss in the project.

step 1: npm init
step 2: npm install -D tailwindcss
step 3: npx tailwindcss init
step 4: "./src/**/*.{html,js}" (place this inside the content in the tailwind.config.js file for the tailwind is working in those files)
step 5: (optional)create folder called dist and change the content to "./dist/**/*.{html,js}" in the tailwind.config.js file
step 6: Create src and inside the create input.css
step 7: inside the input.css insert this lines of code: 
       "@tailwind base;
	@tailwind components;
	@tailwind utilities;"
step 8: npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch (this command is used for run the tailwindcss in the files)
step 9: insert the link tag for adding output.css in the html file
step 10: "scripts": { } add the "dev": tailwindcss -i ./src/input.css -o ./dist/output.css --watch" because using this to not run every time this command to the terminal
step 11: npm run dev
