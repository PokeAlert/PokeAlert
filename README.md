Download links (latest version at the top) 
###[Download Section](https://github.com/PokeAlert/PokeAlert/releases)

# PokeAlert - Pokemon Notification for PokemonGO 
PokeAlert has been developed by a handsome (:)) and enthusiast Pokemon trainer. Basically it is an nice alternative to PokeVision, an app to help you scan for Pokemon around you AND that triggers notifications when you are not using the app.

####Before starting let's get the things straight. With PokeAlert you will be allowed to freely scan wherever you want. This means that if you scan YOUR location and then scan New-York or whatever REALLY FARE from YOUR location, it is an obvious sign of cheating and you will probably have your account banned.

####With great scanner comes great responsibilities, be smart and just scan walkable or (drivable area). PokeAlert itself is very stealthy and respect a 10 seconds timeout between requests so if you scan responsively you should be safe!

####DO NOT USE YOUR OFFICIAL ACCOUNT. Please create a separate Pokemon Trainer or Gmail account JUST for this app

# Features
- Stealth mode, scans are controlled and do not spam PokemonGO servers to avoid bans
- Login with Google or Pokemon Trainer Account
- Multi-Account (Add one or more accounts for faster scan)
- Shows pokemon on a Map
- Scan in the background
- Sends notification when a Pokemon is found
- Filters to chose which pokemon trigger a notification
- Filters to chose which pokemon will be shown on the map


<p align="center">
  <img src="http://i.imgur.com/MgmooCR.png" width="300"/>
</p>


# Quick Tutorial Step-By-Step
1) Download and install the latest APK

2) Start the app

3) Login with either a gmail account or a Pokemon Trainer account (remember, don't use your official account, instead create some separate accounts just for scanning)

4) Basically, you are good to go, simply press the "Play" button and you will see the scan starting (pink circle moving around)


# Background scan service
If you do not want to manually scan areas, you can use the background scan service. When activated, PokeAlert will periodically scan in the background and send notification when a Pokemon is found! You do not need to stare at the map, simply put your phone in your pocket and wait for that Snorlax! :p

1) Tap on the options (Top-Right corner)

2) Tap on Settings

3) Configure the scan radius (for background service I like to put it between 120m and 310m)

4) Configure the scan interval (it is the interval in which the app will receive a new location and starts scan) you can set to 20seconds it is a good number. If you prefer save some battery set to 5 or 10 minutes

Note: There is only ONE scan at the same time. it means that if a new location is received and that a scan is still running, the scan will be ignored and wait until the next location.


# Multi-Accounts
PokemonGO server only accept 1 request every 10 second per account. 
This means that if a scan is composed of 25 scan points, it will take 250seconds to complete, which is over 4 minutes. This is VERY slow. But with PokeAlert you can add more than one account. This will increase the request rate and finish the scans much faster.

Example:
A scan of 400m is composed of 25 scan points (meaning there is gonna be 25 requests with 25 different location)

each scan point is associated to 1 account

Scenario with 1 account:
point1/account1, point2/account1, point3/account1, point3/account1 ... point25/account1

Remember 1 account can only make 1 request every 10 second.. so to finish the scan it will take 250seconds = over 4minutes

Scenario with 5 account:
point1/account1, point2/account2, point3/account3, point4/accoun4, point5/account5, point6/account1, point7/account2 ... point25/account5

point1,2,3,4,5 will be made at the same time<br/>
point6,7,8,9,10 will respectively wait until 10sec is passed for each account<br/>
point6,7,8,9,10 will be made at the same time<br/>
point11,12,13,14,15 will respectively wait until 10sec is passed for each account<br/>
point11,12,13,14,15 will be made at the same time<br/>
point16,17,18,19,20 will respectively wait until 10sec is passed for each account<br/>
point16,17,18,19,20 will be made at the same time<br/>

**This total to (theoretically) 30 seconds for a 400m scan instead of 4 minutes when using 1 account**


1) Tap on the options (Top-Right corner)

2) Tap on "Add Extra Accounts"

3) Simply add one or more gmail or Pokemon trainer account
   (We advice to **at least** have 5 accounts)


# Load accounts from file
For people with lots of accounts it can be tedious adding them one by one. This is why you can put all your account in a text file and use the "LOAD FROM FILE" option in the "Add Extra Accounts" screen

1) create a file named "pokealert_accounts.txt" at the ROOT of your SDcard
2) Add your account in the file like this

ptc_username_1 password PTC<br />
ptc_username_2 password PTC<br />
ptc_username_3 password PTC<br />
ptc_username_4 password PTC<br />
google_username_4 password GOOGLE<br />
google_username_4 password GOOGLE<br />
google_username_4 password GOOGLE<br />

3) got in the "Add Extra Accounts" and simply tap "LOAD FROM FILE". You will see all the account getting added!



# Twitter
https://twitter.com/PokemonGORadar1

# Credits
All the people on https://www.reddit.com/r/pokemongodev/
All the people at https://github.com/Grover-c13/PokeGOAPI-Java/issues
