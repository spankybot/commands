Bot commands:
------
### attacks 
**compliment**: &lt;user&gt; -- Makes the bot compliment &lt;user&gt;.

**gift**: &lt;user&gt; - gives gift to &lt;user&gt;

**insult**: &lt;user&gt; - insults &lt;user&gt;

**kill**: &lt;user&gt; - kills &lt;user&gt;

**lart**: &lt;user&gt; - LARTs &lt;user&gt;

**nk**: outputs a random North Korea propoganda slogan

**sexup**: &lt;user&gt; - flirts with &lt;user&gt;

**slap**: &lt;user&gt; -- Makes the bot slap &lt;user&gt;.

**strax**: Strax quote.

------
### avatar 
**avatar**: &lt;user or user-id&gt; - Get someones avatar

**e**: Expand an emoji

**get_server_banner**: Return a link to the server banner

------
### backup 
**force_backup_data**: No description provided.

------
### bible 
**bible**: &lt;passage&gt; - Prints the specified passage from the Bible

------
### blackmirror_roles 
**charlie**: Assign a role

**nocharlie**: Unassign a role

**verified**: Get server access rights

------
### bot_admin_system 
**about**: Get about.

**system**: -- Retrieves information about the host system.

------
### brainfuck 
**brainfuck**: &lt;prog&gt; - executes &lt;prog&gt; as Brainfuck code

    :type text: str

------
### cats 
**catgifs**: - gets a fucking cat gif.

**cats**: - gets a fucking fact about cats.

------
### cb 
**coa**: &lt;text&gt; - talk to CleverBot

------
### cheer 
**cheer**: :type chan: str

------
### corona 
**corona**: &lt;option&gt; - available options: [all, &lt;country name&gt;]. If option is &lt;country name&gt;, you must specify a country from &lt;https://worldometers.info/coronavirus#countries&gt;.

