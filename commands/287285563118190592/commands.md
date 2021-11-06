Bot commands:
------
### attacks 
**compliment**: <user> -- Makes the bot compliment <user>.

**gift**: <user> - gives gift to <user>

**insult**: <user> - insults <user>

**kill**: <user> - kills <user>

**lart**: <user> - LARTs <user>

**nk**: outputs a random North Korea propoganda slogan

**sexup**: <user> - flirts with <user>

**slap**: <user> -- Makes the bot slap <user>.

**strax**: Strax quote.

------
### avatar 
**avatar**: <user or user-id> - Get someones avatar

**e**: Expand an emoji

**get_server_banner**: Return a link to the server banner

------
### bible 
**bible**: <passage> - Prints the specified passage from the Bible

------
### bot_admin_system 
**about**: Get about.

**invite_me**: Get invitation for bot

**system**: -- Retrieves information about the host system.

------
### brainfuck 
**brainfuck**: <prog> - executes <prog> as Brainfuck code

    :type text: str

------
### cats 
**catgifs**: - gets a fucking cat gif.

**cats**: - gets a fucking fact about cats.

------
### cb 
**coa**: <text> - talk to CleverBot

------
### cheer 
**cheer**: :type chan: str

------
### corona 
**corona**: <option> - available options: [all, <country name>]. If option is <country name>, you must specify a country from <https://worldometers.info/coronavirus#countries>.

**corona_format**: <format> - formats the .corona command for you. Every keyword in ['Cases', 'Deaths', 'Tests', 'CToday', 'DToday', 'C/M', 'D/M', 'T/M', 'Recovered', 'Active', 'Critical', 'Country', 'Continent', 'Vaccines', 'LUpdated'] will be replaced with the appropriate data. Use `clear` if you want to clear your format and use the default one

------
### correction 
**s**: <word replacement> - replace 'word' with replacement

**ss**: <regex replacement> - replace regex with replacement

**toggle_correction_msg_del**: enable/disable automatic deletion of command when running .s/.ss

------
### crypto 
**btc**: - Returns the current btc value

**crypto**: <ticker> [currency] - Returns current value of a cryptocurrency

**eth**: - Returns the current eth value

**ltc**: - Returns the current ltc value

**serak**: No description provided.

------
### cypher 
**cypher**: <pass> <string> -- cyphers <string> with <password>

**decypher**: <pass> <string> - decyphers <string> with <password>

------
### dogpile 
**g**: <query> - Search for a link.

**gis**: <query> - Search for a image.

**nsfwgis**: <query> - Search for a image.

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
**fix**: <text> - fixes a flipped over table. ┬─┬ノ(ಠ_ಠノ)

**flip_text**: <text> - Flips <text> over.

