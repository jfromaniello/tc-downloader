var downloader = require("tc-downloader");

downloader.init();

downloader.start();

downloader.stop();



Configuration file (./config/config.json):

{
  "retryIntervalSeconds" : 60,
	"downloadFolder" : "./downloads/",
	"teamcity" : {
		"hostName" : "mgentile.idb.iadb.org",
		"hostPort" : "8080",
		"feedPath" : "/guestAuth/feed.html",
		"feedParams" : "itemsType=builds&buildStatus=successful&userKey=guest",
		"artifactZipPath" : "repository/downloadAll/",
	    "username" : "myuser",
	    "password" : "mypass"
	}
}
