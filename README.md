# API Automation with Postman & Newman

Automated API testing suite built with **Postman** and executed via **Newman CLI**, generating both **HTML** and **JSON** test execution reports.

## Setup Project
1. Download .zip file
2. Extract and open folder in VS Code

## Project Structure

```
project-folder/
├── API-Automation.postman_collection.json       # Postman API test collection
├── User-Environment.postman_environment.json    # Environment variables configuration
├── newman/                                      # Auto-generated JSON test reports
└── report.html                                  # Exported HTML test report
```

## How to Run
1. Open new Terminal
2. Run command: newman run API-Automation.postman_collection.json -e User-Environment.postman_environment.json
3. Generate 'report.html'. Run Command: newman run "API-Automation.postman_collection.json" -e "User-Environment.postman_environment.json" -r "cli,html" --reporter-html-export "E:\QA Crash Course\Ostad Course materials\Projects\Project Week 1\Postman Collections\newman-tests\report.html"
4. Generate 'json report'. Run Command: newman run "API-Automation.postman_collection.json" -e "User-Environment.postman_environment.json" -r "cli,json"

## Check Generated Report
1. Open project folder from local drive
2. Double click and open report.html
