# League Reporter
Android app for University

 [![MIT](https://camo.githubusercontent.com/52ec9e2dfec7264e254fb7af5ac87f301ced9180/68747470733a2f2f696d672e736869656c64732e696f2f707970692f6c2f417270656767696f2e737667)](https://raw.githubusercontent.com/hyperium/hyper/master/LICENSE)
 
An android app for browsing information from major European football leagues.
EUROPEAN LEAGUES FOOTBALL INFORMATION, BOOKIE ASSISTANT 

THEME : BLUE
 
 football-data.org is a RESTful API in beta with regularly updated data. 
 If you register for a free API key you will get CORS support. I recommend registering for a key to show your support and help the service track usage. However, a key is not required yet so you can try out the endpoints right now. I am excited to see this API grow and mature!
 
 Available endpoints

- /soccerseasons/
- /soccerseasons/{id}/ranking
- /soccerseasons/{id}/fixtures
- /fixtures
- /soccerseasons/{id}/teams
- /teams/{id}
- /teams/{id}/fixtures/

 
 
 Some example calls:

 - http://api.football-data.org/v1/soccerseasons
 - http://api.football-data.org/v1/soccerseasons/351/teams
 - http://api.football-data.org/v1/fixtures
 - http://api.football-data.org/v1/teams/5
 - http://api.football-data.org/v1/soccerseasons/424 (European Championships France 2016)
 
 
 Example JSON output for a team:
 ```JSON
 {
    "_links":{
       "self":{
          "href":"http://api.football-data.org/v1/teams/5"
       },
       "fixtures":{
          "href":"http://api.football-data.org/v1/teams/5/fixtures"
       },
       "players":{
          "href":"http://api.football-data.org/v1/teams/5/players"
       }
    },
    "name":"FC Bayern München",
    "code":"FCB",
    "shortName":"Bayern",
    "squadMarketValue":"559,100,000 €",
    "crestUrl":"http://upload.wikimedia.org/wikipedia/commons/c/c5/Logo_FC_Bayern_München.svg"
 }
  ```
 Crest url gets logo online.

 Links: 
 
 http://www.jokecamp.com/blog/guide-to-football-and-soccer-data-and-apis/#footballdata
 
 
 Used libraries:
 - Android Logger
 - [Universal Image Loader] (https://github.com/nostra13/Android-Universal-Image-Loader)
 - and Icons Online.
 
