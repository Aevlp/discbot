### How to deploy:
Click the button below to deploy to heroku using your own heroku account.  
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)



### Tips:
1. Be careful filling in the "herokuApp" field when deploy the app, otherwise your app can't work properly.
2. The format of "SA_JSON" field should look like the first line below(delete any spaces between each line,but don't add any **line break** between each line,then paste it into one line):  
  {"type": "service_account","project_id": "xxxxx","private_key_id":"xxxxx",......}&nbsp;&nbsp;**√**  
  {"type": "service_account",\n"project_id": "xxxxx",\n"private_key_id":"xxxxx",......}&nbsp;&nbsp;**x**
3. You can ssh into the server from command line:  `heroku ps:exec -a  yourAppName`. [See more details](https://devcenter.heroku.com/articles/heroku-cli)
4. You can update the larvm version in the folder called fanza(fork the repo first, and replace the larvm with a newer version,change the repository field in [app.json](app.json), then deploy your own repo to heroku).
5. The app will be restarted automatically once every 24 hours continuous running due to heroku's policy. [See more details](https://devcenter.heroku.com/articles/dynos#restarting)
6. the format of num ID:"ABC-123" or "ABC-123,abc-124,ABC-125 and more"(comma separated,case insensitive)
7. the format of cid ID:"abc00123" or "abc00123,abc00124,abc00125 and more"(comma separated,case insensitive)  
8. the format of mgs ID:"259LUXU-1200" or "259LUXU-1200,259LUXU-1201,259LUXU-1202 and more"(comma separated,case insensitive)  
9. If you submit many IDs one time, you can put a tag on these IDs, so they can be downloaded under the same folder.(the tag length should be no more than 10 characters, be free to use chinese or japanese name or any other language)
10. In theory, larvm-app can upload no more than 1.5TB data to your google team drive per day.
