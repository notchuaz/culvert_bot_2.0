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

### `/add_member`
**Description**: Adds a single member to the guild. The member name is case-sensitive and must include any special characters if applicable.

**Arguments**:
- `member_name` (str): Name of the member to add.
- `join_date` (optional, str): Date the member joined the guild (format: `YYYY-MM-DD`). Defaults to today's date if not provided.

**Example**:
```bash
/add_member member_name:chuåz join_date:2024-11-20


