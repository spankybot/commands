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

**del_join_event**: &lt;event&gt; - delete a join event

**get_timeout_for**: Get timeout for a join event

**list_join_events**: List on-join events

**set_timeout_for**: &lt;join event, timeout&gt; - Set timeout for a join event. Use &#x27;5s&#x27; for timeout to set it to 5s or 1m to set it to one minute.

------
### auto_order 
**add_chan_to_auto_order**: &lt;channel&gt; -

**del_chan_from_auto_order**: &lt;channel&gt; -

**list_auto_order_chans**: Lists channels that are auto ordered

------
### del_messages 
**delete**: &lt;number&gt; - delete a given number of messages from the channel where the command is executed

------
### grab 
**del_grab**: Delete a grab entry. Specify what the grab message contains or the message ID

------
### help 
**gen_documentation**: No documentation provided.

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
### tag 
**tag_del**: &lt;tag&gt; - delete a tag

------
### temp_role 
**aaaaa**: Temporary role assignment command as defined by server ops.

**ban**: &lt;user [,time], reason&gt; - ban someone permanently or for a given amount of time (e.g. `.ban @plp 5m` bans plp for 5 minutes).

**bbbbb**: Temporary role assignment command as defined by server ops.

**clear_mod_log_chan**: Clear the moderator actions channel. No moderator actions messages will be sent.

**close_user_case**: &lt;id&gt; - mark user case as closed

**create_temp_role_cmd**: &lt;command name, role&gt; - create a command that assigns a temporary role by specifying `command_name role`

**delete_temp_role_cmd**: &lt;command_name&gt; - delete a temporary role command

**get_mod_log_chan**: Return the moderator actions channel

**kick**: &lt;user [reason]&gt; - Kick someone with an optional reason

**list_temp_role_cmds**: list temporary role commands

**set_mod_log_chan**: &lt;channel&gt; - Set channel for moderator actions. When a moderator action will be done through the bot, details about the action will be logged to this channel.

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

