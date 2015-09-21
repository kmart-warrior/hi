exec reset

// press and hold middle mouse button to turn on autosap and sap everything you see.
// release middle button to return to last weapon
alias autosapOn "slot2; +attack; alias toggleAutosap autosapOff"
alias autosapOff "-attack; lastinv; alias toggleAutosap autosapOn"

alias "toggleAutosap" "autosapOn"

alias "+mouse3Down" "toggleAutosap"
alias "-mouse3Down" "toggleAutosap"

bind "mouse3" "+mouse3Down"

alias undisguise "disguise 8 -2"
bind X undisguise

bind R "say_team *****SAPPING*****"
bind T "say_team *****SENTRY DOWN PUSH FOWARD*****

alias e_scout "disguise 1 -1; playgamesound scout.yes01"
alias e_sniper "disguise 2 -1; playgamesound sniper.yes03"
alias e_soldier "disguise 3 -1; playgamesound soldier.yes04"
alias e_demoman "disguise 4 -1; playgamesound demoman.yes01"
alias e_medic "disguise 5 -1; playgamesound medic.yes03"
alias e_hwguy "disguise 6 -1; playgamesound heavy.yes03"
alias e_pyro "disguise 7 -1; playgamesound pyro.moveup01"
alias e_spy "disguise 8 -1; playgamesound spy.yes02"
alias e_engineer "disguise 9 -1; playgamesound engineer.yes03"

alias a_scout "disguise 1 -2; playgamesound scout.no02"
alias a_sniper "disguise 2 -2; playgamesound sniper.no01"
alias a_soldier "disguise 3 -2; playgamesound soldier.no02"
alias a_demoman "disguise 4 -2; playgamesound demoman_no03"
alias a_medic "disguise 5 -2; playgamesound medic.no01"
alias a_hwguy "disguise 6 -2; playgamesound heavy.no03"
alias a_pyro "disguise 7 -2; playgamesound pyro.no01"
alias a_spy "disguise 8 -2; play vo\spy_no03"
alias a_engineer "disguise 9 -2; play vo\engineer_no01"

alias dropdisguise "echo DISGUISE_DROP;disguise 8 -2"

bind 1 e_scout
bind 2 e_soldier
bind 3 e_pyro
bind 4 e_demoman
bind 5 e_hwguy
bind 6 e_engineer
bind 7 e_medic
bind 8 e_sniper
bind 9 e_spy
bind "x" "dropdisguise; slot10"

alias +f_disg "bind 1 a_scout; bind 2 a_soldier; bind 3 a_pyro; bind 4 a_demoman; bind 5 a_hwguy; bind 6 a_engineer; bind 7 a_medic; bind 8 a_sniper; bind 9 a_spy"
alias -f_disg "bind 1 e_scout; bind 2 e_soldier; bind 3 e_pyro; bind 4 e_demoman; bind 5 e_hwguy; bind 6 e_engineer; bind 7 e_medic; bind 8 e_sniper; bind 9 e_spy"

bind SHIFT +f_disg


//Ambassador Zoom Script
alias "+ambyzoom" "fov_desired 75; viewmodel_fov 54; viewmodel_fov_demo 70; sensitivity 1.5"
alias "-ambyzoom" "fov_desired 90; viewmodel_fov 90; viewmodel_fov_demo 70; sensitivity 3.5"
bind "CTRL" "+ambyzoom"
