Bot commands:
------
### admin 
**del_owner_from_cmd**: &lt;command user-group&gt; - Delete user-group from command ownership list

**list_channel_groups**: List available groups of channels

**list_user_groups**: List user groups

**add_chan_to_chgroup**: &lt;channel channel-group&gt; - Add channel to channel group

**get_admin_roles**: No documentation provided.

**add_channel_group**: &lt;group-name&gt; - Create a group of channels

**add_owner_to_cmd**: &lt;command user-group&gt; - Add a user-group to own a command

**list_owners_for_cmd**: &lt;command&gt; - List what user-groups own a command

**set_default_bot_channel**: &lt;channel&gt; - Configure a channel where any bot command can be used, unless otherwise specified by other rules.

**list_fchgroups_for_cmd**: &lt;command&gt; - List in what channel-groups command is NOT usable

**del_chgroup_from_cmd**: &lt;command channel-group&gt; - Delete a user-group from a command&#x27;s ownership

**del_channel_group**: &lt;group-name&gt; - Delete a group of channels

**del_chan_from_chgroup**: &lt;channel channel-group&gt; - Delete channel from channel group

**list_users_in_ugroup**: No documentation provided.

**clear_default_bot_channel**: &lt;channel&gt; - Configure a channel where any bot command can be used, unless otherwise specified.

**del_user_group**: &lt;group name&gt; - Deletes a user group

**del_fchgroup_from_cmd**: &lt;command channel-group&gt; - Delete a user-group from a command&#x27;s forbidden list

**list_chans_in_chgroup**: &lt;channel-group&gt; - List channels in channel-group

**add_user_group**: &lt;group name&gt; - Create a user group

**add_chgroup_to_cmd**: &lt;channel-group command&gt; - Add a channel-group to a command. The command will only be usable in that channel.

**add_admin_role**: &lt;role&gt; - Add role that can run administrative bot commands.

**list_default_bot_channel**: List the built in bot command channel.

**add_fchgroup_to_cmd**: &lt;command channel-group&gt; - Add a forbidden channel-group to command

**del_user_from_ugroup**: &lt;user user-group&gt; - Delete user from user group

**list_chgroups_for_cmd**: &lt;command&gt; - List in what channel-groups command is usable

**remove_admin_role**: No documentation provided.

**add_user_to_ugroup**: &lt;user user-group&gt; - Add user to user group

------
### admin_utils 
**add_join_event**: &lt;&#x27;type&#x27; &#x27;option&#x27;&gt; - Add action to be triggered on user join.

    Possible actions: 

        - message #channel blahblah -&gt; send blahblah to #channel

        - role @role -&gt; set @role on join).

    The scripted message can contain special words that are replaced when the event is triggered:

    - {AGE} - Account age

    - {USER} - User that just joined

    - {USER_ID} - User ID

    

    e.g. &#x27;message #general {USER} / {USER_ID} just joined!&#x27; will send &#x27;John / 12345678910 just joined!&#x27;

**del_join_event**: &lt;event&gt; - delete a join event

**list_join_events**: List on-join events

**kick**: &lt;user&gt; - Kick someone

**ban**: &lt;user&gt; - Ban someone

------
### animal_gifs 
**doggifs**: - Returns a random dog GIF from http://bestanimations.com/

------
### attacks 
**nk**: outputs a random North Korea propoganda slogan

**slap**: &lt;user&gt; -- Makes the bot slap &lt;user&gt;.

**lart**: &lt;user&gt; - LARTs &lt;user&gt;

**gift**: &lt;user&gt; - gives gift to &lt;user&gt;

**sexup**: &lt;user&gt; - flirts with &lt;user&gt;

**insult**: &lt;user&gt; - insults &lt;user&gt;

**compliment**: &lt;user&gt; -- Makes the bot compliment &lt;user&gt;.

**kill**: &lt;user&gt; - kills &lt;user&gt;

