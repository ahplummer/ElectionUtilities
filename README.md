# ElectionUtilities
## LAElectionResults.py
###Description
I was waiting for Election results from the local media on election night a while back, and was amazed at how slow the media was to get the returns from the Louisiana SoS website.  So, I wrote a utility to monitor the Secretary of State RSS feed(s) for certain state-wide races while I was sitting on the couch.
Requirement:  Install BeautifulSoup (pip install BeautifulSoup)
###Usage
```$python LAElectionResults.py -url=http://lasos.blob.core.windows.net/graphical-prod/rss/02212015_RSS.xml```

* -url (required): a valid base URL (for example, http://lasos.blob.core.windows.net/graphical-prod/rss/02212015_RSS.xml)
NOTE: this URL points to the RSS feed found on the SOS website.  Simply navigate to the SOS site on election night, and select the RSS feed.
* -election (optional): A valid election (Governor, for example).  To get this, execute without this option to get all results, then use this parameter to further filter on subsequent calls.
