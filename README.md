# DevOpsHomework

Given provided repository (Can copy into own directory or fork):

1. Set up a CI/CD pipeline in AzureDevops/GitHub/GitLab.
2. A restriction should be created that will allow changes on the master/main branch only via Merge Requests and only after the following criteria are met: Approval from a team member, all threads resolved. 
3. Optional : Include a code coverage step in the pipeline using some sort of lint, example sonar qube.
4. Set up a step in the deployment process that will replace values in the appsettings.json for the AppId and Secret.
5. Set up an AzureKeyVault instance that will hold the secrets that the app will be running, pay mind there is an api method that retrieves the "TestValue" secret from the keyvault, the app prefix is "DevOpsHomeWork".
6. Access to the API endpoints should be allowed only through an APIM.
7. Ensure that the application is available in case of a data center failure.
8. Set up an ApplicationInsights instance that the app could use. Connection string of the AI instance is expected to be in the appsettings.json.

Needless to say that the api has the integrations for the AKV and AI already added with just the configurations needed to be added to appsettings.json file.
Health endpoint is available at the /healthz route.

Good to have:
Deployment process done all that via an IAAC approach. (Arm templates / Terraform etc.)
Docker images should not be publicly available.

Minimum required points for completion:
(1),(2),(4)
