Admin commands:
------
### admin_utils 
**add_join_event**: <'type' 'option'> - Add action to be triggered on user join.

Possible actions:

 * message #channel blahblah -> send blahblah to #channel

 * role @role -> set @role on join).

The scripted message can contain special words that are replaced when the event is triggered:

 * {AGE} - Account age

 * {USER} - User that just joined

 * {USER_ID} - User ID

 * {SEEN_CNT} - How many times this user has been seen in servers shared with the bot



e.g. 'message #general {USER} / {USER_ID} just joined!' will send 'John / 12345678910 just joined!'

**del_join_event**: <event id> - delete a join event

**get_timeout_for**: Get timeout for a join event

**list_join_events**: List on-join events

**set_timeout_for**: <join event id, timeout> - Set timeout for a join event. Use '5s' for timeout to set it to 5s or 1m to set it to one minute.

------
### avatar 
**set_banner_text**: Sets the server banner text to a given content

**set_server_banner**: Sets the server banner to a given URL

------
### birthday 
**bday_dbg**: No description provided.

**birthday**: Manage birthday announcements.



    See `.birthday help` for more info

**trigger_check**: No description provided.

------
### cmd_owner_hook 
**admin_config**: Command usage: `.admin_config <subcommand>`

Available subcommands:

- `admin_roles <subcommand>`: Available subcommands:

> - `add`: <role> - Add a new admin role.

> - `list`: List currently set admin roles.

> - `remove`: <role> - Remove admin role from list.

- `chgroup <subcommand>`: Available subcommands:

> - `create`: <chgroup> - Creates a new channel group with the specified name.

> - `list`: List all channel groups.

> - `remove`: <chgroup> - Delete channel group.

- `chgroup_chans <subcommand>`: Available subcommands:

> - `add`: <chgroup> <channel> - Add specified channel to given channel group.

> - `list`: <chgroup> - List associated channels of specified channel group.

> - `remove`: <chgroup> <channel> - Remove specified channel from given channel group.

- `cmd_chgroups <subcommand>`: Available subcommands:

> - `add`: <command> <chgroup> - Add the given channel group to command with that name.

> - `list`: <command> - List channel groups associated with command.

> - `remove`: <command> <chgroup> - Remove channel group from command.

- `fchgroup <subcommand>`: Available subcommands:

> - `add`: <command> <fchgroup> - Forbid channel group to access command with that name.

> - `list`: <command> - List forbidden channel groups for command.

> - `remove`: <command> <fchgroup> - Remove the channel group's restriction for the command.

- `cmd_owner <subcommand>`: Available subcommands:

> - `add`: <command> <role> - Allow role to execute command, without any restrictions.

> - `list`: <command> - List roles that can execute command without any restrictions.

> - `remove`: <command> <role> - Remove role's permissions to execute command without any restrictions.

- `bot_channel <subcommand>`: Available subcommands:

> - `set`: <channel> - Set the default bot command channel.

> - `get`: Get the default bot command channel, if it exists.

> - `clear`: Clear the default bot command channel.

- `unrestricted_cmd <subcommand>`: Available subcommands:

> - `make`: <command> - Unrestrict command, all channel group and default bot channel restrictions are lifted.

> - `check`: <command> - Check command restriction status.

> - `restore`: <command> - Restrict command, re-instate channel group and default bot channel restrictions.

- `updated_commands`: Display which subcommand matches the old administration command

**command_properties**: Get set command properties

------
### correction 
**toggle_correction_msg_del_ability**: enable/disable ability for automatic deletion of command when running .s/.ss

------
### del_messages 
**delete**: <number> - delete a given number of messages from the channel where the command is executed

------
### firewall 
**firewall**: Manage server firewall.



    Usage:

        - up [expire_time]

        - down

        - status

        - mode autokick|autoban



    Examples:

        .firewall up -> will raise the firewall indefinitely

        .firewall up 10s -> will raise the firewall for 10 seconds

        .firewall up 1h -> will raise the firewall for one hour



        .firewall mode autokick -> enables autokick for the firewall.

