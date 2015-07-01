#Welcome to LSQ!

LSQ is the first tool to allow you to quickly build robust applications using a microservice architecture. This tutorial will walk you through creating a microservice application that:
- collects email address
- adds them to a MailChimp list 
- sends an email using SendGrid
- reports the activity to KeenIO

Before beginning the tutorial you will need to set up an account with the following services:

- ####Sign up for Sendgrid: [https://sendgrid.com/user/signup](https://sendgrid.com/user/signup) 
  - To complete the tutorial, you will need: 
    - Sendgrid Email 
    - Sendgrid Password 
    
- ####Sign up for KeenIO: [https://keen.io/signup](https://keen.io/signup)
  - Create a new project  
  - To complete the tutorial, you will need: 
    - project ID 
    - project writeKey 
    - project readKey 

- ####Sign up for Mailchimp: [https://login.mailchimp.com/signup](https://login.mailchimp.com/signup) 
  - Create a new List
  - Get the unique ID for the list: 
    - Navigate to ‘Lists’ 
    - click on the down arrow for the list and select ‘Settings’ 
    - Scroll to the bottom of the page
  - Get the API key: 
    - Navigate to the your ‘Account’ page 
    - In the ‘Extras’ section, select ‘API Keys’
  - To complete the tutorial, you will need:
    - projectID 
    - writeKey 
    - readKey 

##Tutorial:

1. ####Download & Install 
    1. Visit lsq.io 
    2. Drag to install 

2. ####Create pre-built app 
  - Use the ‘Create a new application’ form to create a new app. 
    1. Give your application a name. Any spaces or invalid characters will be automatically removed. 
    2. Select an application template from the list. 
    3. Click ‘Create Application’ 

  *** This may take a minute. It is installing the application's NPM packages and initializing the LSQ monitoring *** 
3. ####Run and monitor 
  1. Once your services are initialized, the start button will turn from gray to blue. Click the start button to start all of your services! 
  2. Click on the name of the application to view the services for your application. 

4. ####Create a new service 
  1. Select 'node-micro' from the list of LSQ services 
  2. Add functionality 
    -Things to know 
      1. config = LSQ.config.get() 
      2. hostname/port = LSQ.services.get(&lt;service name&gt;) 
      3. request.post(http://&lt;hostname/post&gt;/path)

5. ####Deploy (coming soon)
  - Our 3.0 release will include free deployment for up to three applications! Stay tuned for more information.
