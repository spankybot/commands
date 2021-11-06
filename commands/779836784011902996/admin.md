Admin commands:
------
### admin_utils 
**add_join_event**: &amp;lt;&amp;#x27;type&amp;#x27; &amp;#x27;option&amp;#x27;&amp;gt; - Add action to be triggered on user join.

Possible actions:

 * message #channel blahblah -&amp;gt; send blahblah to #channel

 * role @role -&amp;gt; set @role on join).

The scripted message can contain special words that are replaced when the event is triggered:

 * {AGE} - Account age

 * {USER} - User that just joined

 * {USER_ID} - User ID

 * {SEEN_CNT} - How many times this user has been seen in servers shared with the bot



e.g. &amp;#x27;message #general {USER} / {USER_ID} just joined!&amp;#x27; will send &amp;#x27;John / 12345678910 just joined!&amp;#x27;

**del_join_event**: &amp;lt;event id&amp;gt; - delete a join event

**get_timeout_for**: Get timeout for a join event

**list_join_events**: List on-join events

**set_timeout_for**: &amp;lt;join event id, timeout&amp;gt; - Set timeout for a join event. Use &amp;#x27;5s&amp;#x27; for timeout to set it to 5s or 1m to set it to one minute.

------
### avatar 
**set_banner_text**: Sets the server banner text to a given content

**set_server_banner**: Sets the server banner to a given URL

------
### cmd_owner_hook 
**admin_config**: Command usage: `.admin_config &amp;lt;subcommand&amp;gt;`

Available subcommands:

- `admin_roles &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `add`: &amp;lt;role&amp;gt; - Add a new admin role.

&gt; - `list`: List currently set admin roles.

&gt; - `remove`: &amp;lt;role&amp;gt; - Remove admin role from list.

- `chgroup &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `create`: &amp;lt;chgroup&amp;gt; - Creates a new channel group with the specified name.

&gt; - `list`: List all channel groups.

&gt; - `remove`: &amp;lt;chgroup&amp;gt; - Delete channel group.

- `chgroup_chans &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `add`: &amp;lt;chgroup&amp;gt; &amp;lt;channel&amp;gt; - Add specified channel to given channel group.

&gt; - `list`: &amp;lt;chgroup&amp;gt; - List associated channels of specified channel group.

&gt; - `remove`: &amp;lt;chgroup&amp;gt; &amp;lt;channel&amp;gt; - Remove specified channel from given channel group.

- `cmd_chgroups &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `add`: &amp;lt;command&amp;gt; &amp;lt;chgroup&amp;gt; - Add the given channel group to command with that name.

&gt; - `list`: &amp;lt;command&amp;gt; - List channel groups associated with command.

&gt; - `remove`: &amp;lt;command&amp;gt; &amp;lt;chgroup&amp;gt; - Remove channel group from command.

- `fchgroup &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `add`: &amp;lt;command&amp;gt; &amp;lt;fchgroup&amp;gt; - Forbid channel group to access command with that name.

&gt; - `list`: &amp;lt;command&amp;gt; - List forbidden channel groups for command.

&gt; - `remove`: &amp;lt;command&amp;gt; &amp;lt;fchgroup&amp;gt; - Remove the channel group&amp;#x27;s restriction for the command.

- `cmd_owner &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `add`: &amp;lt;command&amp;gt; &amp;lt;role&amp;gt; - Allow role to execute command, without any restrictions.

&gt; - `list`: &amp;lt;command&amp;gt; - List roles that can execute command without any restrictions.

&gt; - `remove`: &amp;lt;command&amp;gt; &amp;lt;role&amp;gt; - Remove role&amp;#x27;s permissions to execute command without any restrictions.