------
### grab 
**del_grab**: Delete a grab entry. Specify what the grab message contains or the message ID

------
### image_generator 
**force_refresh_porn**: No description provided.

**nuke_porn**: No description provided.

------
### log_events 
**add_filter_out_channel**: <channel> - Don't log events on a certain channel.

**bad_word**: Command usage: `.bad_word <subcommand>`

Available subcommands:

- `add`: <word> - remove a message it contains 'word'

- `list`: List bad words

- `remove`: <word> - Remove a bad word

**clear_event_log_chan**: <channel> - Clear logging channel and deactivate logging.

**clear_filter_out_channel**: <channel> - Remove channel event filtering.

**get_event_log_chan**: <channel> - Get the event log channel.

**list_filtered_out_channels**: <channel> - List filtered channels.

**set_event_log_chan**: <channel> - Activate event logging and log to channel.

Logged events: user join, user leave, message edit, message delete, member update, member ban, member unban.

------
### poll 
**close_poll**: <message link> - Closes poll give in message link

**create_poll**: <title %% option1 %% option2 %% ...> - create a poll with a title and multiple options

**list_polls**: Lists active polls

------
### role_selector 
**add_selector_role_interval**: <selector> <role start> <role end> - adds the roles in the specified interval to the selector

**add_selector_roles**: <selector> <roles> - adds the specified roles to the selector

**create_selector**: <selector name> - create a selector that assigns a role

**delete_selector**: <command_name> - delete a temporary selector command

**remove_selector_role_interval**: <selector> <role start> <role end> - removes the roles in the specified interval from the selector.

    NOTE: THIS REMOVES THE ROLE INTERVAL FROM THE ROLE LIST, NOT FROM THE SELECTOR LIST.

**remove_selector_roles**: <selector> <roles> - removes the specified roles from the selector

**set_selector_description**: <selector> <description> - sets a description for the selector documentation

**set_selector_max_selectable**: <selector> <maxSelectable (int)> - sets the number of max selectable options for the selector. If maxSelectable <= 0, then the number of max selectable options is unlimited

**set_selector_title**: <selector> <title> - sets a title for the selector

------
### say 
**say**: <channel message> - Send a message to a channel

**say_pm**: <user message> - Send a message to an user.

------
### selector 
**del_permanent_selector**: Remove a permanent selector.

**list_permanent_selectors**: No description provided.

**permanent_selector**: <message link/ID> - makes a generated selector permanent (e.g. the bot will always listen for reacts on the given message).

    This command is useful for pinning selectors on channels.

**rebuild_selectors**: No description provided.

------
### tag 
**tag_del**: <tag> - delete a tag

------
### temp_role 
**ban**: <user [,time], reason> - ban someone permanently or for a given amount of time (e.g. `.ban @plp 5m` bans plp for 5 minutes).

**clear_mod_log_chan**: Clear the moderator actions channel. No moderator actions messages will be sent.

**close_user_case**: <id> - mark user case as closed

**create_temp_role_cmd**: <command name, role> - create a command that assigns a temporary role by specifying `command_name role`

**delete_temp_role_cmd**: <command_name> - delete a temporary role command

**export_cases**: No description provided.

**get_mod_log_chan**: Return the moderator actions channel

**kick**: <user [reason]> - Kick someone with an optional reason

**list_temp_role_cmds**: list temporary role commands

**set_mod_log_chan**: <channel> - Set channel for moderator actions. When a moderator action will be done through the bot, details about the action will be logged to this channel.

**set_temp_role_cmd_type**: No description provided.

**show_user_case**: <id> - show details for a given user case

**userhistory**: <user> - List confinement reasons for user

**warn**: <user reason> - Warn a user

------
### watcher 
**clear_rupdates_channel**: Remove reddit updates channel.

**get_rupdates_channel**: List reddit updates annoucement channel.

**set_rupdates_channel**: <channel> - Send reddit updates on channel.

**startwatch**: Start watching subreddits.

**stopwatch**: Stop watching subreddits.

**subwatch_add**: Add a subreddit to the watch list.

**subwatch_del**: Remove a subreddit from the watch list

