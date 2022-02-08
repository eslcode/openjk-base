# openjk-base

Jedi Academy full featured client for competitive play (limited edition)

* Privacy hardening (`esl_antileak`, auto rename to Padawan on disconnect and disabling GUID by default)
* Encrypted chat with a 128-bit key PKI (`esay`, `esay_team`, `etell`, `etell_target`, `esl_chat_key`, `esl_chat_toggle` for sending encrypted via SHIFT+Enter)
* Command timers without blocking input (`/timer`)
* Non-blocking alternative to `wait` (`/do` for ms delay and `dofps` for fps delay, multiple commands possible)
* Shader tracer (`shadertrace`)
* Cvar unlocker (`esl_cvarprotection`)
* Lag unlocker 
* Draw people spectating you (`cg_drawspectators`)
* Anti-afk with custom commands (`esl_noafk`, `esl_noafk_cmd`, `esl_afktime`)
* Extra Sensory Perception (`esl_drawnames_*` includes ping, distance, client number, saber stance and HP teller)
* Wallhack (`esl_wallcontrol`)
* Aimbot (`+esl_targetacquire`, `esl_targetacquire_*`)
* Speedhack (`esl_movespeed` and `esl_prorun`)
* Laghack (`esl_disableNetSend`)
* Metroid "charged" jump (`+esl_jump`)
* Extended client list (`esl_userinfo_*`)
* Some public exploits from aluigi
* Range circles (`esl_drawcircles`)
* Faster connection (`esl_fastconn_*`)
* Vertical cvar exploit (`esl_verticalcvar`)
* Chat walk exploit (`esl_chatwalk`)
* High wallrun exploit (`esl_autoProWallrun`)
* Auto-wiggle exploit (`esl_prowiggle` - most efficient auto-wiggle ever existed, proven to work on japlus and fps30)
* Parry bot with a flexible config (`esl_b_*`)
* Auto-poke (`esl_propoke`)
* Full force automation (`esl_ff_antisplat` anti splat, `esl_ff_antigrip` anti grip (auto push, auto pull and custom cmd), `esl_ff_autoheal` auto heal, `esl_ff_autodrain` auto drain, `esl_ff_autoabsorb` auto absorb, `esl_ff_autokick` auto kickflip)
* A lot of other stuff

Not included in this version (available in the full edition):

* 2 private japlus DoS exploits (crash any server including JoF)
* japlus IP spoofing exploit (substitutes your IP to any other making bans easily to avoid)
* basejka 1.01 FX spawner exploit (spawn effects on the map without admin permission)
* basejka 1.01 permanent invulnerability exploit (nobody can hit you)
* auto strafe feature


Ported from JAPRO/EJK:

* Low jump (`cg_jumpHeight`)
* Flipkick (`flipkick`, `flipkick_*`)
* Strafe helper (`strafeHelper`, `cg_strafeHelper_*`)
* Bright skins (`cg_playerSkins_bright` enhanced with `cg_playerSkins_shader` for a custom shader for player models) 
* Custom chat styles (`cl_chatStylePrefix` and `cl_chatStyleSuffix`)
* Movement keys (`cg_movementKeys`)
* Speedometer (`speedometer` and `cg_speedometer`)
* `cg_drawHitBox`
* `com_renderfps`
* `cg_showpos`
* `cg_autoKillWhenFalling` enhanced with `esl_autoCmdWhenFalling` - a custom command on fall

Why this has been released:

This game became a script competition due to many critical vulnerabilities that remain unfixed so there is no point in keeping this client private.

We gave some time before release and notified the current server code project maintainers about the problems, but they continued to refuse the existence of vulnerabilities that make possible exploiting the game in a very blatant way by this and a few other private clients of the same complexity. Auto wiggle exploit, parry bot and speedhacks are most exemplar demonstrations of how easy one can win without putting effort. 

The most problematic parts of the server-side code are saber blocks and saber attack that vastly depend on RNG, which means the whole gameplay is based on luck. The netcode is also 20 years old and remains highly unoptimized which makes it unplayable on ping higher than 50, unless the player use exploits. 

All these issues were fixed by the MB2 coding team, however they decided to not help improving the original game and left JKA community without fixes, thus the fixes weren't released yet. Those issues were the subject of discussions for last 10 years and current JKA devs still prefer to refuse the facts or simply not caring.