**strax**: Strax quote.

------
### avatar 
**avatar**: &lt;user or user-id&gt; - Get someones avatar

------
### bible 
**bible**: &lt;passage&gt; - Prints the specified passage from the Bible

------
### books 
**books**: &lt;query&gt; - Searches Google Books for &lt;query&gt;.

------
### brainfuck 
**brainfuck**: &lt;prog&gt; - executes &lt;prog&gt; as Brainfuck code

    :type text: str

------
### brew 
**brew**: &lt;query&gt; - returns the first brewerydb search result for &lt;query&gt;

------
### cats 
**catgifs**: - gets a fucking cat gif.

**cats**: - gets a fucking fact about cats.

------
### cb 
**coa**: No documentation provided.

------
### cryptocurrency 
**dogecoin / doge**: - Returns the current dogecoin value

**dogecoin / doge**: - Returns the current dogecoin value

**crypto**: &lt;ticker&gt; [currency] - Returns current value of a cryptocurrency

**bitcoin / btc**: - Returns the current bitcoin value

**bitcoin / btc**: - Returns the current bitcoin value

**litecoin / ltc**: - Returns the current litecoin value

**litecoin / ltc**: - Returns the current litecoin value

------
### cypher 
**decypher**: &lt;pass&gt; &lt;string&gt; - decyphers &lt;string&gt; with &lt;password&gt;

**cypher**: &lt;pass&gt; &lt;string&gt; -- cyphers &lt;string&gt; with &lt;password&gt;

------
### del_messages 
**delete**: &lt;number&gt; - delete a given number of messages from the channel where the command is executed

------
### dex 
**dex**: No documentation provided.

------
### dogpile 
**gis**: &lt;query&gt; - Uses the dogpile search engine to search for images.

**g**: &lt;query&gt; - Uses the dogpile search engine to find shit on the web.

------
### domainr 
**domain**: &lt;domain&gt; - uses domain.nr&#x27;s API to search for a domain, and similar domains

    :type text: str

------
### dramatica 
**drama**: &lt;phrase&gt; - gets the first paragraph of the Encyclopedia Dramatica article on &lt;phrase&gt;

------
### drinks 
**drink**: &lt;nick&gt; - makes the user a random cocktail.

------
### eightball 
**8ball**: &lt;question&gt; - asks the all knowing magic electronic eight ball &lt;question&gt;

------
### etymology 
**etymology**: &lt;word&gt; - retrieves the etymology of &lt;word&gt;

    :type text: str

------
### fact 
**fact**: - Gets a random fact about numbers or dates.

------
### flip 
**fix**: &lt;text&gt; - fixes a flipped over table. ┬─┬ノ(ಠ_ಠノ)

**flip**: &lt;text&gt; - Flips &lt;text&gt; over.

