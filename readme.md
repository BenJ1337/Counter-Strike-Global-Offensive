## Counter-Strike-Global-Offensive Binds/Commands

1. [Command Detail](#1-Command-Detail)
2. [Buy Script](#2-buy-script)
3. [Crosshair](#3-crosshair)
4. [Viewmodel](#4-viewmodel)
5. [Radar](#5-radar)
6. [Display Text out of the console](#6-display-text-out-of-the-console)
7. [Limit FPS (144Hz Monitor)](#7-limit-fps-144Hz-monitor)
8. [Anti Autokick](#8-anti-autokick)
9. [Network Statistics](#9-network-statistics)
10. [Display Equipment of your Teammates](#10-display-equipment-of-your-teammates)
11. [Hide Player-Profil Pictures](#11-hide-player-profil-pictures)

### 1. Command Detail

- [Command Detail - Source Engine (developer.valvesoftware.com)](https://developer.valvesoftware.com/wiki/Console_Command_List)
- [Command Detail - CSGO](/CSGO-Cmds.csv)

### 2. Buy Script

	bind "kp_end" "buy p250;"
	bind "kp_ins" "buy vesthelm;"
	bind "kp_del" "buy defuser;"
	bind "kp_enter" "buy ak47; buy m4a1;"

	bind "kp_home" "buy hegrenade;"
	bind "kp_uparrow" "buy flashbang;"
	bind "kp_pgup" "buy smokegrenade;"

	bind "kp_plus" "buy molotov; buy incgrenade;"
	bind "kp_minus" "buy decoy;"
	bind "kp_leftarrow" "buy p90;"
	bind "kp_5" "buy awp;"
	bind "kp_rightarrow" "buy galilar; buy famas;"
	bind "kp_downarrow" "buy tec9; buy fiveseven;"
	bind "kp_pgdn" "buy deagle;"
	bind "kp_multiply" "buy Taser;"
	bind "kp_slash" "buy ump45;"

### 3. Crosshair

	cl_crosshairalpha "200"
	cl_crosshaircolor "5"
	cl_crosshaircolor_b "0"
	cl_crosshaircolor_r "0"
	cl_crosshaircolor_g "250"
	cl_crosshairdot "0"
	cl_crosshairgap "-14"
	cl_crosshairsize "2"
	cl_crosshairstyle "4"
	cl_crosshairusealpha "1"
	cl_crosshairthickness "0.5"
	cl_fixedcrosshairgap "-9"
	cl_crosshair_outlinethickness "1"
	cl_crosshair_drawoutline "1"

### 4. Viewmodel

	viewmodel_presetpos "3"
	viewmodel_fov "68"
	viewmodel_offset_x "2"
	viewmodel_offset_y "2"
	viewmodel_offset_z "-2"
	cl_viewmodel_shift_left_amt "0"
	cl_viewmodel_shift_right_amt "0"
	cl_bob_lower_amt "0"
	cl_bobamt_lat "0"
	cl_bobamt_vert "0"
	cl_bobcycle "0.98"

### 5. Radar

	cl_radar_always_centered 0
	cl_radar_scale 0.4
	cl_hud_radar_scale 1.3

### 6. Display Text out of the console

	developer "1"
	con_filter_enable "2"
	con_filter_text_out "Player:"
	con_filter_text "Damage "

### 7.Limit FPS (144Hz Monitor)

	fps_max "150"

### 8. Anti Autokick

	alias prevAutoKick prevAutoKick_on;
	alias "prevAutoKick_on" "+forward; +moveleft; +left; alias prevAutoKick prevAutoKick_off";
	alias "prevAutoKick_off" "-forward; -moveleft; -left; alias prevAutoKick prevAutoKick_on";
	bind "l" "prevAutoKick"

### 9. Network Statistics

	net_graph 1;
	net_graphpos 1;
	net_graphproportionalfont 0;

### 10. Display Equipment of your Teammates

	alias ToggleInfo info_off;
	alias "info_off" "-cl_show_team_equipment;cl_teamid_overhead_always 0; alias ToggleInfo info_on";
	alias "info_on" "+cl_show_team_equipment;cl_teamid_overhead_always 1; alias ToggleInfo info_off";
	bind "u" "ToggleInfo"
	ToggleInfo;

### 11. Hide Player-Profil Pictures

	cl_hide_avatar_images "2";
	0 - Show all Pictures
	1 - Show only your own profil picture
	2 - Show your and your friends profil picture
