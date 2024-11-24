# culvert_bot_2.0
A Discord bot used to track culvert scores of guild members.

# Discord Bot Commands

This document provides an overview of all the commands available in the bot, including their descriptions, arguments, and examples.

---

## Command Categories
- [Admin Commands](#admin-commands)
- [Culvert Commands](#culvert-commands)

---

## Admin Commands

### `/admin record_scores`
**Description:** Provides a modal to record scores for any number of members in the guild on the provided date. The member name is case-sensitive and must include any special characters if applicable.

**Example:**
```bash
/admin record_scores
```

### `/admin add_member`
**Description:** Adds a single member to the guild. The member name is case-sensitive and must include any special characters if applicable.

**Arguments:**
- `member_name` (str): Name of the member to add.
- `join_date` (optional, str): Date the member joined the guild (format: `YYYY-MM-DD`). Defaults to today's date if not provided.

**Example:**
```bash
/admin add_member member_name:chuåz join_date:2024-11-20
```

### `/admin update_score`
**Description:** Updates a specific member's score for a given date.

**Arguments:**
- `member_name` (str): Name of the member to update.
- `date` (str): Date of the score to update.

**Example:**
```bash
/admin update_score member_name=chuåz date:2024-11-20
```

### `/admin update_join_date`
**Description:** Updates the join date of a specific member.

**Arguments:**
- `member_name` (str): Name of the member to update.
- `new_join_date` (str): Date the member joined.

**Example:**
```bash
/admin update_join_date member_name:chuåz new_join_date:2024-11-20
```

### `/admin update_member_class`
**Description:** Update the class of a specific member.

**Arguments:**
- `member_name` (str): Name of the member to update.
- `new_class` (str): Class of the member.

**Example:**
```bash
/admin update_member_class member_name:chuåz new_class:Adele
```

### `/admin update_member_level`
**Description:** Updates the level of a specific member.

**Arguments:**
- `member_name` (str): Name of the member to update.
- `level` (int): The new level to update to.

**Example:**
```bash
/admin update_member_level member_name:chuåz level:288
```

### `/admin add_achievement
**Description:** Assigns a specific achievement to a member in the guild.

- `member_name` (str): Name of the member to assign the achievement to.
- `achievement` (str): The achievement to assign. Available options:
  - **Black Mage Solo Clear**
  - **Hard Seren Solo Clear**
  - **Easy Kalos Solo Clear**
  - **Easy Kaling Solo Clear**
  - **Normal Kalos Solo Clear**
  - **Extreme Lotus Solo Clear**
  - **Normal Kaling Solo Clear**
  - **Chaos Kalos Clear**
  - **Extreme Black Mage Clear**
  - **Extreme Seren Clear**
  - **Hard Kaling Clear**
  - **Reach Floor 40 in Dojo**
  - **Reach Floor 50 in Dojo**
  - **Reach Floor 60 in Dojo**
  - **Reach Floor 70 in Dojo**
  - **Reach Floor 80 in Dojo**
  - **Reach Floor 90 in Dojo**

**Example**:
```bash
/add_achievement member_name:Liwa achievement:Black Mage Solo Clear
```

### `/admin delete_member`
**Description**: Delete a specific member from the guild. You can choose to fully remove the member or mark them as inactive (`in_guild=false`)

**Arguments**:
- `member_name` (str): Name of the member to delete.
- `keep_in_file` (bool): Whether to keep the member in the file but mark them as inactive. Default: `False`.

**Example**:
```bash
/admin delete_member member_name:chuåz keep_in_file:true
```

### `/admin reinstate`
**Description:** Reinstates a member marked as inactive (`in_guild=false`) to active status (`in_guild=true`).

**Arguments:**
- `member_name` (str): Name of the inactive member to reinstate

**Exaxmple:**
```bash
/admin reinstate member_name:chuåz
```


