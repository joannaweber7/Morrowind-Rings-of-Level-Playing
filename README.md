# Morrowind-Rings-of-Level-Playing
; Script from old Morrowind mod to instantly level a character in Bloodmoon to level 50, especially useful for testing mods with a clean save. This is an adaptation of a script by Grumpy, expanded, revised and attached to a ring in the game. Mod can be downloaded from Morrowind Mod History.
	
	short OnPcEquip
	short myadd
	
	if ( OnPCEquip == 0 )
		Return
	elseif ( myadd > 9 )
		Return
	elseif ( myadd == 0 )
		player->setlevel 50
		player->sethealth 500
		player->setspeed 100
		player->setstrength 100
		player->setfatigue 400
		player->setintelligence 100
		player->setwillpower 100
		player->setagility 100
		player->setendurance 100
		player->setpersonality 92
		player->setluck 40
		player->setreputation 60
		set myadd to 1
	elseif ( myadd == 1 )
		player->setlongblade 100
		player->setmarksman 100
		player->setsecurity 24
		player->setathletics 100
		player->setacrobatics 100
		player->setunarmored 100
		player->setlightarmor 100
		player->setmediumarmor 100
		player->setheavyarmor 62
		player->setblock 100
		player->setmagicka 200
		player->setmysticism 19
		player->setillusion 19
		player->setconjuration 14
		player->setalteration 19
		player->setenchant 14
		player->setdestruction 14
		player->sethandtohand 14
		player->setspeechcraft 14
		player->setrestoration 24
		player->setmercantile 14
		player->setalchemy 19
		player->setsneak 62
		player->setspear 14
		player->setaxe 62
		player->setbluntweapon 100
		player->setarmorer 100
		player->setshortblade 14
		set myadd to 2
	elseif ( myadd == 2 )
		player->addspell mark
		player->addspell recall
		player->addspell levitate
		player->addspell "almsivi intervention"
		player->addspell "divine intervention"
		player->addspell "hearth heal"
		player->addspell "command humanoid"
		player->addspell "command creature"
		player->addspell "concealment"
		player->addspell "cure common disease"
		player->addspell "cure common disease other"
		player->addspell "dire weakness to fire"
		player->addspell "fireball_large"
		player->addspell "resist magicka"
		player->addspell "restore agility"
		player->addspell "restore endurance"
		player->addspell "restore intelligence"
		player->addspell "restore luck"
		player->addspell "restore personality"
		player->addspell "restore speed"
		player->addspell "restore strength"
		player->addspell "restore willpower"
		player->addspell "sanctuary"
		player->addspell "slowfall"
		player->addspell "sotha's mirror"
		player->addspell "strong feather"
		player->addspell "summon skeletal minion"
		player->addspell "summon scamp"
		player->addspell "BM_summonwolf"
		player->addspell "BM_summonbear"
		player->addspell "absorb health"
		player->addspell "common disease immunity"
		player->addspell "blight disease immunity"
		player->addspell "her_reflected_glory"
		player->addspell "her_protection"
		player->addspell "her_ironskin"
		set myadd to 3
	elseif ( myadd == 3 )
		player->additem "p_restore_magicka_e" 10
		player->additem "p_restore_health_e" 25
		player->additem "p_restore_fatigue_e" 5
		player->additem "adamantium boots" 1
		player->additem "expensive_pants_Mournhold" 1
		player->additem "expensive_shirt_Mournhold" 1
		player->additem "expensive_shoes_Mournhold" 1
		player->additem "daedric long bow" 1
		player->additem "steel arrow" 200
		player->additem "gold_001" 65000
		player->additem "gold_001" 65000
		player->additem "apparatus_g_alembic_01" 1
		player->additem "apparatus_g_calcinator_01" 1
		player->additem "apparatus_g_mortar_01" 1
		player->additem "apparatus_g_retort_01" 1
		player->additem "pick_grandmaster" 1
		player->additem "pick_master" 5
		player->additem "probe_grandmaster" 1
		player->additem "probe_master" 1
		player->additem "wraithguard" 1
		player->additem "sunder" 1
		player->additem "keening" 1
		player->additem "cuirass_savior_unique" 1
		player->additem "boots of blinding speed[unique]" 1
		player->additem "amulet of shadows" 1
		player->additem "caius_pants" 1
		player->additem "caius_shirt" 1
		player->additem "seizing" 1
		player->additem "teeth" 1
		player->additem "hortatorring" 1
		player->additem "hortatorrobe" 1
		player->additem "hortatorbelt" 1
		player->additem "ring of azura" 1
		player->additem "common_shoes_02_surefeet" 1
		player->additem "thong" 1
		player->additem "peakstar_pants_unique" 1
		player->additem "artifact_amulet of heartfire" 1
		player->additem "artifact_amulet of heartheal" 1
		player->additem "artifact_amulet of heartrime" 1
		player->additem "artifact_amulet of heartthrum" 1
		player->additem "daedric_special" 1
		player->additem "King's_Oath_pc" 1
		player->additem "Sword of Almalexia" 1
		player->additem "nerevarblade_01_flame" 1
		player->additem "heart ring" 1
		player->additem "madstone" 1
		player->additem "moon_and_star" 1
		player->additem "BM_hunterspear_unique" 1
		player->additem "BM_Mace_Aevar_UNI" 1
		player->additem "BM_Ice_Shield" 1
		player->additem "BM Wolf Helmet_heartfang" 1
		player->additem "ring_khajiit_unique" 1
		player->additem "ebony wizard's staff" 1
		player->additem "conoon_chodala_axe_unique" 1
		player->additem "misc_soulgem_grand" 10
		player->additem "repair_grandmaster_01" 10
		player->additem "BM Nordic Pick" 1
		set myadd to 4
	elseif ( myadd == 4 )
		player->equip "adamantium boots" 1
		player->equip "expensive_pants_Mournhold" 1
		player->equip "expensive_shirt_Mournhold" 1
		player->equip "daedric long bow" 1
		player->equip "steel arrow" 200
		set stronghold to 6
		set FabAttack to 1
		set colonyservice to 6
		set ColonyState to 36
		Set SkaalAttack to 4
		Set colonyside to 1
		set myadd to 5
	elseif ( myadd == 5 )
		Journal "CO_13" 70
		Journal "MG_Guildmaster" 100
		Journal "FG_KillHardHeart" 100
		Journal "IL_Grandmaster" 100
		Journal "MG_Guildmaster" 100
		Journal "MG_Advancement" 70
		Journal "MT_Grandmaster" 110
		Journal "A2_4_MiloGone" 1
		Journal "A2_6_Incarnate" 50
		Journal "A2_2_6thHouse" 50
		Journal "A2_3_CorprusCure" 50
		Journal "HH_Stronghold" 300
		Journal "B7_TelvanniHort" 70
		Journal "B6_HlaaluHort" 50
		Journal "B5_RedoranHort" 60
		Journal "B8_All_Hortator" 50
		Journal "B8_All_Nerevarine" 50
		Journal "B8_MeetVivec" 50
		Journal "B8_MeetVivec" 55
		Journal "C3_destroyDagoth" 50
		Journal "A1_SleepersAwake" 50
		Journal "TR_DBAttack" 30
		Journal "TR_DBAttack" 60
		Journal "TR_Champion" 80
		Journal "TR_Champion" 110
		Journal "TR_SothaSil" 110
		Journal "TR_Bamz" 100
		Journal "BM_MeadHall" 100
		Journal "BM_Morale" 110
		Journal "BM_SkaalAttack" 100
		Journal "BM_Sun" 100
		Journal "BM_Trees" 100
		Journal "BM_Water" 100
		Journal "BM_Earth" 100
		Journal "BM_Wind" 100
		Journal "BM_Missionary" 100
		Journal "BM_Wildhunt" 100
		Journal "BM_Trial" 100
		Journal "CO_5" 80
		set myadd to 6
	elseif ( myadd == 6 )
		Act_BM_Earth_parts->Enable
		Act_BM_Sun_parts->Enable
		Act_BM_Tree_parts->Enable
		Act_BM_Water_parts->Enable
		Act_BM_Wind_parts->Enable
		ex_s_door_rigmor->disable
		"BM_werewolf_skaal1a3"->disable
		"BM_werewolf_skaal1b3"->disable
		"BM_werewolf_skaal1c3"->disable
		"bm_werewolf_skaal1d3"->disable
		"bm_werewolf_skaal1e3"->disable
		"bm_werewolf_skaal1f3"->disable
		"bm_werewolf_skaal1g3"->disable
		"bm_werewolf_skaal2a"->disable
		"Tharsten Heart-Fang"->disable
		"Mirisa"->disable
		"Rigmor HalfHand"->disable
		"Carnius Magius"->disable
		"BM_Udyrfrykte"->disable
		"sjoring hard-heart"->disable
		"varus vatinius"->disable
		"trebonius artorius"->disable
		"eno hlaalu"->disable
		"gothren"->disable
		"stacey"->disable
		"orvas dren druglord"->disable
		"caius cosades"->disable
		"bolvyn venim"->disable
		"yngling half-troll"->disable
		"eydis fire-eye"->disable
		"tongue_toad"->disable
		"ulath-pal"->disable
		"ahaz"->disable
		"ranabi"->disable
		"ashu-ahhe"->disable
		"raynasa rethan"->disable
		"banden indarys"->disable
		"reynel uvirith"->disable
		"salas valor"->disable
		"gaenor"->disable
		set myadd to 7
	elseif ( myadd == 7 )
		"Dagoth_ur_1"->disable
		"Dagoth_ur_1"->disable
		"dagoth_ur_2"->disable
		"akula door a"->disable
		"akula door b"->disable
		"dagoth baler"->disable
		"dagoth daynil"->disable
		"dagoth delnus"->disable
		"dagoth drals"->disable
		"Dagoth Draven"->disable
		"dagoth elam"->disable
		"dagoth fals"->disable
		"dagoth fandril"->disable
		"dagoth felmis"->disable
		"dagoth fervas"->disable
		"dagoth fovon"->disable
		"dagoth galmis"->disable
		"dagoth garel"->disable
		"dagoth gares"->disable
		"dagoth girer"->disable
		"dagoth goral"->disable
		"dagoth ienas"->disable
		"dagoth irvyn"->disable
		"dagoth mendras"->disable
		"dagoth molos"->disable
		"dagoth muthes"->disable
		"dagoth nilor"->disable
		"dagoth ralas"->disable
		"dagoth rather"->disable
		"dagoth reler"->disable
		"dagoth soler"->disable
		"dagoth tanis"->disable
		"dagoth ulen"->disable
		"dagoth uvil"->disable
		"dagoth vaner"->disable
		"dagoth_hlevul"->disable
		"blight cloud"->Disable;this is the big object outside
		"in_akulakhan00"->PlayGroup, Death1
		"in_dagoth_bridge00"->PlayGroup, Death1
		"heart_akulakhan"->disable
		set HeartDestroyed to 1
		set myadd to 8
	elseif ( myadd == 8 )
		ModRegion "Red Mountain Region" 50 50 0 0 0 0 0 0
		ChangeWeather "Red Mountain Region" 0
		"Dagoth Uthol"->SetHealth 0
		"Dagoth Vemyn"->SetHealth 0  
		"Dagoth Endus"->SetHealth 0
		"Dagoth Odros"->SetHealth 0
		"Dagoth Tureynul"->SetHealth 0
		"Dagoth Gilvoth"->SetHealth 0
		"Dagoth Araynys"->SetHealth 0
		set DestroyBlight to -1;global variable
		Player->ModReputation 10;gives the player reputation reward
		"fabricant_verm_attack"->disable
		"fabricant_hulkin_attack"->disable
		"fabricant_verminous_C"->disable
		"centurion_projectile_C"->disable
		"fabricant_hulking_C"->disable
		"centurion_steam_A_C"->disable
		"fabricant_hulking_C_L"->disable
		"fabricant_verminous"->disable
		fabricant_verminous-rs->sethealth 0
		in_sotha_sil00->disable
		Almalexia_warrior->disable
		Imperfect->sethealth 0
		fabricant_hulking->disable
		fabricant_hulking_ss->disable
		set myadd to 9
	elseif ( myadd == 9 )

PCJoinFaction "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"
PCRaiseRank "Mages Guild"

PCJoinFaction "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"
PCRaiseRank "Ashlanders"

PCJoinFaction "Blades"
PCRaiseRank "Blades"
PCRaiseRank "Blades"
PCRaiseRank "Blades"
PCRaiseRank "Blades"
PCRaiseRank "Blades"
PCRaiseRank "Blades"

PCJoinFaction "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"
PCRaiseRank "Fighters Guild"

PCJoinFaction "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"
PCRaiseRank "Imperial Legion"

PCJoinFaction "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"
PCRaiseRank "Temple"

PCJoinFaction "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"
PCRaiseRank "Imperial Cult"


PCJoinFaction "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"
PCRaiseRank "Morag Tong"


PCJoinFaction "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"
PCRaiseRank "Thieves Guild"

PCJoinFaction "Skaal"

PCJoinFaction "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"
PCRaiseRank "East Empire Company"

Set OnPCEquip to 0
set myadd to 10
endif

end
