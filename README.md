**Disclaimer: If Niantic Labs asks that to stop all PokeAert activities, PokeAlert will comply and the request will be fulfilled immediately**

Download links (latest version at the top) 
###[Download Section](https://github.com/PokeAlert/PokeAlert/releases)
##Join us on Discord: <a href="https://discord.gg/JdFdPw3"> <img src="http://i.imgur.com/sXlKZUB.png"> </a>

# PokeAlert - Pokemon Notification for PokemonGO 
PokeAlert has been developed by a handsome (:)) and enthusiast Pokemon trainer. Basically it is an nice alternative to PokeVision, an app to help you scan for Pokemon around you AND that triggers notifications when you are not using the app.

####Before starting let's get the things straight. With PokeAlert you will be allowed to freely scan wherever you want. This means that if you scan YOUR location and then scan New-York or whatever REALLY FARE from YOUR location, it is an obvious sign of cheating and you will probably have your account banned.

####With great scanner comes great responsibilities, be smart and just scan walkable or (drivable area). PokeAlert itself is very stealthy and respect a 10 seconds timeout between requests so if you scan responsively you should be safe!

####DO NOT USE YOUR OFFICIAL ACCOUNT. Please create a separate Pokemon Trainer or Gmail account JUST for this app

# Features
- Ditto mode, special mode that allows PokeAlert to find Ditto **(Warning!!! This mode is interfering with your account! Pokemons and items are being transfered in order to makes space for new ones!!)**
- Real Player tries to simulate 'natural behavior of player' (Pokestop spinnning, Pokemon catching, Item transfers) **(Warning!!! Real Player is interfering with your account! Pokemons and items are being transfered in order to make space for new ones!!)**
- IP ban and Speed Cap detection- Scanning circles are turning red if one of these happens.
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

You can also follow this guide made by Twitter user @CrimOfSweden
https://docs.google.com/document/d/1bZ8OHdF1YOE9O3hWKmoYmBM0R1Pqb3su-0Hnru_zjeI/pub


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

# Fixed location

Normaly, when the background service is enabled, PokeAlert will periodically scan your location in the background. But you can as well instruct PokeAlert to only scan a "fixed" location" here is how:

1) Long press on the Map

This will show a blue circle and whenever you enable the background service PokeAlert will scann that area

To remove the locked area simply click "once" on the blue circle


# Multi-Scan

**This is a feature for advance user**

PokeAlert let yout select "multiple" locked areas and assign any number of accounts to them. 

## Create a fixed area

1) Activate the feature in the Settings ("use multi scan")

2) Long press on the map. A dialog appear that will ask you select which account will be scanning this area

3) Press Ok, and you will see a blue circle on the map

4) Long press on the map to create a new area. A dialog appear that will ask you to select which account will be scanning this area

## Edit a fixed area

1) Click ONCE on a blue circle

2) Check or uncheck the accounts of your choice and press OK

Note: You cannot edit an area while a scan is running

## Delete an area

1) Click ONCE on a blue circle

2) Uncheck all the account and press OK


**Again, this feature is for advanced. When scannng on single area, PokeAlert is smart enough to make your accounts travel as a walking person and avoid making accounts jumps to fare**

**Now with Multi-Scan you are free to decide which accounts can scan which area, but if you create areas that are really fare from each other and start mixing which account scan which area then you MIGHT see these account ban faster as they jump location too fare**

**If you are a normal Joe you probably should not be using multi-scan and only scan one area as usual...**


# Recommendations

This section will explain why an account can become banned and some tips to avoid this.

## Niantic possible anti-scan technics

First to understand better why it is preferable to avoid doing certain things, here a list of reason an account "might" get flagged/banned:

###### Things that are is users hands:

 - Distance between scans: This might be the one that makes the more sense. If a scan (point) is considered "too fare" from a previous one they (Niantic) might judge that it was impossible for a normal user to fly/drive/walk there in a normal time. 

 - Delay between each requests: The original PokemonGO game only makes **1 request every 10 seconds**. If this delay is not respected nothing is returned by the server. And if this rules is periodically not respected this "might" indicate a non-normal behaviour and risk an account to be flagged/banned
 

###### Things that are not in users hands:

 - The requests PokeAlert sends to the PokemonGO server are not the same as the original PokemonGO game: There is a lot to consider when talking to the server. PokeAlert tries to mimic **as much as possible** the real game. But sometimes it is possible that things are slightly different and it "can" be used to get an account flagged.

 - The ratio **distance/pokemon caught**: Niantic "Might" use this criteria to detect a normal user vs scanning account and PokeAlert doesn't (yet?) catches pokemon now and then to adjust that ratio. This might explain why after 2 or 3 weeks an account might become banned.



## Tips to make your accounts last longer (PokeAlert viagra):

 1) Do not login with with your "scanning" accounts in the **PokemonGO game** with the same phone you using your main playing account. And of course do not login with your main playing account in PokeAlert!

 2) Scan around you as much as possible (avoid jumping over 2km away from scan to scan)
 
 3) Don't scan cities where your are not just for fun 

 4) Don't use your PokeAlert accounts on any other third-party app.
 
 
 5) avoid starting and stopping the background service (and manual scan) every 2 seconds (remember that 10 seconds rules?, when you start and stop to frequently the 10 seconds rules is not respected and might raise an eye brow server side) 

 6) For user that use the 70m radius it is very easy to break rule 5). So try manually wait 10 seconds between scans.


###### Settings recommendations:

 - Add at least 4-5 accounts for a better experience.

 - For user between 2 and 5 accounts I would suggest using not more than 300m radius and a background scan delay of minimum 20 seconds

 - For users that have between 10 and 15 accounts I'd suggest using not more than 550m radius and a background scan delay of minimum 20 seconds.


Note this is not an exact science. We do not know all the technics Niantic might use to detect non-normal behaviours. 
PokeAlert tries to be as stealthy as possible but it might happens of course that some of you account becomes banned after a while even by following the below rules.






# Twitter
https://twitter.com/PokemonGORadar1

# Credits
All the people on https://www.reddit.com/r/pokemongodev/
All the people at https://github.com/Grover-c13/PokeGOAPI-Java/issues
