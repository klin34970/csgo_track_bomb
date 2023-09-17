I - Description
I made this plugin for my community Zombie4Ever.eu and was allowed to share it.
This plugin will show a menu for the bomber at the roundstart and will choose the direction and way where he wants to go. Also they are some warning HUD/chat/Alert for the bomb event loke bomb_pickup, bomb_dropped....

II - Cvars
"active_track_bomb" Enable/Disable Track the bomb
"active_track_bomb_c4_explode" Enable/Disable Explode bomb on holder
"active_track_bomb_name" Enable/Disable Name of holder in chat
"active_track_bomb_chat" Enable/Disable Chat message
"active_track_bomb_hint" Enable/Disable Hint message
"active_track_bomb_alert" "Enable/Disable Alert message"
"active_track_bomb_delay_time_msg" Delay time for Chat/Hint/Alert Message
"active_track_bomb_hit_num" Number of hit for explode bomb

You can only choose active_track_bomb_hint or active_track_bomb_alert

III - Configs
"TrackBomb" 
{ 
    "de_dust2" 
    { 
        "direction" 
        { 
            "A"
            { 
                "1"            "Short" 
                "sound1"        "track_bomb/bombsitea.mp3" 
                "2"            "Long" 
                "sound2"        "track_bomb/bombsitea.mp3" 
                "3"            "Middle" 
                "sound3"        "track_bomb/bombsitea.mp3" 
            } 
            "B" 
            { 
                "1"            "Tunnel" 
                "sound1"        "track_bomb/bombsiteb.mp3" 
                "2"            "Middle Tunnel" 
                "sound2"        "track_bomb/bombsiteb.mp3" 
                "3"            "Middle" 
                "sound3"        "track_bomb/bombsiteb.mp3" 
            } 
        } 
    } 

    "de_dust" 
    { 
        "direction" 
        { 
            "A" 
            { 
                "1"            "Way1" 
                "sound1"        "track_bomb/bombsitea.mp3" 
                "2"            "Way2" 
                "sound2"        "track_bomb/bombsitea.mp3" 
            } 
            "B" 
            { 
                "1"            "Way1" 
                "sound1"        "track_bomb/bombsiteb.mp3" 
                "2"            "Way2" 
                "sound2"        "track_bomb/bombsiteb.mp3" 
                "3"            "Way3" 
                "sound3"        "track_bomb/bombsiteb.mp3" 
            } 
        } 
    } 
}  
Sounds will be automactically downloaded and precached.
You can put 100maps max, 8 directions max and 16 ways max but this can be increase of course.
You can custom the sound for each way.
The sound is played when the bomber choose the way.
If you don't want song set to "none" Ex: "sound1" "none"


IV - Notes
If the bomber drop and re-pickup the bomb, the menu will not popup. 
If the bomber is killed the menu is disabled.
If the bomber is killed and "active_track_bomb_c4_explode" is enabled, the bomb will explode, so when a bomb explode it disappears.

V - Changelogs
V1.0.3
-Fixed a material path.

V1.0.2
-Added cvar active_track_bomb_freeze_holder will freeze the bomber at round start until he choose a way.
-Menu doesn't have exit back button anymore.
-Plugin infos set.

V.1.0.1
-Possibility to have the explose bomb mod without the tracking mod.