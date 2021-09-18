Admin commands:
------
### admin 
**add_admin_role**: &lt;role&gt; - Add role that can run administrative bot commands.

**add_chan_to_chgroup**: &lt;channel channel-group&gt; - Add channel to channel group

**add_channel_group**: &lt;group-name&gt; - Create a group of channels

**add_chgroup_to_cmd**: &lt;command channel-group&gt; - Add a channel-group to a command. The command will only be usable in that channel.

**add_fchgroup_to_cmd**: &lt;command channel-group&gt; - Add a forbidden channel-group to command

**add_owner_to_cmd**: &lt;command user-group&gt; - Add a user-group to own a command

**clear_default_bot_channel**: &lt;channel&gt; - Configure a channel where any bot command can be used, unless otherwise specified.

**del_chan_from_chgroup**: &lt;channel channel-group&gt; - Delete channel from channel group

**del_channel_group**: &lt;group-name&gt; - Delete a group of channels

**del_chgroup_from_cmd**: &lt;command channel-group&gt; - Delete a user-group from a command&#x27;s ownership

**del_fchgroup_from_cmd**: &lt;command channel-group&gt; - Delete a user-group from a command&#x27;s forbidden list

**del_owner_from_cmd**: &lt;command user-group&gt; - Delete user-group from command ownership list

**get_admin_roles**: No documentation provided.

**is_cmd_unrestricted**: &lt;command&gt; - Check if command is channel restricted or not

**list_channel_groups**: List available groups of channels

**list_chans_in_chgroup**: &lt;channel-group&gt; - List channels in channel-group

**list_chgroups_for_cmd**: &lt;command&gt; - List in what channel-groups command is usable

**list_default_bot_channel**: List the built in bot command channel.

**list_fchgroups_for_cmd**: &lt;command&gt; - List in what channel-groups command is NOT usable

**list_owners_for_cmd**: &lt;command&gt; - List what user-groups own a command

**remove_admin_role**: No documentation provided.

**remove_restrictions_for_cmd**: &lt;command&gt; - Remove channel restrictions for a command to make it usable on the whole server

**restore_restrictions_for_cmd**: &lt;command user-group&gt; - Restore channel restrictions for command

**set_default_bot_channel**: &lt;channel&gt; - Configure a channel where any bot command can be used, unless otherwise specified by other rules.

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

------
### log_events 
**add_bad_word**: &lt;word&gt; - remove a message it contains &#x27;word&#x27;

**add_filter_out_channel**: &lt;channel&gt; - Don&#x27;t log events on a certain channel.

**clear_event_log_chan**: &lt;channel&gt; - Clear logging channel and deactivate logging.

**clear_filter_out_channel**: &lt;channel&gt; - Remove channel event filtering.

**get_event_log_chan**: &lt;channel&gt; - Get the event log channel.

**list_bad_words**: List bad words

**list_filtered_out_channels**: &lt;channel&gt; - List filtered channels.

**remove_bad_word**: &lt;word&gt; - Remove a bad word

**set_event_log_chan**: &lt;channel&gt; - Activate event logging and log to channel.

Logged events: user join, user leave, message edit, message delete, member update, member ban, member unban.

------
### poll 
**close_poll**: &lt;message link&gt; - Closes poll give in message link

**create_poll**: &lt;title %% option1 %% option2 %% ...&gt; - create a poll with a title and multiple options

**list_polls**: Lists active polls

------
### roddit_irc_mode 
**add_access_role**: No documentation provided.

**get_access_roles**: No documentation provided.

**remove_access_role**: No documentation provided.

------
### role_selector 
**add_selector_role_interval**: &lt;selector&gt; &lt;role start&gt; &lt;role end&gt; - adds the roles in the specified interval to the selector

**add_selector_roles**: &lt;selector&gt; &lt;roles&gt; - adds the specified roles to the selector

**create_selector**: &lt;selector name&gt; - create a selector that assigns a role

**delete_selector**: &lt;command_name&gt; - delete a temporary selector command

**remove_selector_role_interval**: &lt;selector&gt; &lt;role start&gt; &lt;role end&gt; - removes the roles in the specified interval from the selector.

    NOTE: THIS REMOVES THE ROLE INTERVAL FROM THE ROLE LIST, NOT FROM THE SELECTOR LIST.

**remove_selector_roles**: &lt;selector&gt; &lt;roles&gt; - removes the specified roles from the selector

**set_selector_description**: &lt;selector&gt; &lt;description&gt; - sets a description for the selector documentation

**set_selector_max_selectable**: &lt;selector&gt; &lt;maxSelectable (int)&gt; - sets the number of max selectable options for the selector. If maxSelectable &lt;= 0, then the number of max selectable options is unlimited

**set_selector_title**: &lt;selector&gt; &lt;title&gt; - sets a title for the selector

------
### say 
**say**: &lt;channel message&gt; - Send a message to a channel

**say_pm**: &lt;user message&gt; - Send a message to an user.

------
### selector 
**del_permanent_selector**: Remove a permanent selector.

**list_permanent_selectors**: No documentation provided.

**permanent_selector**: &lt;message link/ID&gt; - makes a generated selector permanent (e.g. the bot will always listen for reacts on the given message).

    This command is useful for pinning selectors on channels.

**rebuild_selectors**: No documentation provided.

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

**export_cases**: No documentation provided.

**get_mod_log_chan**: Return the moderator actions channel

**ghinion**: Temporary role assignment command as defined by server ops.

**kick**: &lt;user [reason]&gt; - Kick someone with an optional reason

**list_temp_role_cmds**: list temporary role commands

**set_mod_log_chan**: &lt;channel&gt; - Set channel for moderator actions. When a moderator action will be done through the bot, details about the action will be logged to this channel.

**set_temp_role_cmd_type**: No documentation provided.

**show_user_case**: &lt;id&gt; - show details for a given user case

**userhistory**: &lt;user&gt; - List confinement reasons for user

**warn**: &lt;user reason&gt; - Warn a user

------
### watch 
**clear_rupdates_channel**: Remove reddit updates channel.

**get_rupdates_channel**: List reddit updates annoucement channel.

**set_rupdates_channel**: &lt;channel&gt; - Send reddit updates on channel.

**startwatch**: Start watching subreddits.

**stopwatch**: Stop watching subreddits.

**subwatch_add**: Add a subreddit to the watch list.

**subwatch_del**: Remove a subreddit from the watch list

