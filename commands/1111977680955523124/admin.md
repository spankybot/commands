Admin commands:
------
### admin_utils 
**add_join_event**: &lt;&#x27;type&#x27; &#x27;option&#x27;&gt; - Add action to be triggered on user join.

    Possible actions:

     * message #channel blahblah -&gt; send blahblah to #channel

     * role @role -&gt; set @role on join).

    The scripted message can contain special words that are replaced when the event is triggered:

     * {AGE} - Account age

     * {USER} - User that just joined

     * {USER_ID} - User ID

     * {SEEN_CNT} - How many times this user has been seen in servers shared with the bot



    e.g. &#x27;message #general {USER} / {USER_ID} just joined!&#x27; will send &#x27;John / 12345678910 just joined!&#x27;

**del_join_event**: &lt;event id&gt; - delete a join event

**get_timeout_for**: Get timeout for a join event

**list_join_events**: List on-join events

**set_timeout_for**: &lt;join event id, timeout&gt; - Set timeout for a join event. Use &#x27;5s&#x27; for timeout to set it to 5s or 1m to set it to one minute.

------
### avatar 
**set_banner_text**: Sets the server banner text to a given content

**set_server_banner**: Sets the server banner to a given URL

------
### chatgpt 
**cbot_refresh_all**: No description provided.

------
### cmd_owner_hook 
**admin_config**: Command usage: `.admin_config <subcommand>`

Available subcommands:

- `admin_roles <subcommand>`: Available subcommands:
> - `add`: &lt;role&gt; - Add a new admin role.
> - `list`: List currently set admin roles.
> - `remove`: &lt;role&gt; - Remove admin role from list.

- `chgroup <subcommand>`: Available subcommands:
> - `create`: &lt;chgroup&gt; - Creates a new channel group with the specified name.
> - `list`: List all channel groups.
> - `remove`: &lt;chgroup&gt; - Delete channel group.

- `chgroup_chans <subcommand>`: Available subcommands:
> - `add`: &lt;chgroup&gt; &lt;channel&gt; - Add specified channel to given channel group.
> - `list`: &lt;chgroup&gt; - List associated channels of specified channel group.
> - `remove`: &lt;chgroup&gt; &lt;channel&gt; - Remove specified channel from given channel group.

- `cmd_chgroups <subcommand>`: Available subcommands:
> - `add`: &lt;command&gt; &lt;chgroup&gt; - Add the given channel group to command with that name.
> - `list`: &lt;command&gt; - List channel groups associated with command.
> - `remove`: &lt;command&gt; &lt;chgroup&gt; - Remove channel group from command.

- `fchgroup <subcommand>`: Available subcommands:
> - `add`: &lt;command&gt; &lt;fchgroup&gt; - Forbid channel group to access command with that name.
> - `list`: &lt;command&gt; - List forbidden channel groups for command.
> - `remove`: &lt;command&gt; &lt;fchgroup&gt; - Remove the channel group&#x27;s restriction for the command.

- `cmd_owner <subcommand>`: Available subcommands:
> - `add`: &lt;command&gt; &lt;role&gt; - Allow role to execute command, without any restrictions.
> - `list`: &lt;command&gt; - List roles that can execute command without any restrictions.
> - `remove`: &lt;command&gt; &lt;role&gt; - Remove role&#x27;s permissions to execute command without any restrictions.

- `bot_channel <subcommand>`: Available subcommands:
> - `set`: &lt;channel&gt; - Set the default bot command channel.
> - `get`: Get the default bot command channel, if it exists.
> - `clear`: Clear the default bot command channel.

- `unrestricted_cmd <subcommand>`: Available subcommands:
> - `make`: &lt;command&gt; - Unrestrict command, all channel group and default bot channel restrictions are lifted.
> - `check`: &lt;command&gt; - Check command restriction status.
> - `restore`: &lt;command&gt; - Restrict command, re-instate channel group and default bot channel restrictions.

- `updated_commands`: Display which subcommand matches the old administration command

**command_properties**: Get set command properties

------
### correction 
**toggle_correction_msg_del_ability**: enable/disable ability for automatic deletion of command when running .s/.ss

------
### del_messages 
**delete**: &lt;number&gt; - delete a given number of messages from the channel where the command is executed

------
### firewall 
**firewall**: Manage server firewall.



    Usage:

        - up [expire_time]

        - down

        - status

        - mode autokick|autoban



    Examples:

        .firewall up -&gt; will raise the firewall indefinitely

        .firewall up 10s -&gt; will raise the firewall for 10 seconds

        .firewall up 1h -&gt; will raise the firewall for one hour



        .firewall mode autokick -&gt; enables autokick for the firewall.

------
### grab 
**del_grab**: Delete a grab entry. Specify what the grab message contains or the message ID

**export_grabs**: No description provided.

------
### irc 
**irc_settings**: Command usage: `.irc_settings <subcommand>`

Available subcommands:

- `request_chan`: No description provided.

- `add_access_role`: No description provided.

- `list_access_roles`: No description provided.

- `del_access_role`: No description provided.

- `add_nsfw_forbid_role`: No description provided.

- `list_nsfw_forbid_roles`: No description provided.

- `del_nsfw_forbid_role`: No description provided.

