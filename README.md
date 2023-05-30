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
This view will do two things
1. Handle redirect request sent by google with code for token. You
need to implement mechanism to get access_token from given
code
2. Once got the access_token get list of events in users calendar

### Note: To run this assignment need google account credentials which need to save in the project directory and add a redirect URL in your google cloud.