**corona_format**: &lt;format&gt; - formats the .corona command for you. Every keyword in [&#x27;Cases&#x27;, &#x27;Deaths&#x27;, &#x27;Tests&#x27;, &#x27;CToday&#x27;, &#x27;DToday&#x27;, &#x27;C/M&#x27;, &#x27;D/M&#x27;, &#x27;T/M&#x27;, &#x27;Recovered&#x27;, &#x27;Active&#x27;, &#x27;Critical&#x27;, &#x27;Country&#x27;, &#x27;Continent&#x27;, &#x27;Vaccines&#x27;, &#x27;LUpdated&#x27;] will be replaced with the appropriate data. Use `clear` if you want to clear your format and use the default one

------
### correction 
**s**: &lt;word replacement&gt; - replace &#x27;word&#x27; with replacement

**ss**: &lt;regex replacement&gt; - replace regex with replacement

**toggle_correction_msg_del**: enable/disable automatic deletion of command when running .s/.ss

------
### crypto 
**btc**: - Returns the current btc value

**crypto**: &lt;ticker&gt; [currency] - Returns current value of a cryptocurrency

**eth**: - Returns the current eth value

**ltc**: - Returns the current ltc value

**serak**: No description provided.

------
### cypher 
**cypher**: &lt;pass&gt; &lt;string&gt; -- cyphers &lt;string&gt; with &lt;password&gt;

**decypher**: &lt;pass&gt; &lt;string&gt; - decyphers &lt;string&gt; with &lt;password&gt;

------
### face 
**eyes**: No description provided.

**glasses**: No description provided.

**hat**: No description provided.

**moustache**: No description provided.

------
### fact 
**fact**: - Gets a random fact about numbers or dates.

------
### flip 
**fix**: &lt;text&gt; - fixes a flipped over table. ┬─┬ノ(ಠ_ಠノ)

**flip_text**: &lt;text&gt; - Flips &lt;text&gt; over.

**table**: &lt;text&gt; - (╯°□°）╯︵ &lt;ʇxǝʇ&gt;

------
### gaming 
**choose**: &lt;choice1&gt;, [choice2], [choice3], etc. - randomly picks one of the given choices

    :type text: str

**coin**: [amount] - flips [amount] coins

    :type text: str

**dice**: &lt;dice roll&gt; - simulates dice rolls. Example: &#x27;dice 2d20-d5+4 roll 2&#x27;: D20s, subtract 1D5, add 4

    :type text: str

------
### giphy 
**gif**: &lt;query&gt; - Searches giphy.com for a gif using the provided search term.

------
### github 
**ghissue**: &lt;username|repo&gt; [number] - gets issue [number]&#x27;s summary, or the open issue count if no issue is specified

------
### goodreads 
**goodreads**: &lt;text&gt; - List first goodreads result.

**goodreads_search**: &lt;text&gt; - Search for books on Goodreads.

------
### grab 
**grab**: &lt;user&gt; - grab user&#x27;s last message. If &lt;user&gt; is empty, it will try to grab the message you&#x27;re replying to

**grabl**: &lt;user&gt; - List quotes for user. If no user is specified, it lists everything on the server.

**grabr**: Grab random quote

**grabs**: &lt;expression&gt; - Search for &#x27;expression&#x27; in grab texts.

**grabu**: &lt;user&gt; - Grab random quote from user

------
### help 
**help**: Get help for a command or the help document

------
### igen 
**igen**: Command usage: `.igen <subcommand>`

Available subcommands:

- `t2i`: &lt;prompt&gt; &lt;negative_prompt&gt; - Generate an image from text. Use quotes if you want to use spaces in the prompt.

------
### imdb 
**imdb**: &lt;movie&gt; - gets information about &lt;movie&gt; from IMDb

------
### img_manip 
**cat**: No description provided.

**crowd**: No description provided.

**df**: Deepfry image

**flip**: Flip image horizontally

**flop**: Flip image vertically

**fried**: No description provided.

**hue**: No description provided.

**img_text**: Add text to image

**implode**: Implode image

**negate**: Invert colors

**noise**: No description provided.

**npc**: No description provided.

**pulse**: No description provided.

**rain**: No description provided.

**resize**: Resize image

**roll**: No description provided.

**scan**: No description provided.

**shake**: No description provided.

**tint**: No description provided.

**wobble**: No description provided.

**woke**: No description provided.

**zoom**: No description provided.

------
### irc 
**accept_invite**: No description provided.

**irc**: Command usage: `.irc <subcommand>`

Available subcommands:

- `member <subcommand>`: Available subcommands:
> - `list`: List members

- `op <subcommand>`: Available subcommands:
> - `add`: &lt;name&gt; - Add an operator
> - `list`: List operators
> - `remove`: &lt;name&gt; - Remove an operator

- `set <subcommand>`: Available subcommands:
> - `topic`: &lt;topic&gt; - set channel topic
> - `nsfw`: &lt;topic&gt; - make channel NSFW
> - `sfw`: &lt;topic&gt; - make channel SFW
> - `permission_based`: Instead of managing access through roles, it uses channel permissions
> - `role_based`: Instead of managing access through permissions, it uses role access
> - `associated_role`: Set the role name associated to the channel

- `get <subcommand>`: Available subcommands:
> - `associated_role`: Get the role name associated to the channel

- `ban <subcommand>`: Available subcommands:
> - `list`: List channel bans
> - `member`: &lt;name/ID&gt; - ban a member
> - `unban`: &lt;name/ID&gt; - unban a member

- `kick`: &lt;name/ID&gt; - kick a member

------
### jokes 
**awesome**: - Prints a webpage to show &lt;nick&gt; how awesome they are.

**boobs**: - prints boobies!

**bookpun**: - Suggests a pun of a book title/author.

**confucious**: - confucious say man standing on toilet is high on pot.

**dadjoke**: - love em or hate em, bring on the dad jokes.

**doit**: - prints a do it line, example: mathmaticians do with a pencil

**lawyerjoke**: - returns a lawyer joke, so lawyers know how much we hate them

**pun**: - Come on everyone loves puns right?

**triforce**: - returns a triforce!

**wisdom**: - words of wisdom from various bathroom stalls.

------
### llm 
**llm**: No description provided.

**llm_reset**: Reset the chat history

------
### lurve 
**lurve**: lurves all over &lt;user&gt;

------
### magik 
**gmagik**: No description provided.

**magik**: No description provided.

------
### markov 
**markov**: &lt;user channel&gt; - Generate sentence using a markov chain for a user using data from the given channel.

    If no user is specified, a sentence will be generated using all user messages.

------
### pipe 
**pipe**: Command usage: `.pipe <subcommand>`

Available subcommands:

- `create`: &lt;name&gt; &lt;description&gt;: Create a new pipe

- `list`: List all pipes

- `delete`: &lt;name&gt;: Delete a pipe

- `trigger <subcommand>`: Available subcommands:
> - `list`: List all triggers

- `action <subcommand>`: Available subcommands:
> - `list`: List all actions

------
### plugin_dogpile 
**g**: &lt;query&gt; - Search for a link.

**gis**: &lt;query&gt; - Search for a image.

**nsfwgis**: &lt;query&gt; - Search for a image.

------
### plugin_poll 
**close_poll**: No description provided.

**create_poll**: No description provided.

**list_polls**: No description provided.

------
### qalc 
**calc**: &lt;expression&gt; - qalc interface

------
### quran 
**quran**: &lt;verse&gt; - Prints the specified Qur&#x27;anic verse(s) and its/their translation(s)

------
### remind 
**remind**: &lt;period message&gt; - ask the bot to remind you about something in given period (e.g. &#x27;.remind 1h bleh bleh&#x27; sends you &#x27;bleh bleh&#x27; in one hour

------
### remote_plugins 
**igram**: No description provided.

**tt**: No description provided.

------
### roddit_curs 
**curs**: &lt;currency&gt; - Returns current value of a currency in RON

------
### roddit_dex 
**dex**: &lt;cuvant&gt; - Cauta definitia pentru un cuvant in DEX

------
### roddit_family 
**accept_adoption**: &lt;id&gt; - Acceptă o ofertă de adopție

**accept_marry**: &lt;id&gt; - Acceptă o ofertă de căsătorie.

**deny_adoption**: &lt;id&gt; - Refuză o ofertă de adopție

**deny_marry**: &lt;id&gt; - Refuză o ofertă de căsătorie

------
### roddit_horoscop 
**horoscop**: horoscop &lt;zodie&gt; - Afișează horoscopul unei zodii

**horoscop2**: horoscop2 &lt;zodie&gt; - Afișează horoscopul unei zodii

**horoscop3**: &lt;zodie&gt;

**horoscop3_get**: No description provided.

**horoscop3_reset**: No description provided.

**horoscop3_set**: No description provided.

------
### roddit_inactive 
**inactive**: Command usage: `.inactive <subcommand>`

Available subcommands:

- `manual_run`: Run the inactive check manually.

- `force_user`: Force a user to be marked as inactive.

- `tutorial`: No description provided.

- `timeout <subcommand>`: Available subcommands:
> - `set`: Set the timeout for inactive users: 1d, 1h, 1m, 1s or a combination of those.
> - `remove`: Remove the timeout for inactive users.
> - `list`: List the timeout for inactive users.

- `notify_chan <subcommand>`: Available subcommands:
> - `set`: Set the channel where notifications are sent when a user is marked as inactive or active.
> - `remove`: Remove the channel where notifications are sent when a user is marked as inactive or active.
> - `list`: List the channel where notifications are sent when a user is marked as inactive or active.

- `addable <subcommand>`: Available subcommands:
> - `add`: Add a role to the list of roles to be added when a user is marked as inactive.
> - `remove`: Remove a role from the list of roles to be added when a user is marked as inactive.
> - `list`: List all roles that are added when a user is marked as inactive.

- `removable <subcommand>`: Available subcommands:
> - `add`: Add a role to the list of roles to be removed when a user is marked as inactive.
> - `remove`: Remove a role from the list of roles to be removed when a user is marked as inactive.
> - `list`: List all roles that are removed when a user is marked as inactive.

- `user_notify_chan <subcommand>`: Available subcommands:
> - `set`: Set the channel where the user is pinged when marked as active.
> - `remove`: Remove the channel where the user is pinged.
> - `list`: List the channel where the user is pinged.

- `explain`: Explain the settings.

- `activity <subcommand>`: Available subcommands:
> - `breakdown`: Produces a report of the activity of users.
> - `users`: Produces a report of the activity of users.
> - `users_kick`: No description provided.

------
### shorten 
**expand**: &lt;url&gt; - unshortens &lt;url&gt;

**isgd**: &lt;url&gt; [custom] - shortens a url using is.gd with [custom] as an optional custom shortlink,

    or unshortens &lt;url&gt; if already short

**shorten**: &lt;url&gt; [custom] - shortens a url with [custom] as an optional custom shortlink

------
### spamfun 
**bang**: Bang bang.

**spamfun**: Command usage: `.spamfun <subcommand>`

Available subcommands:

- `chan_set`: Set the channel to spam in.

- `chan_unset`: Unset the channel to spam in.

- `chan_get`: Get the channel to spam in.

- `duckhunt_start`: Start duck hunt.

- `duckhunt_stop`: Stop duck hunt.

- `duckhunt_get`: Get duck hunt.

- `emit_duck`: Emit a duck.

- `duck_score`: Get duck score.

------
### spank 
**bdsm**: Just a little bit of kinky fun.

**spank**: &lt;user&gt; - Spanks a  &lt;user&gt;

------
### steam 
**steam**: &lt;text or ID&gt; - Search for a Steam game by name or ID.

**steamsearch**: &lt;text&gt; - Search steam for games.

------
### stock 
**dquote**: No description provided.

**quote**: No description provided.

**stock**: No description provided.

------
### suggest 
**suggest**: &lt;phrase&gt; - Gets suggested phrases for a google search

------
### system 
**invite_me**: Get invitation for bot

------
### tag 
**tag**: &lt;tag&gt; - Return a tag. &#x27;.tag list&#x27; lists tags, &#x27;.tag random&#x27; returns random tag

**tag_add**: &lt;identifier content&gt; - add tag content as indentifier

------
### text 
**letters**: &lt;text&gt; - text to emoji letters

------
### time_plugin 
**beats**: - Gets the current time in .beats (Swatch Internet Time).

**time**: &lt;location&gt; - Gets the current time in &lt;location&gt;.

------
### txt2img 
**txt2img**: Generate a image using sent text

    &quot;&lt;option&gt; - available input for custom fonts:

    .image &lt;font name&gt;-&lt;size&gt;-&lt;text color&gt;-&lt;bg color&gt;

    VALID_FONTS=

    &#x27;sofia&#x27;,

    &#x27;ostirch&#x27;,

    &#x27;diso&#x27;,

    &#x27;learning&#x27;,

    &#x27;hotel&#x27;,

    &#x27;plp&#x27;,

    &#x27;default&#x27;

    &#x27;symbols&#x27;

    Example usage of this command :

    .text2img sofia-30-red-yellow the quick brown fox jumps over the lazy dog

------
### urban 
**urban**: urban &lt;phrase&gt; [id] -- Looks up &lt;phrase&gt; on urbandictionary.com.

------
### userinfo 
**inrole**: [role name] List how many members each role has. Calling it with no role name will list all roles

**userinfo**: &lt;mention&gt; - gets various data about the mentioned user

------
### utility 
**base64**: &lt;string&gt; -- Encode &lt;string&gt; with base64.

**capitalize**: &lt;string&gt; -- Capitalizes &lt;string&gt;.

    :type text: str

**debase64**: &lt;string&gt; -- Decode &lt;string&gt; with base64.

**derpify**: &lt;text&gt; - returns some amusing responses from your input.

**escape**: &lt;string&gt; -- Unicode escapes &lt;string&gt;.

**hash**: &lt;string&gt; -- Returns hashes of &lt;string&gt;.

**isbase64**: &lt;string&gt; -- Checks if &lt;string&gt; is a valid base64 encoded string

**leet**: &lt;text&gt; -- Makes &lt;text&gt; more 1337h4x0rz.

**length**: &lt;string&gt; -- Gets the length of &lt;string&gt;

**lower**: &lt;string&gt; -- Convert string to lowercase.

**qrcode**: &lt;link&gt; - returns a link to a QR code image for &lt;link&gt;

**reverse**: &lt;string&gt; -- Reverses &lt;string&gt;.

**rot13**: &lt;string&gt; -- Encode &lt;string&gt; with rot13.

**superscript**: &lt;text&gt; -- Makes &lt;text&gt; superscript.

**swapcase**: &lt;string&gt; -- Swaps the capitalization of &lt;string&gt;.

**titlecase**: &lt;string&gt; -- Convert string to title case.

**unescape**: &lt;string&gt; -- Unicode unescapes &lt;string&gt;.

**upper**: &lt;string&gt; -- Convert string to uppercase.

**vapor**: &lt;string&gt; -- Converts &lt;string&gt; to full width characters.

------
### uwu 
**uwu**: &lt;text&gt; - translate text to UwU

------
### vicky 
**vicky**: &lt;hot&gt; &lt;crazy&gt; - Returns the zone from the universal hot crazy matrix

------
### wandbox 
**wb**: wandbox interface

------
### watcher 
**subwatch_list**: List watched subreddits.

------
### weather 
**weather**: &lt;location&gt; - Gets weather data for &lt;location&gt;.

------
### whois 
**whois**: &lt;domain&gt; - Does a whois query on &lt;domain&gt;.

------
### youtube 
**youtube**: &lt;query&gt; - Returns the first YouTube search result for &lt;query&gt;.