------
### log_events 
**add_filter_out_channel**: &lt;channel&gt; - Don&#x27;t log events on a certain channel.

**bad_word**: Command usage: `.bad_word <subcommand>`

Available subcommands:

- `add`: &lt;word&gt; - remove a message it contains &#x27;word&#x27;

- `list`: List bad words

- `remove`: &lt;word&gt; - Remove a bad word

**clear_event_log_chan**: &lt;channel&gt; - Clear logging channel and deactivate logging.

**clear_filter_out_channel**: &lt;channel&gt; - Remove channel event filtering.

**get_event_log_chan**: &lt;channel&gt; - Get the event log channel.

**list_filtered_out_channels**: &lt;channel&gt; - List filtered channels.

**set_event_log_chan**: &lt;channel&gt; - Activate event logging and log to channel.

    Logged events: user join, user leave, message edit, message delete, member update, member ban, member unban.

------
### plugin_poll 
**poll**: Command usage: `.poll <subcommand>`

Available subcommands:

- `create`: &lt;title %% option1 %% option2 %% ...&gt; - create a poll with a title and multiple options

- `list`: Lists active polls

- `close`: &lt;message link&gt; - Closes poll give in message link

**sanitize_polls**: TODO: clean up polls, fetch unregistered votes

------
### role_selector 
**selectors**: Command usage: `.selectors <subcommand>`

Available subcommands:

- `description`: &lt;selector&gt; &lt;description&gt; - sets a description for the selector documentation. If the description is &quot;get&quot;, it will instead display the current description

- `max_selectable`: &lt;selector&gt; &lt;maxSelectable (int)&gt; - sets the number of max selectable options for the selector. If maxSelectable &lt;= 0, then the number of max selectable options is unlimited. Ommiting maxSelectable will, instead, display the current set value

- `title`: &lt;selector&gt; &lt;title&gt; - sets a title for the selector. If the title is &quot;get&quot;, it will instead display the current title.

- `add_roles`: &lt;selector&gt; &lt;roles&gt; - adds the specified roles to the selector

- `add_role_interval`: &lt;selector&gt; &lt;role start&gt; &lt;role end&gt; - adds the roles in the specified interval to the selector

- `del_role_interval`: &lt;selector&gt; &lt;role start&gt; &lt;role end&gt; - removes the roles in the specified interval from the selector.

    NOTE: THIS REMOVES THE ROLE INTERVAL FROM THE ROLE LIST, NOT FROM THE SELECTOR LIST.

- `del_roles`: &lt;selector&gt; &lt;roles&gt; - removes the specified roles from the selector

- `create`: &lt;selector name&gt; - create a selector that assigns a role

- `list`: list selector commands

- `remove`: &lt;selector&gt; - delete a selector command

------
### say 
**say**: &lt;channel message&gt; - Send a message to a channel

**say_pm**: &lt;user message&gt; - Send a message to an user.

------
### selector 
**del_permanent_selector**: Remove a permanent selector.

**list_permanent_selectors**: No description provided.

**permanent_selector**: &lt;message link/ID&gt; - makes a generated selector permanent (e.g. the bot will always listen for reacts on the given message).

    This command is useful for pinning selectors on channels.

**rebuild_selectors**: No description provided.

------
### tag 
**tag_del**: &lt;tag&gt; - delete a tag

------
### temp_role 
**ban**: &lt;user [,time], reason&gt; - ban someone permanently or for a given amount of time (e.g. `.ban @plp 5m` bans plp for 5 minutes).

**clear_mod_log_chan**: Clear the moderator actions channel. No moderator actions messages will be sent.

**close_user_case**: &lt;id&gt; - mark user case as closed

**create_temp_role_cmd**: &lt;command name, role&gt; - create a command that assigns a temporary role by specifying `command_name role`

**delete_temp_role_cmd**: &lt;command_name&gt; - delete a temporary role command

**export_cases**: No description provided.

**get_mod_log_chan**: Return the moderator actions channel

**kick**: &lt;user [reason]&gt; - Kick someone with an optional reason

**list_temp_role_cmds**: list temporary role commands

**set_mod_log_chan**: &lt;channel&gt; - Set channel for moderator actions. When a moderator action will be done through the bot, details about the action will be logged to this channel.

**set_temp_role_cmd_type**: No description provided.

**show_user_case**: &lt;id&gt; - show details for a given user case

**timeout**: Timeout an user:

    timeout @plp 1m - timeouts plp for one minute

    timeout @plp - displays timeout for plp

    If the user is timeouted, the timeout can be modified by issuing the timeout command again.

**userhistory**: &lt;user&gt; - List confinement reasons for user

**warn**: &lt;user reason&gt; - Warn a user

------
### watcher 
**clear_rupdates_channel**: Remove reddit updates channel.

**get_rupdates_channel**: List reddit updates annoucement channel.

**set_rupdates_channel**: &lt;channel&gt; - Send reddit updates on channel.

**startwatch**: Start watching subreddits.

**stopwatch**: Stop watching subreddits.

**subwatch_add**: Add a subreddit to the watch list.

**subwatch_del**: Remove a subreddit from the watch list

------
### womenro_admin 
**get_auto_member**: No description provided.

**set_auto_member**: Set auto valoare to a timeout value (e.g. 10h - 10 hours, 100d - 100 days, etc.).

