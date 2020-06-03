# tft_data
I am pulling tft challenger match data from RIOT API. The aim of the project is to classify each match datapoint into comps via clustering. Some statistics based analysis are available on e.g. reddit, but most of them only count each specific comp. For example if someone plays blaster brawlers with Asol instead of MF, it might not show up on the statistics since it is different from the mainstream version. Kayle comps often have less representation since they have many variation. I want to group the data into comps without pre-defining what the comps are. This way, I might be able to identify new interesting comps being played but not yet mainstream. 

Sample results:

['Set3_Celestial_1.0', 'DarkStar_1.0', 'Sniper_1.0', 'Set3_Mystic_0.7', 'Chrono_0.6', 'Vanguard_0.6', 'Set3_Sorcerer_0.5', 'ManaReaver_0.2', 'Protector_0.2', 'Set3_Brawler_0.1']
Playrate:  7.67 %
Average placement:  4.81
Average placement with 0, 1, 2 contesters:  4.79 4.82 4.97
Winrate:  10.6 %
Winrate with 0, 1, 2 contesters:  10.62 % 11.26 % 7.69 %
-------------------------------------------------------------------------
['Set3_Brawler_1.8', 'Blaster_1.6', 'Chrono_0.9', 'Mercenary_0.8', 'Rebel_0.5', 'Set3_Mystic_0.2', 'Starship_0.2', 'Set3_Celestial_0.1', 'Demolitionist_0.1', 'SpacePirate_0.1', 'Valkyrie_0.1']
Playrate:  9.81 %
Average placement:  4.53
Average placement with 0, 1, 2 contesters:  4.4 4.66 4.56
Winrate:  11.67 %
Winrate with 0, 1, 2 contesters:  13.95 % 8.33 % 12.75 %
-------------------------------------------------------------------------
['Set3_Celestial_1.2', 'Set3_Blademaster_1.0', 'Chrono_1.0', 'ManaReaver_0.8', 'Mercenary_0.5', 'Valkyrie_0.5', 'Set3_Mystic_0.4', 'Protector_0.3', 'Sniper_0.3', 'Vanguard_0.3', 'Blaster_0.1']
Playrate:  24.79 %
Average placement:  4.4
Average placement with 0, 1, 2 contesters:  3.94 4.28 4.59
Winrate:  11.68 %
Winrate with 0, 1, 2 contesters:  16.56 % 11.11 % 10.2 %
-------------------------------------------------------------------------
['Infiltrator_2.0', 'MechPilot_1.0', 'Set3_Sorcerer_0.8', 'Demolitionist_0.6', 'Valkyrie_0.5', 'Mercenary_0.2', 'DarkStar_0.1']
Playrate:  9.58 %
Average placement:  4.5
Average placement with 0, 1, 2 contesters:  4.29 4.91 5.0
Winrate:  10.75 %
Winrate with 0, 1, 2 contesters:  12.93 % 6.72 % 0.0 %
-------------------------------------------------------------------------
['Set3_Sorcerer_2.8', 'StarGuardian_1.0', 'Vanguard_0.6', 'Chrono_0.5', 'Mercenary_0.5', 'Demolitionist_0.2', 'DarkStar_0.1', 'Set3_Mystic_0.1', 'SpacePirate_0.1']
Playrate:  7.41 %
Average placement:  4.6
Average placement with 0, 1, 2 contesters:  4.52 4.78 4.6
Winrate:  12.67 %
Winrate with 0, 1, 2 contesters:  13.29 % 11.7 % 6.67 %
-------------------------------------------------------------------------
['Set3_Brawler_1.8', 'Chrono_1.0', 'Set3_Sorcerer_1.0', 'Set3_Void_1.0', 'Infiltrator_0.9', 'Demolitionist_0.1', 'Mercenary_0.1']
Playrate:  12.97 %
Average placement:  4.24
Average placement with 0, 1, 2 contesters:  3.88 4.5 5.04
Winrate:  15.89 %
Winrate with 0, 1, 2 contesters:  19.61 % 12.88 % 9.8 %
-------------------------------------------------------------------------
['SpacePirate_1.1', 'Mercenary_0.9', 'Vanguard_0.9', 'Set3_Celestial_0.8', 'Demolitionist_0.7', 'Sniper_0.7', 'Chrono_0.6', 'ManaReaver_0.6', 'Set3_Mystic_0.3', 'Blaster_0.2', 'DarkStar_0.1']
Playrate:  5.45 %
Average placement:  4.64
Average placement with 0, 1, 2 contesters:  4.6 4.72 5.08
Winrate:  12.82 %
Winrate with 0, 1, 2 contesters:  13.89 % 10.58 % 0.0 %
-------------------------------------------------------------------------
['Set3_Celestial_2.1', 'Protector_1.1', 'ManaReaver_1.0', 'SpacePirate_1.0', 'Sniper_0.4', 'Vanguard_0.4', 'Mercenary_0.2', 'Chrono_0.1', 'Set3_Mystic_0.1']
Playrate:  3.07 %
Average placement:  4.91
Average placement with 0, 1, 2 contesters:  4.87 6.08 3.67
Winrate:  11.57 %
Winrate with 0, 1, 2 contesters:  11.86 % 0.0 % 33.33 %
-------------------------------------------------------------------------
['Cybernetic_1.5', 'Set3_Blademaster_0.8', 'ManaReaver_0.7', 'Chrono_0.6', 'Blaster_0.4', 'Vanguard_0.4', 'Set3_Celestial_0.3', 'Infiltrator_0.2', 'Mercenary_0.2', 'Valkyrie_0.2', 'Set3_Brawler_0.1']
Playrate:  7.62 %
Average placement:  4.92
Average placement with 0, 1, 2 contesters:  4.9 4.91 5.25
Winrate:  11.86 %
Winrate with 0, 1, 2 contesters:  12.62 % 11.43 % 6.25 %
-------------------------------------------------------------------------
['Rebel_1.8', 'Demolitionist_0.9', 'Mercenary_0.9', 'Blaster_0.8', 'Starship_0.5', 'Set3_Brawler_0.4', 'Set3_Mystic_0.4', 'Set3_Blademaster_0.2', 'Chrono_0.1', 'SpacePirate_0.1', 'Valkyrie_0.1']
Playrate:  11.54 %
Average placement:  4.27
Average placement with 0, 1, 2 contesters:  4.13 4.36 4.8
Winrate:  14.29 %
Winrate with 0, 1, 2 contesters:  16.24 % 12.04 % 10.61 %
-------------------------------------------------------------------------