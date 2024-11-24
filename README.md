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
**Description**: Provides a modal to record scores for any number of members in the guild on the provided date. The member name is case-sensitive and must include any special characters if applicable.

**Example**:
```bash
/admin record_scores
```

### `/admin update_score`
**Description**: Updates a specific member's score for a given date.

**Arguments**:
- `member_name` (str): Name of the member to update.
- `date` (str): Date of the score to update.

**Example**:
```bash
/admin update_score member_name=chuåz date:2024-11-20
```

### `/admin delete_member`
**Description**: Delete a specific member from the guild. You can choose to fully remove the member or mark them as inactive (`in_guild=false`)

**Arguments**:
- `member_name` (str): Name of the member to delete.
- `keep_in_file` (bool): Whether to keep the member in the file but mark them as inactive. Default: `False`.

**Example**:
```bash
delete_member member_name:chuåz keep_in_file:true
```

### `/admin add_member`
**Description**: Adds a single member to the guild. The member name is case-sensitive and must include any special characters if applicable.

**Arguments**:
- `member_name` (str): Name of the member to add.
- `join_date` (optional, str): Date the member joined the guild (format: `YYYY-MM-DD`). Defaults to today's date if not provided.

**Example**:
```bash
/admin add_member member_name:chuåz join_date:2024-11-20


