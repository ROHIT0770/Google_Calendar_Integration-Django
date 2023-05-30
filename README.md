# Google_Calendar_Integration-Django

Problem: In this assignment you have to implement google calendar integration using django rest api. You need to use the OAuth2 mechanism to get users calendar access. Below are detail of API endpoint and corresponding views which you need to implement 
You need to use the OAuth2 mechanism to get users calendar access. Below are detail of API endpoint and corresponding views which you need to implement

For run this project on a local Computer: 

```sh
pip install - r requriments.txt
```
Prerequisites run this project on a local machine:
for this you need to Register your application on the Google Developers Console and you need to create Google Account Credentials file(Credentials.json) to implement Google Calendar integration using Django REST API, you will need to use the Google Calendar API and OAuth2 mechanism to authenticate and authorize user access to their calendar.
- Endpoint:
```
/rest/v1/calendar/init/ -> GoogleCalendarInitView()
```
This view should start step 1 of the OAuth. Which will prompt user for his/her credentials

```
/rest/v1/calendar/redirect/ -> GoogleCalendarRedirectView()
```
The purpose of this view is two fold:
1. Managing redirect requests sent by Google containing a code for obtaining a token. It requires implementing a mechanism to retrieve an access token from the provided code.
2. Upon successfully obtaining the access token, retrieving a list of events from the user's calendar.
### Note: In order to successfully execute this assignment, it is essential to have your Google account credentials readily available. These credentials should be securely stored within the project directory. Additionally, please ensure that you have configured a redirect URL in your Google Cloud account to ensure smooth functioning of the assignment.



