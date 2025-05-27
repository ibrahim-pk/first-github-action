🚀 How to Create Your First GitHub Actions Workflow
Follow these simple steps to set up your first GitHub Actions workflow:

✅ 1. Go to Your Repository
Open your GitHub repository where you want to add the workflow.

🗂️ 2. Create Workflow Directory
Navigate to the root of your project and create the following directory:
mkdir -p .github/workflows

📝 3. Create Workflow File
Inside the .github/workflows folder, create a YAML file (e.g., main.yml):
touch .github/workflows/main.yml

✍️ 4. Add Basic Workflow Content
  name: First Workflow

on:
  push
  pull_request:
    branches: [ main ]

jobs:
   my-first-job:
    runs-on: ubuntu-latest

    steps:
      - name:Print a message
        run echo "Hello world"

      - name:Cheking 
        run echo "checking"
        
🔄 6. Trigger the Workflow
Push any code or open a pull request to trigger the workflow.

📊 7. Check Workflow Status
Go to your GitHub repository → Actions tab to view the status and logs of your workflow.