**table**: <text> - (╯°□°）╯︵ <ʇxǝʇ>

------
### gaming 
**choose**: <choice1>, [choice2], [choice3], etc. - randomly picks one of the given choices

    :type text: str

**coin**: [amount] - flips [amount] coins

    :type text: str

**dice**: <dice roll> - simulates dice rolls. Example: 'dice 2d20-d5+4 roll 2': D20s, subtract 1D5, add 4

    :type text: str

------
### giphy 
**gif**: <query> - Searches giphy.com for a gif using the provided search term.

------
### github 
**ghissue**: <username|repo> [number] - gets issue [number]'s summary, or the open issue count if no issue is specified

------
### grab 
**grab**: <user> - grab user's last message. If <user> is empty, it will try to grab the message you're replying to

**grabl**: <user> - List quotes for user. If no user is specified, it lists everything on the server.

**grabr**: Grab random quote

**grabs**: <expression> - Search for 'expression' in grab texts.

**grabu**: <user> - Grab random quote from user

------
### help 
**help**: Get help for a command or the help document

------
### image_generator 
**amateur**: No description provided.

**anal**: No description provided.

**asians**: No description provided.

**aww**: No description provided.

**blep**: No description provided.

**blonde**: No description provided.

**buci**: No description provided.

**capre**: No description provided.

**craci**: No description provided.

**cutu**: No description provided.

**femboy**: No description provided.

**fetch_image**: No description provided.

**fetish**: No description provided.

**lesbiene**: No description provided.

**milf**: No description provided.

**nsfwfunny**: No description provided.

**pisi**: No description provided.

**plsgayporn**: No description provided.

**plsporn**: No description provided.

**raton**: No description provided.

**roscate**: No description provided.

**skinny**: No description provided.

**sloboz**: No description provided.

**tatuate**: No description provided.

**teen**: No description provided.

**thicc**: No description provided.

**thot**: No description provided.

**traps**: No description provided.

**tzatze**: No description provided.

------
### imdb 
**imdb**: <movie> - gets information about <movie> from IMDb

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
### irc_mode 
**accept_invite**: No description provided.

**add_op**: <name> - Add an operator

**advertise**: <channel [description]> - advertise a channel by optionally specifying a channel description

**ban_member**: <name/ID> - ban a member

**get_associated_role**: Get the role name associated to the channel

**iclear**: Clear a channel property.

**iget**: Get a channel property.

**ilist**: List properties.

**invite_member**: <user> Invite someone to an invite-only channel

**irc_help**: No description provided.

**iset**: Set a channel property.

**join**: <chname> - join a channel

**kick_member**: <name/ID> - kick a member

**list_bans**: List channel bans

**list_members**: List members

**list_ops**: List operators

**make_nsfw**: <topic> - make channel NSFW

**make_permission_based**: Instead of managing access through roles, it uses channel permissions

**make_role_based**: Instead of managing access through permissions, it uses role access

**make_sfw**: <topic> - make channel SFW

**part**: <chname> - leave a channel

**remove_op**: <name> - Remove an operator

**request_channel**: <name> - request a channel by specifying a name

**set_associated_role_name**: Set the role name associated to the channel

**set_topic**: <topic> - set channel topic

**unban_member**: <name/ID> - unban a member

------
### jokes 
**awesome**: - Prints a webpage to show <nick> how awesome they are.

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
### lurve 
**lurve**: lurves all over <user>

------
### magik 
**gmagik**: No description provided.

**magik**: No description provided.

------
### markov 
**markov**: <user channel> - Generate sentence using a markov chain for a user using data from the given channel.

    If no user is specified, a sentence will be generated using all user messages.

------
### name_generator 
**namegen**: [generator|list] - generates some names using the chosen generator, or lists all generators if 'list' is specified

    :type bot: cloudbot.bot.CloudBot

------
### qalc 
**calc**: <expression> - qalc interface

------
### quran 
**quran**: <verse> - Prints the specified Qur'anic verse(s) and its/their translation(s)

------
### remind 
**remind**: <period message> - ask the bot to remind you about something in given period (e.g. '.remind 1h bleh bleh' sends you 'bleh bleh' in one hour

------
### roddit_admin 
**votat**: No description provided.

------
### roddit_curs 
**curs**: <currency> - Returns current value of a currency in RON

------
### roddit_dex 
**dex**: <cuvant> - Cauta definitia pentru un cuvant in DEX

------
### roddit_family 
**accept_adoption**: <id> - Acceptă o ofertă de adopție

**accept_marry**: <id> - Acceptă o ofertă de căsătorie.

**adopt**: <user> - Inițiază o cerere de adopție cu user-ul menționat

**bug_report**: <text> - raportează un bug către cel care se ocupă cu această funcționalitate a botului.

**choose_parent**: <părinte> - Alege părintele cu care vrei să rămâi după divorț.

**deny_adoption**: <id> - Refuză o ofertă de adopție

**deny_marry**: <id> - Refuză o ofertă de căsătorie

**disown**: <user> - Dezmoștenește unul din copii

**divorce**: Divorțează cu partenerul tău.

**family_info**: Informații generale despre comenzile legate de familie

**family_support**: Afișează toate comenzile pe care le poate face cineva. Lista se poate schimba după mulți factori. `.family_support full` dezactivează dinamicitatea

**family_tree**: <user> - Afișează arborele genealogic al unei persoane. Dacă nu este menționat cineva, va afișa arborele tău genealogic

**leave_parents**: Nu alege niciun părinte cu care să rămâi. Nu vei mai putea alege un părinte după.

**marry**: <user> - Inițiază o cerere în căsătorie cu persoana menționată

**offer_inbox**: Afișează toate cererile disponibile pe care le-ai primit.

**offer_outbox**: Afișează toate cererile disponibile pe care le-ai trimis.

**revoke_adopt_request**: Dacă te-ai răzgândit și nu vrei să adoptezi pe cineva.

**revoke_marry_request**: Dacă te-ai răzgândit și nu vrei să te căsătorești.

**run_away**: Fugi de acasă. Sunt eliminate toate legăturile cu părinții tăi.

------
### roddit_fun 
**aplauze**: No description provided.

**aram**: No description provided.

**ayy**: No description provided.

**bitter**: No description provided.

**bluntlee**: No description provided.

**brutalistu**: No description provided.

**cacat**: No description provided.

**cancel**: No description provided.

**cola**: No description provided.

**dance**: No description provided.

**iazo**: No description provided.

**injur**: No description provided.

**iubestemafa**: Vezi compatiblitatea ta cu o persoana. Sau o chestie.

**jupi**: No description provided.

**manea**: No description provided.

**mcioran**: No description provided.

**mpuric**: No description provided.

**mtutea**: No description provided.

**muie**: No description provided.

**murmuz**: No description provided.

**puti**: No description provided.

**shrug**: No description provided.

**vasile**: No description provided.

------
### roddit_horoscop 
**horoscop**: horoscop <zodie> - Afișează horoscopul unei zodii

------
### roddit_irc_mode_selectors 
**vreau_canal**: Generate channel selector

**vreau_toate_canalele**: Generate server-wide channel selector.

------
### roddit_roles 
**vreau_culoare**: Culori

**vreau_eveniment**: Roluri pentru evenimente

**vreau_joc**: Roluri pentru jocuri

**vreau_rol**: Roluri random

------
### role_selector 
**list_selectors**: list selector commands

------
### shorten 
**expand**: <url> - unshortens <url>

**isgd**: <url> [custom] - shortens a url using is.gd with [custom] as an optional custom shortlink,

    or unshortens <url> if already short

**shorten**: <url> [custom] - shortens a url with [custom] as an optional custom shortlink

------
### spank 
**bdsm**: Just a little bit of kinky fun.

**spank**: <user> - Spanks a  <user>

------
### stock 
**dquote**: No description provided.

**quote**: No description provided.

**stock**: No description provided.

------
### suggest 
**suggest**: <phrase> - Gets suggested phrases for a google search

------
### tag 
**tag**: <tag> - Return a tag. '.tag list' lists tags, '.tag random' returns random tag

**tag_add**: <identifier content> - add tag content as indentifier

------
### text 
**letters**: <text> - text to emoji letters

------
### time_plugin 
**beats**: - Gets the current time in .beats (Swatch Internet Time).

**time**: <location> - Gets the current time in <location>.

------
### txt2img 
**txt2img**: Generate a image using sent text

    "<option> - available input for custom fonts:

    .image <font name>-<size>-<text color>-<bg color>

    VALID_FONTS=

    'sofia',

    'ostirch',

    'diso',

    'learning',

    'hotel',

    'plp',

    'default'

    'symbols'

    Example usage of this command :

    .text2img sofia-30-red-yellow the quick brown fox jumps over the lazy dog

------
### urban 
**urban**: urban <phrase> [id] -- Looks up <phrase> on urbandictionary.com.

------
### userinfo 
**inrole**: [role name] List how many members each role has. Calling it with no role name will list all roles

**userinfo**: <mention> - gets various data about the mentioned user

------
### utility 
**base64**: <string> -- Encode <string> with base64.

**capitalize**: <string> -- Capitalizes <string>.

    :type text: str

**debase64**: <string> -- Decode <string> with base64.

**derpify**: <text> - returns some amusing responses from your input.

**escape**: <string> -- Unicode escapes <string>.

**hash**: <string> -- Returns hashes of <string>.

**isbase64**: <string> -- Checks if <string> is a valid base64 encoded string

**leet**: <text> -- Makes <text> more 1337h4x0rz.

**length**: <string> -- Gets the length of <string>

**lower**: <string> -- Convert string to lowercase.

**qrcode**: <link> - returns a link to a QR code image for <link>

**reverse**: <string> -- Reverses <string>.

**rot13**: <string> -- Encode <string> with rot13.

**superscript**: <text> -- Makes <text> superscript.

**swapcase**: <string> -- Swaps the capitalization of <string>.

**titlecase**: <string> -- Convert string to title case.

**unescape**: <string> -- Unicode unescapes <string>.

**upper**: <string> -- Convert string to uppercase.

**vapor**: <string> -- Converts <string> to full width characters.

------
### uwu 
**uwu**: <text> - translate text to UwU

------
### vicky 
**vicky**: <hot> <crazy> - Returns the zone from the universal hot crazy matrix

------
### wandbox 
**wb**: wandbox interface

------
### watcher 
**subwatch_list**: List watched subreddits.

------
### weather 
**weather**: <location> - Gets weather data for <location>.

------
### whois 
**whois**: <domain> - Does a whois query on <domain>.

------
### youtube 
**youtube**: <query> - Returns the first YouTube search result for <query>.

