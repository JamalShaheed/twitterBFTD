
Hi there, if you have ended up here from a link on Twitter then the website you are looking for does not exist (if you were looking for savesofia.org she got the transplant and is healthy)

If you were the previous owner of the domain send me an email at jamal.shaheed@gmail.com and I can transfer ownership (if the domain wasen't too expensive to purchase you can have it free of charge)

Fo anyone else read below

-----------------------------------------------------------------------------------------------------------------------------------

The script takes in a list of Twitter handles and dowloads all previous tweets, it then runs a WHOIS check on each domain linked by the tweet, storing the URL to a text file if an entry dosen't exist (meaning the domain has expired/ is avalible for regristration)


This Python script was originally created by [misterch0c](https://github.com/misterch0c) he did all the hard work.

This fork has a few changes to the original repo

* More exclusions, read from a csv file
* The ability to follow referal links (bit.ly, smart.url) recursively
* Files to be read from/written are now called with commandline arguments instead of hardcoded
* Some exceptions caught to stop the script terminating before searching all provided twitter handles
* Domains that are owned are added to the exclusion list to avoid repeated testing

Some features/changes to be made:
- [ ] add verbose output and quiet output flags 
- [x] PEP8 compliant formating
- [ ] Deal with URL's that have a '?' instead of a / 
- [ ] Get around Twitter API limits when downloading Tweets
- [ ] Try filter out Tweets with no URL before downloading (might not be possible/ worth it)
- [ ] Add the ability to check Twitter handle through commandline argument instead of file

---------------------------------------------------------------------------------------------------------------------------------

`pip install pythonwhois tweepy requests`

Usage: `python3 twrtBFTD.py -i FILE_WITH_TWITTER_HANDLES -o FILE_WRITE_RESULTS_TO`
A sample file "accounts" has been provided with the top 1000 Twitter users

Example Usage to use "accounts" file and write to PWND.txt:
`python3 twrtBFTD.py -i accounts -o PWND.txt`

Got to https://apps.twitter.com/ to create your consumer key/secret and access token/secret and add them to secrets.py
