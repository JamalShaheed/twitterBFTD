
Hi there, if you have ended up here from a link on Twitter then the website you are looking for does not exist (if you were looking for savesofia.org she got the transplant and is healthy)

If you were the previous owner of the domain send me an email at jamal.shaheed@gmail.com and I can transfer ownership (if the domain wasen't too expensive to purchase you can have it free of charge)

Fo anyone else read below

-----------------------------------------------------------------------------------------------------------------------------------

This Python script was originally created by [misterch0c](https://github.com/misterch0c/twitterBFTD) he did all the hard work, I simply added more exclusions (with plans to add the ability to follow referal links and ignore previously checked domains)

The script takes in a list of Twitter handles and dowloads all previous tweets, it then runs a WHOIS check on each domain linked by the tweet, storing the URL to a text file if an entry dosen't exist (meaning the domain has expired/ is avalible for regristration)
---------------------------------------------------------------------------------------------------------------------------------

Twitter back from the death looks in a user tweets history for domain names that are available for registration.

See blogpost: [How I hijacked top celebrities tweets including Katy Perry, Shakira…](https://medium.com/@MisterCh0c/how-i-hijacked-top-celebrities-tweets-including-katy-perry-shakira-fca3a0e751c6#.eddyocox9)


`pip install pythonwhois tweepy`

Usage:
Just run it at the root of the folder and it will create BFTD_results.txts