**table**: &lt;text&gt; - (╯°□°）╯︵ &lt;ʇxǝʇ&gt;

------
### fmk 
**fmk**: [nick] - Fuck, Marry, Kill

------
### foaas 
**fuckoff**: [name] - tell some one to fuck off or just .fos for a generic fuckoff

------
### foods 
**pancake**: &lt;user&gt; - gives pancakes to [user]

**cookie**: &lt;user&gt; - gives a cookie to [user]

**pie**: &lt;user&gt; - gives pie to [user]

**cereal**: &lt;user&gt; - gives cereal to [user]

**brekkie / brekky**: &lt;user&gt; - gives brekkie to [user]

**tea**: &lt;user&gt; - gives tea to [user]

**soup**: &lt;user&gt; - gives Some Soup to [user]

**noodles**: &lt;user&gt; - gives noodles to [user]

**chocolate**: &lt;user&gt; - gives chocolate to [user]

**sandwich**: &lt;user&gt; - gives a sandwich to [user]

**halal / halaal**: &lt;user&gt; - gives food to [user]

**milkshake**: &lt;user&gt; - gives a milkshake to [user]

**nugget**: &lt;user&gt; - gives nuggets to [user]

**doobie**: &lt;user&gt; - gives a doobie to [user]

**brekkie / brekky**: &lt;user&gt; - gives brekkie to [user]

**kosher**: &lt;user&gt; - gives food to [user]

**sushi**: &lt;user&gt; - gives sushi to [user]

**pasta**: &lt;user&gt; - gives pasta to [user]

**kebab**: &lt;user&gt; - gives a kebab to [user]

**wine**: &lt;user&gt; - gives wine to [user]

**halal / halaal**: &lt;user&gt; - gives food to [user]

**burger**: &lt;user&gt; - gives a tasty burger to [user]

**pizza**: &lt;user&gt; - gives pizza to [user]

**cake**: &lt;user&gt; - gives a cake to [user]

**keto**: &lt;user&gt; - gives food to [user]

**icecream**: &lt;user&gt; - gives icecream to [user]

**scone**: &lt;user&gt; - gives a scone to [user]

**potato**: &lt;user&gt; - gives a potato to [user]

**cheese**: &lt;user&gt; - gives cheese to [user]

**muffin**: &lt;user&gt; - gives a muffin to [user]

**steak**: &lt;user&gt; - gives a nice steak dinner to [user]

**rice**: &lt;user&gt; - gives rice to [user]

**chicken**: &lt;user&gt; - gives chicken to [user]

**taco**: &lt;user&gt; - gives a taco to [user]

**beer**: &lt;user&gt; - gives beer to [user]

**coffee**: &lt;user&gt; - gives coffee to [user]

**donut**: &lt;user&gt; - gives a donut to [user]

------
### fortune 
**fortune**: - hands out a fortune cookie

------
### gaming 
**roll**: &lt;dice roll&gt; - simulates dice rolls. Example: &#x27;dice 2d20-d5+4 roll 2&#x27;: D20s, subtract 1D5, add 4

    :type text: str

**coin**: [amount] - flips [amount] coins

    :type text: str

**choose**: &lt;choice1&gt;, [choice2], [choice3], etc. - randomly picks one of the given choices

    :type text: str

------
### giphy 
**gif**: &lt;query&gt; - Searches giphy.com for a gif using the provided search term.

------
### github 
**ghissue**: &lt;username|repo&gt; [number] - gets issue [number]&#x27;s summary, or the open issue count if no issue is specified

------
### gnomeagainsthumanity 
**cahb**: &lt;text&gt; - Submit text with _ for the bot to fill in the rest. You can submit text with multiple _

**cah**: &lt;text&gt; - Submit text to be used as a CAH whitecard

------
### grab 
**grabl**: &lt;user&gt; - List quotes for user.  

**grabs**: &lt;expression&gt; - Search for &#x27;expression&#x27; in grab texts.  

**grab**: &lt;user&gt; - grab user&#x27;s last message

**grabu**: &lt;user&gt; - Grab random quote from user

------
### help 
**gen_documentation**: No documentation provided.

**help**: Get help for a command or the help document

------
### imdb 
**imdb**: &lt;movie&gt; - gets information about &lt;movie&gt; from IMDb

------
### issafe 
**issafe**: &lt;website&gt; -- Checks the website against Google&#x27;s Safe Browsing List.

------
### jokes 
**confucious**: - confucious say man standing on toilet is high on pot.

**lawyerjoke**: - returns a lawyer joke, so lawyers know how much we hate them

**yomomma**: &lt;nick&gt; - tells a yo momma joke to &lt;nick&gt;

**pun**: - Come on everyone loves puns right?

**triforce**: - returns a triforce!

**doit**: - prints a do it line, example: mathmaticians do with a pencil

**boobs**: - prints boobies!

**bookpun**: - Suggests a pun of a book title/author.

**dadjoke**: - love em or hate em, bring on the dad jokes.

**awesome**: - Prints a webpage to show &lt;nick&gt; how awesome they are.

**wisdom**: - words of wisdom from various bathroom stalls.

------
### kenm 
**kenm**: - Wisdom from Ken M.

------
### lenny 
**lenny**: why the shit not lennyface

**flenny**: flenny is watching.

------
### linux 
**kernel**: - gets a list of linux kernel versions

------
### lmgtfy 
**lmgtfy**: [phrase] - gets a lmgtfy.com link for the specified phrase

------
### log_events 
**list_filtered_out_channels**: &lt;channel&gt; - List filtered channels.

**get_event_log_chan**: &lt;channel&gt; - Get the event log channel.

**set_event_log_chan**: &lt;channel&gt; - Activate event logging and log to channel.

Logged events: user join, user leave, message edit, message delete, member update, member ban, member unban.

**add_filter_out_channel**: &lt;channel&gt; - Don&#x27;t log events on a certain channel.

**clear_filter_out_channel**: &lt;channel&gt; - Remove channel event filtering.

**clear_event_log_chan**: &lt;channel&gt; - Clear logging channel and deactivate logging.

------
### lurve 
**lurve**: lurves all over &lt;user&gt;

------
### metacritic 
**metacritic**: [all|movie|tv|album|x360|ps3|pc|gba|ds|3ds|wii|vita|wiiu|xone|ps4] &lt;title&gt; - gets rating for &lt;title&gt; from

     metacritic on the specified medium

------
### metars 
**taf**: [ICAO station code] - returns the taf information for the specified station. A list of station codes can be found here: http://weather.rap.ucar.edu/surface/stations.txt

**metar**: [ICAO station code] - returns the metars information for the specified station. A list of station codes can be found here: http://weather.rap.ucar.edu/surface/stations.txt

------
### mock 
**mock**: &lt;nick&gt; - turn &lt;user&gt;&#x27;s last message in to aLtErNaTiNg cApS

------
### name_generator 
**namegen**: [generator|list] - generates some names using the chosen generator, or lists all generators if &#x27;list&#x27; is specified

    :type bot: cloudbot.bot.CloudBot

------
### pagecheck 
**down**: &lt;url&gt; - checks if &lt;url&gt; is online or offline

    :type text: str

**isup**: &lt;url&gt; - uses isup.me to check if &lt;url&gt; is online or offline

    :type text: str

------
### ping 
**ping**: &lt;host&gt; [count] - pings &lt;host&gt; [count] times

------
### porn 
**buci**: No documentation provided.

**fetch_image**: No documentation provided.

**anal**: No documentation provided.

**capre**: No documentation provided.

**milf**: No documentation provided.

**craci**: No documentation provided.

**force_refresh_porn**: No documentation provided.

**lesbiene**: No documentation provided.

**aww**: No documentation provided.

**nsfwfunny**: No documentation provided.

**tzatze**: No documentation provided.

**sloboz**: No documentation provided.

**blep**: No documentation provided.

**cutu**: No documentation provided.

**tatuate**: No documentation provided.

**pisi**: No documentation provided.

**roscate**: No documentation provided.

**teen**: No documentation provided.

**traps**: No documentation provided.

**thicc**: No documentation provided.

**amateur**: No documentation provided.

**skinny**: No documentation provided.

------
### quran 
**quran**: &lt;verse&gt; - Prints the specified Qur&#x27;anic verse(s) and its/their translation(s)

------
### randomusefulwebsites 
**randomusefulsite**: No documentation provided.

------
### reactions 
**fetish**: &lt;nick&gt; - Did some one just mention what your fetish was? Let &lt;nick&gt; know! Code located in reactions.py

**facepalm**: &lt;nick&gt; - Expresses your frustration with &lt;Nick&gt;. Code located in reactions.py

**dealwithit**: &lt;nick&gt; - Tell &lt;nick&gt; in the channel to deal with it. Code located in reactions.py

**headdesk**: &lt;nick&gt; - Hit your head against the desk becausae of &lt;nick&gt;. Code located in reactions.py

------
### recipe 
**dinner**: - TELLS YOU WHAT THE F**K YOU SHOULD MAKE FOR DINNER

**recipe**: [term] - gets a recipe for [term], or gets a random recipe if no term is specified

------
### roddit_bulau 
**bulautime**: Print remaining time in bulau

**bulau**: &lt;user, duration&gt; - assign bulau role for specified time - duration can be seconds, minutes, hours, days. To set a 10 minute 15 seconds timeout for someone, type: &#x27;.bulau @user 10m15s&#x27;. The abbrebiations are: s - seconds, m - minutes, h - hours, d - days.

------
### roddit_color 
**color**: No documentation provided.

------
### roddit_fun 
**shrug**: No documentation provided.

**cacat**: No documentation provided.

**ayy**: No documentation provided.

**bluntlee**: No documentation provided.

**iazo**: No documentation provided.

**muie**: No documentation provided.

**puti**: No documentation provided.

**jupi**: No documentation provided.

**mtutea**: No documentation provided.

**bitter**: No documentation provided.

**mpuric**: No documentation provided.

**cola**: No documentation provided.

**brutalistu**: No documentation provided.

**mcioran**: No documentation provided.

**dance**: No documentation provided.

**aplauze**: No documentation provided.

**murmuz**: No documentation provided.

------
### roddit_intrebati_orice 
**clear_roddit_channel**: Remove &#x27;intrebati orice&#x27; announcement channel.

**get_roddit_channel**: List &#x27;intrebati orice&#x27; annoucement channel.

**set_roddit_channel**: &lt;channel&gt; - Send &#x27;intrebati orice&#x27; on channel.

------
### rottentomatoes 
**rottentomatoes**: &lt;title&gt; - gets ratings for &lt;title&gt; from Rotten Tomatoes

------
### shorten 
**isgd**: &lt;url&gt; [custom] - shortens a url using is.gd with [custom] as an optional custom shortlink,

    or unshortens &lt;url&gt; if already short

**shorten**: &lt;url&gt; [custom] - shortens a url with [custom] as an optional custom shortlink

**googl**: &lt;url&gt; [custom] - shorten &lt;url&gt; using goo.gl with [custom] as an option custom shortlink,

    or unshortens &lt;url&gt; if already short

**gitio**: &lt;url&gt; [custom] - shortens a github URL &lt;url&gt; using git.io with [custom] as an optional custom shortlink,

    or unshortens &lt;url&gt; if already short

**expand**: &lt;url&gt; - unshortens &lt;url&gt;

------
### spank 
**bdsm**: Just a little bit of kinky fun.

**spank**: &lt;user&gt; - Spanks a  &lt;user&gt;

------
### stock 
**stock**: &lt;symbol&gt; -- gets stock information

------
### suggest 
**suggest**: &lt;phrase&gt; - Gets suggested phrases for a google search

------
### system 
**system**: -- Retrieves information about the host system.

------
### tag 
**tag_del**: &lt;tag&gt; - delete a tag

**tag_add**: &lt;identifier content&gt; - add tag content as indentifier

**tag**: &lt;tag&gt; - Return a tag.

------
### thefuckingweather 
**tfw**: Retrieves weather and forecast data for a given location.



    Data is presented in a dict with three main elements: &quot;location&quot; (the

    location presented by TFW), &quot;current&quot; (current weather data) and &quot;forecast&quot;

    (a forecast of the next two days, with highs, lows, and what the weather

    will be like).



    &quot;current&quot; is a dictionary with three elements: &quot;temperature&quot; (an integer),

    &quot;weather&quot; (a list of descriptive elements about the weather, e.g., &quot;ITS

    FUCKING HOT&quot;, which may be coupled with something such as &quot;AND THUNDERING&quot;)

    and &quot;remark&quot; (a string printed by the server which is meant to be witty but

    is sometimes not. each to their own, I guess).



    &quot;forecast&quot; is a list of dictionaries, which each contain the keys &quot;day&quot; (a

    three-letter string consisting of the day of week), &quot;high&quot; and &quot;low&quot;

    (integers representing the relative extreme temperature of the day), and

    &quot;weather&quot; (a basic description of the weather, such as &quot;Scattered

    Thunderstorms&quot;).



    The default is for temperatures to be in Fahrenheit. If you&#x27;re so inclined,

    you can pass True as a second variable and get temperatures in Celsius.



    If you need a degree symbol, you can use thefuckingweather.DEGREE_SYMBOL.

------
### time_plugin 
**time**: &lt;location&gt; - Gets the current time in &lt;location&gt;.

**beats**: - Gets the current time in .beats (Swatch Internet Time).

------
### trump 
**trump**: trump a user.

------
### urban 
**urban**: urban &lt;phrase&gt; [id] -- Looks up &lt;phrase&gt; on urbandictionary.com.

------
### utility 
**escape**: &lt;string&gt; -- Unicode escapes &lt;string&gt;.

**debase64**: &lt;string&gt; -- Decode &lt;string&gt; with base64.

**lower**: &lt;string&gt; -- Convert string to lowercase.

**derpify**: &lt;text&gt; - returns some amusing responses from your input.

**base64**: &lt;string&gt; -- Encode &lt;string&gt; with base64.

**length**: &lt;string&gt; -- Gets the length of &lt;string&gt;

**leet**: &lt;text&gt; -- Makes &lt;text&gt; more 1337h4x0rz.

**unescape**: &lt;string&gt; -- Unicode unescapes &lt;string&gt;.

**titlecase**: &lt;string&gt; -- Convert string to title case.

**rot13**: &lt;string&gt; -- Encode &lt;string&gt; with rot13.

**upper**: &lt;string&gt; -- Convert string to uppercase.

**hash**: &lt;string&gt; -- Returns hashes of &lt;string&gt;.

**capitalize**: &lt;string&gt; -- Capitalizes &lt;string&gt;.

    :type text: str

**superscript**: &lt;text&gt; -- Makes &lt;text&gt; superscript.

**vapor**: &lt;string&gt; -- Converts &lt;string&gt; to full width characters.

**reverse**: &lt;string&gt; -- Reverses &lt;string&gt;.

**swapcase**: &lt;string&gt; -- Swaps the capitalization of &lt;string&gt;.

**qrcode**: &lt;link&gt; - returns a link to a QR code image for &lt;link&gt;

**isbase64**: &lt;string&gt; -- Checks if &lt;string&gt; is a valid base64 encoded string

------
### validate 
**w3c**: &lt;url&gt; - Runs url through the W3C Markup Validator.

------
### wandbox 
**wb**: wandbox interface

------
### watch 
**subwatch_add**: Add a subreddit to the watch list.

**subwatch_del**: Remove a subreddit from the watch list

**subwatch_list**: List watched subreddits.

**stopwatch**: Stop watching subreddits.

**startwatch**: Start watching subreddits.

**clear_rupdates_channel**: Remove reddit updates channel.

**get_rupdates_channel**: List reddit updates annoucement channel.

**set_rupdates_channel**: &lt;channel&gt; - Send reddit updates on channel.

------
### weather 
**weather**: &lt;location&gt; - Gets weather data for &lt;location&gt;.

------
### whois 
**whois**: &lt;domain&gt; - Does a whois query on &lt;domain&gt;.

------
### wikipedia 
**wiki**: &lt;phrase&gt; - Gets first sentence of Wikipedia article on &lt;phrase&gt;.

------
### xkcd 
**xkcd**: &lt;search term&gt; - Search for xkcd comic matching &lt;search term&gt;

------
### youtube 
**youtube**: &lt;query&gt; - Returns the first YouTube search result for &lt;query&gt;.

