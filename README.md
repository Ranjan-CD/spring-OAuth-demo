# spring-OAuth-demo
This project is for OAuth implementation

✅ Step 1: Go to Google Cloud Console
🔗 Visit: https://console.cloud.google.com/

✅ Step 2: Create or Select a Project
Click on the project dropdown (top left) and choose:

“New Project” → give it a name like JobAppOAuth

Or select an existing one.

✅ Step 3: Enable OAuth2 APIs
Go to the left sidebar → APIs & Services → Library

Search for and enable:

Google People API

(Optional: Gmail API, if you need to send mail)

✅ Step 4: Configure OAuth Consent Screen
Go to APIs & Services → OAuth consent screen

Choose “External” (for public apps) or “Internal” (only for your org GSuite users)

Fill in:

App Name

Support Email

Developer contact info

Click Save and Continue

(You can skip scopes for now)

Add test users if needed (your Gmail ID)

✅ Step 5: Create OAuth 2.0 Credentials
Go to APIs & Services → Credentials

Click “Create Credentials” → OAuth client ID

Choose application type:

Web application

Add:

Authorized redirect URIs (like: http://localhost:8080/login/oauth2/code/google)

Name: JobApp Web

Click Create

✅ Step 6: Copy Client ID & Secret
You will get:

Client ID

Client Secret

Save them securely (e.g. in application.properties or application.yml).