- `bot_channel &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `set`: &amp;lt;channel&amp;gt; - Set the default bot command channel.

&gt; - `get`: Get the default bot command channel, if it exists.

&gt; - `clear`: Clear the default bot command channel.

- `unrestricted_cmd &amp;lt;subcommand&amp;gt;`: Available subcommands:

&gt; - `make`: &amp;lt;command&amp;gt; - Unrestrict command, all channel group and default bot channel restrictions are lifted.

&gt; - `check`: &amp;lt;command&amp;gt; - Check command restriction status.

&gt; - `restore`: &amp;lt;command&amp;gt; - Restrict command, re-instate channel group and default bot channel restrictions.

- `updated_commands`: Display which subcommand matches the old administration command

**command_properties**: Get set command properties

------
### correction 
**toggle_correction_msg_del_ability**: enable/disable ability for automatic deletion of command when running .s/.ss

------
### del_messages 
**delete**: &amp;lt;number&amp;gt; - delete a given number of messages from the channel where the command is executed

------
### firewall 
**firewall**: Manage server firewall.



    Usage:

        - up [expire_time]

        - down

        - status

        - mode autokick|autoban



    Examples:

        .firewall up -&amp;gt; will raise the firewall indefinitely

        .firewall up 10s -&amp;gt; will raise the firewall for 10 seconds

        .firewall up 1h -&amp;gt; will raise the firewall for one hour



        .firewall mode autokick -&amp;gt; enables autokick for the firewall.

------
### grab 
**del_grab**: Delete a grab entry. Specify what the grab message contains or the message ID

------
### log_events 
**add_filter_out_channel**: &amp;lt;channel&amp;gt; - Don&amp;#x27;t log events on a certain channel.

**bad_word**: Command usage: `.bad_word &amp;lt;subcommand&amp;gt;`

Available subcommands:

- `add`: &amp;lt;word&amp;gt; - remove a message it contains &amp;#x27;word&amp;#x27;

- `list`: List bad words

- `remove`: &amp;lt;word&amp;gt; - Remove a bad word

**clear_event_log_chan**: &amp;lt;channel&amp;gt; - Clear logging channel and deactivate logging.

**clear_filter_out_channel**: &amp;lt;channel&amp;gt; - Remove channel event filtering.

**get_event_log_chan**: &amp;lt;channel&amp;gt; - Get the event log channel.

**list_filtered_out_channels**: &amp;lt;channel&amp;gt; - List filtered channels.

**set_event_log_chan**: &amp;lt;channel&amp;gt; - Activate event logging and log to channel.

Logged events: user join, user leave, message edit, message delete, member update, member ban, member unban.

------
### poll 
**close_poll**: &amp;lt;message link&amp;gt; - Closes poll give in message link

**create_poll**: &amp;lt;title %% option1 %% option2 %% ...&amp;gt; - create a poll with a title and multiple options

**list_polls**: Lists active polls

------
### role_selector 
**add_selector_role_interval**: &amp;lt;selector&amp;gt; &amp;lt;role start&amp;gt; &amp;lt;role end&amp;gt; - adds the roles in the specified interval to the selector

**add_selector_roles**: &amp;lt;selector&amp;gt; &amp;lt;roles&amp;gt; - adds the specified roles to the selector

**create_selector**: &amp;lt;selector name&amp;gt; - create a selector that assigns a role

**delete_selector**: &amp;lt;command_name&amp;gt; - delete a temporary selector command

**remove_selector_role_interval**: &amp;lt;selector&amp;gt; &amp;lt;role start&amp;gt; &amp;lt;role end&amp;gt; - removes the roles in the specified interval from the selector.

    NOTE: THIS REMOVES THE ROLE INTERVAL FROM THE ROLE LIST, NOT FROM THE SELECTOR LIST.

**remove_selector_roles**: &amp;lt;selector&amp;gt; &amp;lt;roles&amp;gt; - removes the specified roles from the selector

**set_selector_description**: &amp;lt;selector&amp;gt; &amp;lt;description&amp;gt; - sets a description for the selector documentation

**set_selector_max_selectable**: &amp;lt;selector&amp;gt; &amp;lt;maxSelectable (int)&amp;gt; - sets the number of max selectable options for the selector. If maxSelectable &amp;lt;= 0, then the number of max selectable options is unlimited

**set_selector_title**: &amp;lt;selector&amp;gt; &amp;lt;title&amp;gt; - sets a title for the selector

------
### say 
**say**: &amp;lt;channel message&amp;gt; - Send a message to a channel

**say_pm**: &amp;lt;user message&amp;gt; - Send a message to an user.

------
### selector 
**del_permanent_selector**: Remove a permanent selector.

**list_permanent_selectors**: No description provided.

**permanent_selector**: &amp;lt;message link/ID&amp;gt; - makes a generated selector permanent (e.g. the bot will always listen for reacts on the given message).

    This command is useful for pinning selectors on channels.

**rebuild_selectors**: No description provided.

------
### tag 
**tag_del**: &amp;lt;tag&amp;gt; - delete a tag

------
### temp_role 
**ban**: &amp;lt;user [,time], reason&amp;gt; - ban someone permanently or for a given amount of time (e.g. `.ban @plp 5m` bans plp for 5 minutes).

**clear_mod_log_chan**: Clear the moderator actions channel. No moderator actions messages will be sent.

**close_user_case**: &amp;lt;id&amp;gt; - mark user case as closed

**create_temp_role_cmd**: &amp;lt;command name, role&amp;gt; - create a command that assigns a temporary role by specifying `command_name role`

**delete_temp_role_cmd**: &amp;lt;command_name&amp;gt; - delete a temporary role command

**democratie**: Temporary role assignment command as defined by server ops.

**export_cases**: No description provided.

**get_mod_log_chan**: Return the moderator actions channel

**kick**: &amp;lt;user [reason]&amp;gt; - Kick someone with an optional reason

**list_temp_role_cmds**: list temporary role commands

**set_mod_log_chan**: &amp;lt;channel&amp;gt; - Set channel for moderator actions. When a moderator action will be done through the bot, details about the action will be logged to this channel.

**set_temp_role_cmd_type**: No description provided.

**show_user_case**: &amp;lt;id&amp;gt; - show details for a given user case

**userhistory**: &amp;lt;user&amp;gt; - List confinement reasons for user

**warn**: &amp;lt;user reason&amp;gt; - Warn a user

------
### watcher 
**clear_rupdates_channel**: Remove reddit updates channel.

**get_rupdates_channel**: List reddit updates annoucement channel.

**set_rupdates_channel**: &amp;lt;channel&amp;gt; - Send reddit updates on channel.

**startwatch**: Start watching subreddits.

**stopwatch**: Stop watching subreddits.

**subwatch_add**: Add a subreddit to the watch list.

**subwatch_del**: Remove a subreddit from the watch list

