# Features

### Admin-Only Commands
Only those with administrator priviledges can use these commands. You can also set your own permissions by going into Server Settings -> Integrations -> Culvert Bot and overwrite the bot's permission's there for specific users or roles.

* `/set_date` -> Sets the date for which members of the guild will be entering their scores for. This will be set to None every week at Culvert reset.
   * __Usage:__ Every week, an admin must set the date for which members can enter their own scores, otherwise they will be unable to. 
* `/record_scores` -> Record scores for members on the current week.
    * __Usage:__ Use when logging culvert scores every week.
* `/record_lastweek_scores` -> Record scores for members of the previous week.
    * __Usage:__ Use this to record any score for members of the previous week. I imagine this will be used more versus `/record_scores` since scores are normally recorded after culvert reset.
* `/add_member [member_name]` -> Adds a member to the guild. This command is case-sensitive and **must** include special characters.
    * __Usage:__ Use when a member joins the guild.
* `/add_all` -> Allows the user to add members in bulk in the modal.
    * __Usage:__ Use this when initializing the bot with the guild so it is easier to add more than one member. User `/add_member` to only add a single member to the guild.
    * __Example:__ This will be in the form of `name,level,class,[join_date]` (e.g.chuåz,288,Adele,2024-11-23) [If a date is not provided, the date will be the date the command is executed.
* `/update_score [member_name][date][new_score]` -> Updates the score of a member at specific date.
    * __Usage:__ Use when a member's score needs to be updated or changed.
* `/update_join_date [member_name][join_date]` -> Update the join date of a specific member.
    * __Usage:__ Use this when a member's join date needs to be changed.
* `/update_member_class [member_name][new_class]` -> Update the class of a specific member.
    * __Usage:__ Use this when a member's class needs to be updated or changed.
* `/update_member_level [member_name][level]` -> Update the level of a specific mebmer.
    * __Usage:__ Use this when a member's level needs to be updated or changed.
* `/retrieve_members` -> Returns all active and recorded members in the guild.
    * __Usage:__ This is a QOL command that returns a list of all members in alphabetical order to be used to copy-paste for easier score recording when using `/record_scores`.
    * The list looks like this:
``` bash
Member1,
Member2,
Member3,
Member4,
...
```
* `/delete_member [member_name][keep_in_file]` -> Deletes a specific member from the guild. You can choose to fully remove the member or mark them as inactive.
    * __Usage:__ Set `keep_in_file` to `True` to simply mark the member as inactive but keep all records in the database. Set `keep_in_file` to `False` to completely remove all their records from the database. Any inactive member will not appear in any other command until `/reinstate` is used.
* `/reinstate [member_name]` -> Marks a specific member from inactive to active.
    * __Usage:__ Use this when a member returns to the guild and uses their previous records in the database.
* `/delete_score [member_name][date]` -> Deletes a score for a specific member at a given date.
    * __Usage:__ Use this when a score is needed to be removed from a member.
* `/add_achievement [member_name][achievement]` -> Choose from a list of achievements to give to a specific member.
* `/remove_achievement [member_name][achievement]` -> Removes an achievement from a specific member.

### Public Culvert Commands
* `/profile [member]` -> Displays the culvert profile of a member. Shows class, level, join date, this week's score, best score, closest competitor, weekly rank, change from last week, average change over the last 6 recorded scores, achievements, past scores, and participation.
* `/graph [member] optional:[second_member]` -> Displays a graph of scores for one or two members.
* `/leaderboard [date]` -> Displays the leaderboard for all scores recorded on a specific date.
* `/class [mode][class_name] optional:[graph] optional:[date]` -> Displays class information for culvert scores.
    * Top Mode: Shows the top members with the highest cumulative culvert score.
      * Graph: If `graph` is set to `True`, display a graph of all culvert scores of all members in the specified class.
      * Date: If `date` is specified, display a graph of all culvert scores of all members in the specified class for the date.
    * Compare Mode: Shows the top classes with the highest cumulative culvert score.
      * Date: If `date` is specified, display the top classes with highest total culvert scores on that date.
* `/add_score [member_name][score]` -> Adds a score for a specific member for the current week.

### Available Achievements

* Black Mage Solo
* Hard Seren Solo
* Easy Kalos Solo
* Normal Kalos Solo
* Extreme Lotus Solo
* Normal Kaling Solo
* Chaos Kalos Clear
* Extreme Black Mage Clear
* Extreme Seren Clear
* Hard Kaling Clear
* Extreme Kalos Clear
* Reach Level 260
* Reach Level 265
* Reach Level 270
* Reach Level 275
* Reach Level 280
* Reach Level 285
* Reach Level 290
* Reach Floor 40 in Dojo
* Reach Floor 50 in Dojo
* Reach Floor 60 in Dojo
* Reach Floor 70 in Dojo
* Reach Floor 80 in Dojo
* Reach Floor 90 in Dojo
* Reach 50k Culvert
* Reach 60k Culvert
* Reach 70k Culvert
* Reach 80k Culvert
* Reach 90k Culvert
* Reach 100k Culvert
