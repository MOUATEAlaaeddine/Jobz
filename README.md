🚀 Jobz - Job Management API
A .NET 7 Web API for managing job offers, candidates, companies, and applications.

📋 Prerequisites (macOS)


.NET 7 SDK - Download here
Visual Studio for Mac or VS Code
Git

Check your .NET version:
bashdotnet --version
# Should show 7.x.x


🔧 Setup Instructions


1️⃣ Clone the Repository
bashgit clone https://github.com/MOUATEAlaaeddine/Jobz.git
cd Jobz


2️⃣ Restore Dependencies
bashdotnet restore



3️⃣ Update Database (after migrations are added)
bashdotnet ef database update


4️⃣ Run the API
bashdotnet run
The API will start at: http://localhost:5000 or https://localhost:5001


🧪 Testing the API

Example: Create a Candidate

bashcurl -X POST http://localhost:5000/api/candidats \


  -H "Content-Type: application/json" \

  
  -d '{"nom": "Mouate","prenom": "Alaaeddine","email": "alaa@example.com","telephone": "+212600000000"

  
  }'
  
Example: Get All Job Offers

bashcurl http://localhost:5000/api/offres




🛠️ Development Commands


Build the project
bashdotnet build
Run tests
bashdotnet test
Create a new migration
bashdotnet ef migrations add MigrationName
Update database
bashdotnet ef database update
Clean build artifacts
bashdotnet clean
rm -rf bin obj


📦 Technologies Used


.NET 7 - Framework
ASP.NET Core Web API - REST API
Entity Framework Core - ORM
SQLite - Database (development)
xUnit - Testing (coming soon)



🌿 Git Workflow
Work on a feature branch
bashgit checkout -b feature/your-feature-name
# Make changes
git add .
git commit -m "Add: description of changes"
git push -u origin feature/your-feature-name

📝 Current Status
✅ Project setup
🔄 Adding domain models
⏳ Creating API endpoints
⏳ Adding tests
⏳ Adding authentication

👨‍💻 Author
Alaaeddine Mouate
GitHub: @MOUATEAlaaeddine

📄 License
This project is for educational purposes.
