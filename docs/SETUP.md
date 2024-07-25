Documenting the Repository Setup Process
1. Create the Main Repository on GitHub
Log in to GitHub:

Go to GitHub and log in to your account.
Create a New Repository:

Click the + icon in the upper-right corner and select New repository.
Name the repository ecommerce-app.
Optionally, add a description and choose visibility (public or private).
Optionally, initialize with a README or leave it unchecked.
Click Create repository.


2. Clone the Main Repository Locally
Open Terminal:

Locate Terminal in Applications > Utilities, or search for it using Spotlight.
Navigate to Your Projects Directory:

bash
Copy code
cd ~/Projects
Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/ecommerce-app.git
cd ecommerce-app


3. Create Subdirectories for Backend and Frontend
Create Directories:

bash
Copy code
mkdir ecommerce-backend ecommerce-frontend
Add Initial Files and Commit Changes:

For Backend:

bash
Copy code
cd ecommerce-backend
touch README.md
git add README.md
git commit -m "Initial commit for backend project"
For Frontend:

bash
Copy code
cd ../ecommerce-frontend
touch README.md
git add README.md
git commit -m "Initial commit for frontend project"


4. Push Changes to GitHub
Push Changes from the Main Directory:

bash
Copy code
cd ..
git add .
git commit -m "Add backend and frontend directories"
git push -u origin main


5. Troubleshoot Authentication Issues
If You Encounter Authentication Issues:
Generate a Personal Access Token (PAT):

Go to GitHub Settings.
Generate a new token with the appropriate scopes.
Copy the token and keep it secure.
Update Git Credentials:

bash
Copy code
git remote set-url origin https://<username>:<personal-access-token>@github.com/your-username/ecommerce-app.git
Clear Cached Credentials (if needed):

bash
Copy code
git credential-cache exit
Push Again:

bash
Copy code
git push origin main
6. Verify the Repository on GitHub
Check the Repository:
Go to your GitHub repository page and refresh to see if the directories and files appear correctly.
