# What is MP-TVSeries #

MP-TVSeries is a popular TV Series plug-in for MediaPortal, an open-source media center application. It focuses on managing the user's TV Series library with minimal user interaction, allowing for a more user friendly and ease of use experience.

The MP-TVSeries plugin will scan your hard drive (including network and removable drives) for video files, it then analyzes them by their path structures to determine if they are TV Shows. If the file(s) are recognized then the plugin will go online to thetvdb.com and retrieve information about them. You can then browse, manage and play your episodes from inside MediaPortal in a nice graphical layout.

This Plugin does not play Live TV

# MPTVSeries Window ID #
  * 9811

# Questions, Suggestions & Bug Reports #

There are 3 ways you can receive support for the plugin, Submitting log files and or Screenshots is recommended

> ## Mediaportal Forum ##
> MP-TVSeries has a dedicated [sub-forum](http://forum.team-mediaportal.com/my-tvseries-162/), try searching as you question may have been answered, if not please create a new thread

> ## Issue Tracker ##
> MP-TVSeries has a issue tracker [here](http://code.google.com/p/mptvseries/issues/list). Recommended if you have a re-producible bug or enhancement request

> ## IRC ##
> Join the #mp-tvseries IRC channel on Freenode

> ## Submitting Useful Log Files ##
> If you require assitance its smart to include the log files with your post,  you will likely find the community will more often look at your issue if you provide all the necessary information. Instructions are below.

  * Launch **MediaPortal Debug-Mode** shortcut from your Windows Start Menu (Team MediaPortal/MediaPortal)
  * Select the second option _Report a bug to a Plugin Developer or a Skin Designer_
> > ![http://mptvseries.googlecode.com/svn/wiki/Images/DebugMode.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/DebugMode.jpg)
  * Click _Proceed_, (Mediaportal will now automatically run)
  * **Reproduce the issue** in MP-TVSeries, do what is needed to show the problem, reproduce the issue only
  * Close MediaPortal
  * A **MediaPortalLogs\_Date\_Time.zip** file will be automatically created on your desktop. Attach this file to your thread/post


---


# Integration with Social Media Websites #

MP-TVSeries optionally integrates with the [follw.it](http://follw.it) and [trakt.tv](http://trakt.tv) and [myshows.ru](http://myshows.ru) websites, which are built around sharing with your friends what shows and movies you are into.

One of the advantages to connecting to one or all of the sites is the syncronisation of your watch flags and ratings, which we recommend. This is very useful if you have multiple htpcs, or if you need to start your tv series database from scratch.

You can use any or all of the sites at the same time.

## Follw.it ##

  * From version 2.8.0+, you can configure follw.it from within the Plugin Configuration for MP-TVSeries


> ### Configuration ###

  * Load MP-TVSeries from Mediaportal Configuration, Plugins.
  * Click _Follw.it Tab_
  * Click _Setup Account_
  * Follow the OnScreen instructions
> ![http://mptvseries.googlecode.com/svn/wiki/Images/FollwitConfig.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/FollwitConfig.jpg)


## Trakt.tv ##

  * From version 2.8.1+, the Trakt.tv support will be moved to its own plugin called [Trakt for Mediaportal](http://trakt.tv/downloads/mediaportal). This plugin will be included with the MP-TVSeries installer should you wish to install it or you can download MPEI package at any time.

> ### Configuration After Install ###

  * Load Mediaportal Configuration, Plugins.
  * Load _Trakt_ which is under 'Windows Plugins'
  * Type in your trakt.tv username and password
  * Check the box for MP-TVSeries and any optional plugin
  * Click OK
> ![http://mptvseries.googlecode.com/svn/wiki/Images/TraktConfig.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/TraktConfig.jpg)

## myshows.ru ##

> For Russian MP users [myshows.ru](http://www.myshows.ru) is supported. Now it is possible to mark episodes as watched automatically after playback and toggle watched status manually from Mediaportal.

> ### Installation ###

> [Download](http://code.google.com/p/mptvseries/issues/detail?id=578) Myshows Plugin.dll and copy it into \Team MediaPortal\MediaPortal\plugins\process

> ### Configuration ###

  * Load 'MyShowsPlugin' from Mediaportal Configuration, Plugins.
  * Enter your myshows.ru login and password
  * Click "Test Login" to verify your credentials
  * Click "OK"
  * Click "OK" in Mediaportal Configuration to save settings.
![http://mptvseries.googlecode.com/svn/wiki/Images/MyShowsConfig.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/MyShowsConfig.jpg)


---


# File Naming Conventions #
MP-TVSeries supports various naming conventions, if you want a perfect match without any user interaction, its best to name the Series as it is shown on thetvdb.com. If the Show contains a : such as CSI: Miami you could use CSI Miami or CSI- Miami

> ## Examples Of Supported Filenames ##
Here are a few random examples which will parse.
  * Alias.S01E01.avi
  * Alias - S01E01 - Pilot.avi
  * Alias.1x1.avi
  * Alias - 1x1 - Pilot.avi
  * Alias 01x01.mkv

> ## Series with Specials ##
Specials need to be labeled as Season 0, Lets take Top Gear Polar Special for example, Find Top Gear on thetvdb and click on [Specials](http://www.thetvdb.com/?tab=season&seriesid=74608&seasonid=22070&lid=7). We can see in the Specials list, its labeled as Episode 49, so a filename for that could be
  * Top Gear - S00E49 - Polar Special.avi
  * Top Gear - 0x49.mkv

> ## Original Series And Remakes ##
If you have a series which has been rebooted, lets take Battlestar Galatica for example, there is the Original, a 1980's version and a 2003 version, How do you name these? go to [thetvdb.com](http://www.thetvdb.com), search Battlestar Galatica. We need to name our files the same way. note each series has a different show id comfirming they are all different series
> ![http://mptvseries.googlecode.com/svn/wiki/Images/TvdbBSGExample.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/TvdbBSGExample.jpg)

  * Battlestar Galactica  - S01E01.avi  (match as original series)
  * Battlestar Galactica (1980) - S01E01.avi  (match as 1980's series)
  * Battlestar Galactica (2003) - S01E01.avi  (match as 2003 series)

If a series was already imported incorrectly in Mediaportal, highlight the series, press F9 or Info on remote, then press 'Force new online lookup for series'.
This will prompt you to select a series or manually enter a search term.

> ## Mini-Series ##
A standalone Mini Series, like Dune, will usually have the part 1, part 2 etc listed at Season 1, Episode 1, Episode 2 etc on thetvdb. If for example, the Mini Series lead to a TV Show, such as BattleStar Galactica (2003) that Mini Series may be listed in Specials / Season 0.

The Solution is to check the Mini-Series on [thetvdb.com](http://thetvdb.com), match your files names to their syntax. Examples:

  * Frank Herbert's Dune - S01E01.avi
  * Frank Herbert's Dune - S01E02.avi
  * Frank Herbert's Dune - S01E03.avi
  * Battlestar Galactica (2003) - S00E01 - MiniSeries(1).avi
  * Battlestar Galactica (2003) - S00E02 - MiniSeries(2).avi

> ## Single File - Double Episode ##
MP-TVSeries can support 2 episodes in a single file. More than 2 is not currently supported

See examples below

  * Alias.1x01.1x02.avi
  * Alias S01E01-E02.avi
  * Alias S01E01 + S01E02.avi
  * Alias - s01e01 - s01e02.mkv
  * Alias #1.01 + #1.02.avi

If you start playback on 1x01 from "Alias - S01E01-E02.avi", then both episodes will be played, the end result is both episode 1 and 2 will be marked as watched. You can still start playback on 1x02, but it will start at the beginning of the file (but this is what one would expect anyway). If you start 1x01, but stop at the halfway point where 1x02 begins, then both 1x01+02 show as unwatched and when you try to restart playback you will get the "resume from" dialog

> ## Single Episode - Multiple Files ##
MP-TVSeries is does not currently support combining multiple files into a single episode, It will show those files as duplicates in the episode list

We recommend in this scenario to join the files together, Click the following links for example programs for [AVI files](http://www.alexander-noe.com/video/amg/) and [MKV files](http://www.bunkus.org/videotools/mkvtoolnix/)

> ## Episodes with Air Date ##
MP-TVSeries now supports AirDate parsing, matched up from episodes listed at theTVDB.com
Some examples below are episodes which will now parse by default - Note: requires atleast v2.9.3 for MP 1.1 or v3.0.5 for MP 1.2B

  * Conan.(2010).2010.11.08.Baa.Baa.Blackmail.mkv
  * Conan.(2010).2011.07.20.Hell.Hath.No.Cell.Phone.Reception.mkv
  * The.Colbert.Report.2011.07.27.Dr.Missy.Cummings.mkv

> ## Auto Renaming of Files ##
MP-TVSeries does not currently support the auto renaming of your files. However their are free 3rd party tools such as [TheRenamer](http://www.theRenamer.com), [Tv Rename](http://www.tvrename.com), [Media Centre Master ](http://www.mediacentermaster.com/) and [Filebot](http://filebot.sourceforge.net/) which you could use to organise/rename the files in your collection.

> ## Folder Structure ##
There are many variations you could use, below is a way that works well with the renaming tools above.
  * TV  --> Series Name  --> Season # ---> 30 Rock - S01E01 - Pilot.avi
> ![http://mptvseries.googlecode.com/svn/wiki/Images/FolderStructureExample.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/FolderStructureExample.jpg)



---


# Episode Ordering - Online Matching #
MP-TVSeries has options to change the episode ordering for a series, you will only see options available if its applicable to that series

> ## Air Date ##
> This is the default option, shows will be ordered by the date they were aired

> ## DVD Order ##
> Choose this option to have your episodes listed in the order they were released on DVD, DVD ordering if often used to correct minor, sometimes major changes in episode ordering that was initially aired on TV

> ## Title ##
> This matches episode by title.  Example. firefly - 1x01 - Serenity.mkv In this case will be parsed as 'Serenity' and will attempt to find an online match with episodes that have that title.
> This may be useful for specials which keep on getting re-ordered online.

> ## Absolute Order ##
> This option can only be selected on a Series, not a Season. Some series, like Anime may not be broken in Seasons. In order to accommodate this Absolute Order can be used

> ## Changing Matching Method ##
> You can initially select these options on your [inital import](http://code.google.com/p/mptvseries/wiki/GettingStarted?ts=1301693772&updated=GettingStarted#Initial_Configuration),or you can change it inside Mediaportal
  * In Mediaportal - Select the Series or Season
  * Press F9 on keyboard or INFO on MCE Remote
  * Choose ACTIONS
  * Choose CHANGE ONLINE MATCHING METHOD


---


# Download Episode Information for Whole Series #
To download all the available information for your Series, including Episodes you may not have, Episodes that have not aired yet, and display these episodes inside Mediaportal, do either or the following to enable. note: all episode info will be downloaded next import run.

> ## Option 1: Enable in Configuration ##
  * Load MP-TVSeries Plugin Configuration
  * OnlineData Tab
  * Check the box _'Download Episode Information for the whole Series'_
  * The next import may take a while as it downloads all the available information for all your imported Series
> ![http://mptvseries.googlecode.com/svn/wiki/Images/DownloadEpisodeInfoAll.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/DownloadEpisodeInfoAll.jpg)

> ## Option 2: Enable in Mediaportal ##
  * in Mediaporal, MP-TVSeries Plugin
  * Press F9 on keyboard or INFO on MCE Remote
  * Click OPTIONS
  * Change 'DOWNLOAD ALL EPISODE INFO' to ON

> ## Show / Hide ##
  * in Mediaporal, MP-TVSeries Plugin
  * Press F9 on keyboard or INFO on MCE Remote
  * Click OPTIONS
  * Change 'SHOW ALL EPISODES' to ON

> You will now see all episodes for a Series, Depending on Skin, those episodes may show in a different colour, e.g. Orange in Blue3Wide & StreamedMP. If a Season only shows a partial amount of all the expected episodes, then those episodes havent been added yet on thetvdb.com.


---

# Importing #

> ## Imported Episode Image is Incorrect ##
> If you find a episode which has a incorrect episode image, it may be been incorrectly uploaded at thetvdb. When the image is replaced with a correct version, MP-TVSeries will not automatically download this, however you can do this manually

> Note: MP-TVSeries v2.7+ will show a FanArt episode image if there is no episode image available, which will be updated automatically, and not to be confused with an Incorrect Episode Image

  * In Mediaportal, Select the Episode
  * Press F9 on keyboard, or INFO on MCE remote
  * Click ACTIONS
  * Click UPDATE

> ## Importing Videos Not At TheTVDB ##
> MP-TVSeries is not intended for this scenario, but there is a solution you can use. If you have videos that you want to show in MP-TVSeries, and its not appropriate to create it at thetvdb.com, such as personal movies recorded on video cameras etc, you can try the following - Recommend MP-TVSeries v2.9+

  * Create proper filenames with season and episode syntax e.g.
    * My Trip to Fiji - S01E01.avi
    * My Trip to Fiji - S01E02.avi
    * My Trip to Fiji - S01E03.avi
    * My Trip to Fiji - S01E04.avi

  * Load Media Portal Configuration, MP-TVSeries plugin.
  * Start the Import Wizard, and select Skip when no match is found for the 'My Trip to Fiji'
  * Finish Import
  * Select 'Details' tab.
  * Find your Series, Enter Series and Episode info (This will create USEREDIT fields in database)
  * Right Click on series and select 'Ignore on Scan' so we dont prompt to match series everytime an import is run.
  * Enter GUI and select series, then play!

> By default MP-TVSeries will automatically generate episode titles if they dont exist online e.g Episode 1, Episode 2 etc. If this behaviour is not wanted you can manually edit the Options Table in the database and set **AutoGenerateEpisodeTitles** to Zero. This change will only take affect for **NEW** episodes added to database, if you want to respect episode titles from filenames for existing files that have been import then you need to clear the database and re-import.


---


# Custom Artwork #
Typically if you are importing videos not available on theTVDB.com such as sports videos, then you will most likely want to add some artwork. Follow these instructions to get custom artwork in tvseries:

  * In your thumbs\MPTVSeriesBanners\ folder create the **Show Name** if it doesnt already exist (this should match your series name, replace invalid filename characters with underscore) and then create the following directory structure:
> > ![http://mptvseries.googlecode.com/svn/wiki/Images/FAQ/CustomArtworkExplorerFolderStructure.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/FAQ/CustomArtworkExplorerFolderStructure.jpg)
  * In the **episodes** folder create artwork in the following format: custom-{seasonindex}x{episodeindex}.jpg e.g. **custom-2001x1.jpg**
  * In the **seasons** folder create artwork in the following format: custom-{seasonindex}.jpg e.g **custom-2011.jpg**
  * In the **widebanner** and **posters** folders create artwork in the following format: **custom.jpg**
  * For **fanart**, you must first find the **Online Series ID** which is located in the configuration details tab for the selected series. This is typically a negative number e.g. **-70**. Now simply drop a fanart file into your fanart directory e.g. **thumbs\Fan Art\fanart\original\-70.jpg**

Now in Configuration, select the series and pick the **custom** artwork from the drop down list.

> ![http://mptvseries.googlecode.com/svn/wiki/Images/FAQ/ConfigSeriesArtwork.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/FAQ/ConfigSeriesArtwork.jpg)

---


# Subtitle Support #
Newer versions of MP-TVSeries will now be supporting the [SubCentral](http://forum.team-mediaportal.com/showthread.php?t=85545&referrerid=104898) Plugin, 'Subtitle Downloader' will be retired, as it will no longer be maintained.

> ## Installation ##
  * [Download](http://www.team-mediaportal.com/extensions/movies-videos/subcentral) the SubCentral Plugin
  * Check SubCentral Plugin is enabled in MP Configuration, Plugins
  * in MP-TVSeries Configuration, Click General tab
  * (Optional) Tick “Offer to download subtitles before playing (SubCentral)” if you want to perform an automatic subtitle search before playing an episode that does not have any subtitles.

> ## Download a Subtitle ##
  * In the Episode list, highlight the episode you want to download a subtitle
  * Press F9 on keyboard or INFO on MCE Remote
  * Select 'SUBTITLES...'
  * Find Select and Download the required Subtitle
  * Return to the TV Series Plugin

> ## Turn on Subtitles ##
  * Play An Episode
  * Press 'Y' on keyboard or press INFO on MCE remote, select Subtitles
  * Choose the language of subitle if available
  * Highlight 'ENABLED' and press OK
  * Return to episode, press Back on MCE Remote or ESC on keyboard
  * TIP: Press Yellow on MCE remote to toggle subtitles on / off


---


# MP-TVSeries File Locations #
The following are the locations of the files and folders used by MP-TVSeries, should you need to backup / restore or just have a look around

> ## MP-TVSeries.dll ##
> This is the plugin itself which is used by Mediaportal, located in
| x86 | C:\Program Files \Team MediaPortal\MediaPortal\plugins\Windows |
|:----|:---------------------------------------------------------------|
| x64 | C:\Program Files (x86)\Team MediaPortal\MediaPortal\plugins\Windows |

> ## TVSeriesDatabase4.db3 ##
> This is the database file, where your MP-TVSeries data is stored. its recommended to backup this file incase you experience database corruption.
| XP |  C:\Documents and Settings\All Users\Application Data\Team MediaPortal\MediaPortal\database |
|:---|:--------------------------------------------------------------------------------------------|
| Vista & Win7 |  C:\ProgramData\Team MediaPortal\MediaPortal\database                                       |

> ## MPTVSeriesBanners and Fan Art (Folders) ##
> These two folders inside the thumbs folder are where the artwork is stored.
| XP |  C:\Documents and Settings\All Users\Application Data\Team MediaPortal\MediaPortal\thumbs |
|:---|:------------------------------------------------------------------------------------------|
| Vista & Win7 |  C:\ProgramData\Team MediaPortal\MediaPortal\thumbs                                       |

> ## MP-TVSeries.log ##
> This file contains a log of activities in the MP-TVSeries plugin, which is useful for diagnostic purposes
| XP |  C:\Documents and Settings\All Users\Application Data\Team MediaPortal\MediaPortal\log |
|:---|:---------------------------------------------------------------------------------------|
| Vista & Win7 |  C:\ProgramData\Team MediaPortal\MediaPortal\log                                       |

> ## Language.XML (Files) ##
> This directory contains all the language files, in XML format that can be used in MP-TVSeries
| XP |  C:\Documents and Settings\All Users\Application Data\Team MediaPortal\Mediaportal\language\MP-TVSeries\ |
|:---|:---------------------------------------------------------------------------------------------------------|
| Vista & Win7 |  C:\ProgramData\Team MediaPortal\Mediaportal\language\MP-TVSeries\                                       |

> ## Series Cache (Files) ##
> From MP-TVSeries v2.9+, there will be caching of the files downloaded from thetvdb to speed up your import time. Cached series are only removed if the online api reports newer information is available.

| XP |  C:\Documents and Settings\All Users\Application Data\Team MediaPortal\Mediaportal\MP-TVSeries\Cache\ |
|:---|:------------------------------------------------------------------------------------------------------|
| Vista & Win7 |  C:\ProgramData\Team MediaPortal\Mediaportal\MP-TVSeries\Cache\                                       |

# MP-TVSeries Registry Location #

If you have modified the default path to the DB, that is stored
and can be changed in the registry using the following key

| HKEY\_CURRENT\_USER\Software\MPTVSeries\DBFile |
|:-----------------------------------------------|

Note: if you are using the default path, this will be empty.



---


# Backup and Migration #

If you want to backup your MP-TVSeries data, or migrate it to a new computer you need to backup/restore the following.

  * Backup [TVSeriesDatabase4.db3](http://code.google.com/p/mptvseries/wiki/FAQ#TVSeriesDatabase4.db3)
  * Backup [MPTVSeriesBanners and Fan Art (Folders)](http://code.google.com/p/mptvseries/wiki/FAQ#MPTVSeriesBanners_and_Fan_Art_(Folders)). Note you could just copy the entire 'thumbs' folder (recommend), especially if you have ClearART etc are doing the same process with MovingPictures.



---


# Multiple HTPCs and MP-TVSeries #

Mediaportal 1 does not have native support for sharing its databases across multiple clients, this is something scheduled for Mediaportal 2. There are options, the first, is the [multi-seat](http://wiki.team-mediaportal.com/UserGuides/CentralisedDatabases) Approach (not recommended/supported). The Second option, is below

> ## Main HTPC ##

  * Make sure all paths are using UNC paths, no local paths, mapped drives are not recommended
  * Configure your first HTPC with all the options/settings you prefer
  * Check your main HTPC is synced follw.it and or trakt
  * Run a Full Import
  * Close Mediaportal

> ## Additional HTPCs ##

> Its recommeded to have the same version of the MP-TVSeries plugin as your Main HTPC

  * Close Mediaporal
  * From the main HTPC, copy its [TVSeriesDatabase4.db3](http://code.google.com/p/mptvseries/wiki/FAQ#TVSeriesDatabase4.db3) to your additional HTPCs, overwriting.
  * From the main HTPC, copy its [MPTVSeriesBanners and Fan Art (Folders)](http://code.google.com/p/mptvseries/wiki/FAQ#MPTVSeriesBanners_and_Fan_Art_(Folders)) to your additional HTPCs, overwriting. Note you could just copy the entire thumbs folder (recommend), especially if you are doing the same process with MovingPictures etc.
  * Open Mediaportal and you should have a working MP-TVSeries. When a show is watched on 1 HTPC it will be replicated to the others when it next syncs with Follw.it or Trakt.tv

> ### Advantages ###
  * You can use all HTPCs at the same time
  * No greater risk of Database Corruption

> ### Disadvantages ###
  * Every new episode added after you copied the database/thumbs will be imported on every additional HTPC, so this will use additional internet traffic
  * Changes you make on one HTPC, e.g. disabling fanart, changing views, adding/removing favourites are not replicated to the other HTPCs. (Until you copy the database again)


---


# Language Support #
MP-TVSeries supports multiple languages, and you are welcome to contribute by updating or adding a new language.

> ## Configuration ##
  * Lauch the MP-TVSeries Plugin Configuration
  * Click _General_ Tab
  * Drop down the Language box, choose your language
  * Close MediaPortal

> ## Update Language ##
> If you find a language has incorrect spelling, or missing some translation fields, you can update the appropriate .xml file in the [Language Folder](http://code.google.com/p/mptvseries/wiki/FAQ#Language.XML_(Files)). Please submit the updated file on the [forum](http://forum.team-mediaportal.com/my-tvseries-162/)

> ## Add New Language ##
  * Download the latest English XML [here](http://mptvseries.googlecode.com/svn/trunk/MP-TVSeries/Resources/Languages/en(us).xml)
  * Rename en(us).xml to yourlanguage.xml
  * Update All Fields Possible
  * Submit the new xml to the [forum](http://forum.team-mediaportal.com/my-tvseries-162/) to be included in an upcoming build


---


# Edit Database #

> If you need to edit the MP-TVSeries database directly,you can download a SQLite tool, such as [sqlitebrowser](http://sqlitebrowser.sourceforge.net/development.html) and open the [TVSeriesDatabase4.db3](http://code.google.com/p/mptvseries/wiki/FAQ#TVSeriesDatabase4.db3) file.

> ![http://mptvseries.googlecode.com/svn/wiki/Images/SQLiteOpen.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/SQLiteOpen.jpg)


---

# Database Corruption #
Its sometimes reported that the database file TVSeriesDatabase4.db3 has become damaged in some fashion. The MP-TVSeries plugin in Mediaportal may not function correctly, such as your Series/Episodes are missing etc.

> ## Identify Corruption ##
> The MP-TVSeries.log file will usually contain multiple events like the following:
  * Commit failed on this command:
  * SQLiteClient:  cmd:sqlite3\_finalize err:CORRUPT detailed:database disk image is malformed query

> ## Causes ##
  * If you are using Mediaportal/MP-TVSeries in (unsupported and not recommended) [multi-seat mode](http://wiki.team-mediaportal.com/UserGuides/CentralisedDatabases), this will likely lead to database corruption if multiple clients write to the database at the same time
  * Hard Shutdown of PC while MP-TVSeries is preforming a database operation, (i.e Power Loss)
  * PC Crash / Lockup / BSOD
  * Your just unlucky!

> ## Solution ##
> There are 2 options, restore from a backup file, start a new database. Note: Artwork that has already been downloaded will be automatically re-used and not re-downloaded

> ### Option 1 - Restore from Backup File ###
> If you installed MP-TVSeries from the installer, it would have made a backup database in the below directory location. You could take the backup file from this location and overwrite the corrupt [TVSeriesDatabase4.db3](http://code.google.com/p/mptvseries/wiki/FAQ#TVSeriesDatabase4.db3). If the backups are extremely old, it may be wiser to use Option 2

| XP | C:\Documents and Settings\All Users\Application Data\Team MediaPortal\MediaPortal\database\TVSeries\_Backup\ |
|:---|:-------------------------------------------------------------------------------------------------------------|
| Vista & Win7 | C:\ProgramData\Team MediaPortal\MediaPortal\database\TVSeries\_Backup\                                       |


> ### Option 2 - New Database ###

  * (Optional) To retain your watch flags, and your NOT currently synced with [follw.it](http://code.google.com/p/mptvseries/wiki/FAQ#Follw.it) or [trakt.tv](http://code.google.com/p/mptvseries/wiki/FAQ#Trakt.tv), _Export Watched Flags.._ from the MP-TVSeries plugin configuration, General Tab
> ![http://mptvseries.googlecode.com/svn/wiki/Images/ExportImportWatchFlags.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/ExportImportWatchFlags.jpg)
  * Delete your database file [TVSeriesDatabase4.db3](http://code.google.com/p/mptvseries/wiki/FAQ?ts=1301645826&updated=FAQ#TVSeriesDatabase4.db3)
  * TVSeriesDatabase4.db3 will be re-created next time mediportal or the MP-TVSeries plugin configuration executes
  * Reimport your shows
  * (Optional) _Import Watched Flags_ after import is complete, or resetup your [follw.it](http://code.google.com/p/mptvseries/wiki/FAQ#Follw.it) or [trakt.tv](http://code.google.com/p/mptvseries/wiki/FAQ#Trakt.tv) account.

---


# Tips And Tricks #

> ## Delete From Disk, Database, Disk & Database ##
> > This lets you delete files or just entries from the database so the can be rescanned
    * Enable 'Allow user to delete files from context menu' in the general tab, in MP-TVSeries Plugin Configuration
    * Select a Series Season or Episode, press 0 on remote or keyboard and select the option


> ## Show Date In Regional Format ##
> > MP-TVSeries by default shows episode dates in YYYY-MM-DD format. To change this to use your regional settings
    * Enable 'Use regional settings to display dates' in the general tab, in MP-TVSeries Plugin Configuration
    * You can further tweak this by changing the Short Date syntax settings in Control Panel, Regional settings.


> ## Use "String Replacements" To Resolve Weird filenames ##
> > You might have made a typo in the filenames, are using cryptic/acronym based filenames or using a different language then what thetvdb.com uses to identify the TV Show. Instead of renaming a lot of files, you can simply use the 'String Replacements' system to fix these problems. You can find this in the 'Import' tab in MP-TVSeries plugin configuration


> ## Fan Art - View Disable Download ##
    * Select a Series/Season/Episode
    * Press Info on Remote or F9 on keyboard and Select FanArt
    * Click on a Fanart tagged Local to toggle between Default (only used if Random FanArt is off)
    * Click on a Fanart tagged Remote to Download that Fanart
    * Press F9 on Keyboard, INFO on remote to Delete a FanArt

> ## Modify 'Recently Added' 'Latest Aired' Views To Exclude Watched Episodes ##
> > To change these views so it only shows episodes currently unwatched, you can [edit](http://code.google.com/p/mptvseries/wiki/FAQ#Edit_Database) the database, and modify the query to below (Views table)

  * Latest Aired Unwatched
```
  episode<;><Episode.FirstAired>;<=;<today><cond><Episode.FirstAired>;>=;<today-30><cond><Episode.Watched>;=;0<;><Episode.FirstAired>;desc<;>
```

  * Recently Added UnWatched
```
  episode<;><Episode.FileDateCreated>;>=;<today-7><cond><Episode.Watched>;=;0<;><Episode.FileDateCreated>;desc<;>
```


> ## Speed Up Import - Ignore Old Series ##
> > If you have a large collection and notice it takes a while for the import process to run, you could tell MP-TVSeries to ignore some of your collection. You should only do this on old shows that are well and truley finished and are unlikely to be edited/changed at the tvdb.com
    * Load MP-TVSeries plugin Configuration
    * Click on the 'Details' Tab
    * Right Click an Old Series
    * Select 'Ignore on Scan'


> ## Speed Up Import - Upgrade to MP-TVSeries 2.9+ ##
> > MP-TVSeries 2.9+ has significantly faster import times compared to MP-TVSeries 2.8 and below due to a new [Caching](http://code.google.com/p/mptvseries/wiki/FAQ#Series_Cache_%28Files%29) feature. If you have a large collection, this is highly recommended.


> ## Speed Up Series Browsing - Change Layout ##
> > In Mediaportal, if you find browsing the Series list is slow or not smooth when scrolling, you may have older HTPC hardware for example, try switching the Series layouts to 'LIST POSTERS' or 'LIST BANNERS'
    * In Mediportal, go into MP-TVSeries and browse your entire Series.
    * Press F9 or INFO on MCE Remote
    * Choose 'CHANGE LAYOUT'
    * Select 'LIST POSTERS' or 'LIST BANNERS'


> ## Fast Cycling of Artwork via Keyboard or Remote ##
> > There is a way to bind a key in Mediaportal for the purpose of having a quick way to change the artwork without having to do into the menu. This need to be linked with the either or both MP actions.

  * ACTION\_PREV\_PICTURE
  * ACTION\_NEXT\_PICTURE


> To map a keyboard button to these actions:

  * Load Mediaportal Configuration
  * Click General,  Keys and Sounds
  * Select the 'WINDOWS' node
  * Click 'ADD' button
  * In Description field type 'MP-TVSeries specific' or similar
  * In Action field, enter '9811' (the window id of MP-TVSeries)
  * Click 'ADD'

> This will allow you to map the actions

  * Click  '<New Action>' node
  * Enter in description e.g. 'Cycle Artwork Next'
  * In actions, choose 'ACTION\_NEXT\_PICTURE'
  * Click on Key: and press keyboard character
  * Click OK
  * Repeat these steps if you want to bind ACTION\_PREV\_PICTURE

> Load Mediaportal, TVSeries plugin, and press the KEY you set to change the artwork


> ## Playlist Keyboard Shortcuts ##
> The following are shortcuts avaialble for playlists in MP-TVSeries
  * Play Next = F8
  * Play Prev = F7
  * Add to Playlist = Y
  * Show Playlist = F1
> Note: for Add to Playlist and Show Playlist shorcuts, you need to add them to "Keys and Sounds" in the Mediaportal Configuration. See screenshow below. Note: Window ID for MP-TVSeries is 9811
> ![http://mptvseries.googlecode.com/svn/wiki/Images/PlaylistShortcuts.jpg](http://mptvseries.googlecode.com/svn/wiki/Images/PlaylistShortcuts.jpg)

---
