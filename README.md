##Usage

```js
var downloader = require("tc-downloader");

downloader.init();
downloader.start();

//and then stop it
downloader.stop();
```

##With windser:

```bash
npm run-script install-windows-service
```

##Configuration

Configuration file (./config/config.json):

```js
{
  "retryIntervalSeconds" : 60,
	"downloadFolder" : "./downloads/",
	"teamcity" : {
		"hostName" : "teamcity.server.com",
		"hostPort" : "8080",
		"feedPath" : "/guestAuth/feed.html",
		"feedParams" : "itemsType=builds&buildStatus=successful&userKey=guest",
		"artifactZipPath" : "repository/downloadAll/",
	    "username" : "myuser",
	    "password" : "mypass"
	}
}
```

