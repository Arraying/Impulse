# Impulse Command Reference

Hey there! This is the official command reference for the Impulse Discord bot.
The names of the commands will be listed as a header without the prefix.
Examples will include a prefix, and a screenshot.

## about

This command shows basic information and statistics.

**Basic usage:** `i/about`

**Example:**

![Example](https://i.imgur.com/0d63AqJ.png)

## editplaylist

This command edits an existing playlist. 

**Removing a track from a playlist:** `i/editplaylist remove <playlist name> <track number>`

**Removing example:** 

![Example](https://i.imgur.com/QzRAWjM.png)

**Swapping tracks in a playlist:** `i/editplaylist swap <playlist name> <track 1> <track 2>`

**Swapping example:**

![Example](https://i.imgur.com/NnrSxCQ.png)

## grab

This command takes the current track and adds it to the beginning of the specified playlist.

**Basic usage:** `i/grab <playlist name>`

**Example:**

![Example](https://i.imgur.com/fjsEe7w.png)

## guide

This command shows a really simple quick start guide for the bot.

**Basic usage:** `i/guide`

**Example:**

![Example](https://i.imgur.com/59G2wfd.png)

## help

This command shows both a list of commands, and information on a specific command.

**Listing commands:** `i/help`

**Listing commands example:**

![Example](https://i.imgur.com/EizPAuY.png)

**Listing commands with page number:** `i/help <page number>`

**Listing commands with page number example:**

![Example](https://i.imgur.com/lGasjIc.png)

**Showing command information:** `i/help <command name, without prefix>`

**Command information example:**

![Example](https://i.imgur.com/lDMmZtv.png)

## invite

This command DMs the user Impulse's invite links.

**Basic usage:** `i/invite`

**Example**

![Example](https://i.imgur.com/yg8ofpl.png)

![Example](https://i.imgur.com/sFvgul5.png)

## loop

This command toggles queue looping. When queue looping is enabled, songs will be appended to the end of the queue after they finish playing.
To disable looping, simply execute the command again.

**Basic usage:** `i/loop`

**Example:**

![Example](https://i.imgur.com/snZEk6K.png)

## nowplaying

This command shows information on the song that is currently playing.

**Basic usage:** `i/nowplaying`.

**Example:**

![Example](https://i.imgur.com/DAxXxbH.png)

## pause

This command acts as a pause/unpause button for a song. To pause a song, execute the command. 
To un-pause the song, execute the command again.

**Basic usage:** `i/pause`

**Example:**

![Example](https://i.imgur.com/PrwPXEP.png)

## ping

This command shows the latency of the current shard and average latency of the process/instance. 

**Basic usage:** `i/ping`

**Example:**

![Example](https://i.imgur.com/nRKPKYU.png)

## play

This command plays music. When there is no music playing, it will start playing. Otherwise it will add the track to the song queue.
Streams are also supported.
The command comes in three varieties: 
* Playing via URL
* Searching on YouTube
* Searching on SoundCloud

For more information on what the URL feature supports click [this](https://github.com/sedmelluq/lavaplayer#supported-formats).

**Playing via URL.** `i/play <url>`

**URL example:**

![Example](https://i.imgur.com/4dM31UV.png)

It is also possible to search for a song on YouTube. You will then be given a list of songs with track numbers. 
To select the song type the track number in chat. To cancel the selection, type "cancel".
If no valid track number was inputted within 30 seconds of executing the play command then the command will time out.

**Searching on YouTube:** `i/play <song name>`

**YouTube search example:** 

![Example](https://i.imgur.com/y3l2T37.png)

Searching on SoundCloud is nearly identical to searching on YouTube. 
The only difference is that you need to specify the `--soundcloud` explicitly to tell the bot to search on SoundCloud.

**Searching on SoundCloud:** `i/play <song name> --soundcloud`

**SoundCloud search example:**

![Example](https://i.imgur.com/0WffGTR.png)

It is also important to note that you can specify the queue position of the song using the `--position` flag, whatever command variety you choose.

**Specifying a position:** `i/play nightcore smells like teen spirit --position <position>

## playlists

This command manages global & user created playlists. At this current point in time it is only possible to own one playlist.

**Creating a playlist:** `i/playlists add <playlist name>`

**Playlist creation example:**

![Example](https://i.imgur.com/8xdG6Q4.png)

**Deleting a playlist:** `i/playlists delete <playlist name>`

**Playlist deletion example:**

![Example](https://i.imgur.com/YF01Aja.png)

**Showing all playlists:** `i/playlists list`

**Playlist list example:**

![Example](https://i.imgur.com/yssaElO.png)

## playplaylist

This command enqueues the contents of a playlist.

**Basic usage:** `i/playplaylist <playlist name>`

**Basic example:**

![Example](https://i.imgur.com/02wqKSh.png)

It is also possible to only enqueue a range of songs from the playlist.
This can be done using the `--first` and `--last` flags.
Both of these flags are optional, and do not need to be provided together.

**Enqueue playlist range:** `i/playplaylist <playlist name> --first <first track number> --last <last track number>`

**Playlist range example:**

![Example](https://i.imgur.com/UKfaJUj.png)

## prefix

This command shows and sets the per-server prefix.

**Showing the prefix:** `i/prefix`

**Prefix showing example:**

![Example](https://i.imgur.com/fB5iUFS.png)

When setting the prefix, the bot only uses the first argument.
Therefore, spaces will not work as intended.
To use a space in the prefix, use `{space}` as a placeholder.

**Setting the prefix:** `i/prefix <prefix>`

**Prefix setting example:** 

![Example](https://i.imgur.com/JQDJY4F.png)

## queue

This command shows and manages the track queue.

**Showing the queue:** `i/queue`

**Queue showing example:**

![Example](https://i.imgur.com/FDeGcyN.png)

**Showing another queue page:** `i/queue <page number>`

**Shuffling the queue:** `i/queue shuffle`

**Queue shuffling example:**

![Example](https://i.imgur.com/28BMyqt.png)

**Removing a track from the queue:** `i/queue remove <track number>`

**Track removal example:**

![Example](https://i.imgur.com/HKzjIA5.png)

**Moving tracks in the queue:** `i/queue move <track position> <other position>`

**Track moving example:**

![Example](https://i.imgur.com/p24LKmS.png)

## showplaylist

This command shows all the tracks in the playlist.

**Showing tracks usage:** `i/showplaylist <playlist name>`

**Track showing example:**

![Example](https://i.imgur.com/lGS62PN.png)

** Showing another page:** `i/showplaylist <playlist name> <page number>`

## skip

This command skips the current song and plays the next song in the queue (if there is any).

**Basic usage:** `i/skip`

**Example:**

![Example](https://i.imgur.com/CvoELah.png)

## stop

This command stops playback.

**Basic usage:** `i/stop`

**Example:**

![Example](https://i.imgur.com/5XRT00y.png)

## theme

This command changes the theme of the bot.
By default, Impulse will have a no-embed code-block theme. 
It is possible to give the bot a cleaner look with other themes.

**List all themes:** `i/theme`

**Theme list example:**

![Example](https://i.imgur.com/lWXKIx7.png)

**Changing the theme:** `i/theme <theme name>`

**Theme change example:** 

![Example](https://i.imgur.com/iWqJ67F.png)

## volume

This command changes or resets the audio playback volume.

**Resetting the volume:** `i/volume`

**Volume reset example:**

![Example](https://i.imgur.com/zqgEdHs.png)

**Changing the volume:** `i/volume <volume>`

**Volume change example:**

![Example](https://i.imgur.com/9Um2jNW.png)



