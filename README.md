# Postman API Automation Integration with GitHub Actions #

Thi repository is a demostration for POC for integrating postman tests with github actions. The tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The reports runs on the scheduled time with the help of the cron.

The HTML Report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page:  ``` https://pravalikabariki.github.io/Phoenix-Inwarranty-Flow/ ```
The latest report is mailed to the team members using GMAIL SMTP.


## About Me ##
Hi, My name is Pravalika Bariki. I have 3+ yrs of experience in Automation Testing. My Skillset Inculdes UI Automation with Selenium Webdriver, Playwright and for API Testing. I use Postman.
You can connect me over LinkedIN: https://www.linkedin.com/in/pravalikabariki/

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edgecase Testing
3. Token Testing
4. Data Driven Testing with CSV
5. Schema Validation
6. Secrets Management with GitHub Secrets

## Tech Stack ##
1. Postman
2. Nodejs 22v
3. Newman
4. Newman-reporter-htmlextra
5. Github Actions
6. Gmail SMTP
7. Github Pages
8. CSV for Data Driven Testing
9. AWS-EC2 Instance for self hosted github runner.

## GitHub Pages ##
You can directly view the latest test report of the Postman Test at the Github Page Link: ''' https://pravalikabariki.github.io/Phoenix-Inwarranty-Flow/ '''

## Project Structure ##   
```
Phoenix Inwarranty Flow
├─ Inwarranty-flow-connection.postman_collection.json
├─ newman-report.png
├─ QA.postman_environment.json
└─ testdata.csv

```

## How to run the project? ##
You can run the project on your local system for that:
1. Clone the project on Local System: ``` https://github.com/PravalikaBariki/Phoenix-Inwarranty-Flow.git ```
2. Install Nodejs and npm from ``` https://nodejs.org/en ```
3. Install Newman using ``` npm install -g newman ```
4. Install Newman-reporter-htmlextra ``` npm install -g newman-reporter-htmlextra ```
5. Run the Newman Command:
 ```
  newman run 'Inwarranty-flow-connection.postman_collection.json' \
  -e QA.postman_environment.json \
  -d testdata.csv \
  -r cli,htmlextra \
  --reporter-htmlextra-export ./newman/index.html
```

## HTML Report ##
The Report will be created in the newman folder
![Postman_Report](https://github.com/PravalikaBariki/Phoenix-Inwarranty-Flow/blob/main/newman-report.png)


             








































