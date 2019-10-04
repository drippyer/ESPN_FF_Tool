# ESPN_FF_Tool
 Small scripts to improve your QoL when using ESPN's fantasy football platform. Must be running Python 3 or higher.
 
The first script in the tool provides a constantly updating scoreboard as seen in the image below.
![image of first script](https://i.imgur.com/5vDJKdB.png)

The second script shows players that are starting on your team in 1+ league but against you in 1+ leagues as well.
![image of second script](https://i.imgur.com/zV0Enpo.png)

### Dependencies
- [ff-espn-api](https://github.com/cwendt94/ff-espn-api) from cwendt94
- [prettyTable](https://github.com/jazzband/prettytable)
- [pyyaml](https://github.com/yaml/pyyaml)

### Run Instructions
1. Copy config.yml.sample into config.yml 
2. In config.yml, enter the current week.
3. For each league you are in:

    a. Replace the value in league_names with your league name. If you are in multiple leagues, add them all to the array. Ex: ['League One', 'League Two']
    
    b. Replace the header 'Sample League:' with your league's name, and fill in your league ID. Copy the entire block and repeat for multiple leagues).
    
        i. Public Leagues: Leave the final two values as None for each league
        ii. Private Leagues: Visit your league's page and copy over the necessary fields from your cookies.  
4. Install the two necessary modules:

    a. `sudo python3 -m pip install pyyaml`
    
    b. `pip install prettyTable`
5. Run `python3 espnTool.py`
