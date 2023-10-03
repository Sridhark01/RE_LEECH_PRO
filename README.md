# RE_LEECH_PRO

-  Clone this repo: ``` git clone https://github.com/Sridhark01/RE_LEECH_PRO RE_LEECH_PRO/ && cd RE_LEECH_PRO ```
 
- Switch to deploy branch: ```git checkout dep```

- Login to heroku: ```heroku login```

- Create heroku app: ```heroku create --region us YOUR-APP-NAME```

- Add remote: ```heroku git:remote -a YOUR-APP-NAME```

- Create container: ```heroku stack:set container```

- Push to heroku: ```git push heroku dep:master -f```


### Extras

- To delete the app: ```heroku apps:destroy YOUR-APP-NAME```

- To restart dyno: ```heroku restart```

- To turn off dyno: ```heroku ps:scale web=0```

- To turn on dyno: ```heroku ps:scale web=1```

- To set heroku variable: ```heroku config:set VARNAME=CONFIG_FILE_URL```

- To get live logs: ```heroku logs -t```


1. Opitionally you can upload your config as a secret on https://gist.github.com/
