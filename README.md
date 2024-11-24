# Features

### Admin-Only Commands
Only those with administrator priviledges can use these commands. You can also set your own permissions by going into Server Settings -> Integrations -> Culvert Bot and overwrite the bot's permission's there for specific users or roles.

* `/record_scores` -> Record any guild member's score at a provided date.
    * __Usage:__ Use when logging culvert scores every week. 
* `/add_member [member_name]` -> Adds a member to the guild. This command is case-sensitive and **must** include special characters.
    * __Usage:__ Use when a member joins the guild.
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
