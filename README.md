# UIcons Universal Icons

UIcons is an attempt to create a universal and cooperative standard for Icons used across different PoGo projects. Full standard and its changes will be discussed openly and to every creator adopting the standard.

Join the discussion @ [Discord](https://discord.gg/cG8JwrJB6Z)

## Repo's that have adopted or have agreed to adopt

* [nileplumb](https://github.com/nileplumb) Shuffle and Home iconsets
* [whitewillem](https://github.com/whitewillem/PogoAssets) Ingame and Ingame outline iconsets
* [jms412](https://github.com/jms412/) Shuffle and Home shiny split icons

### Main folder structure approved

- gym
- raid
  - egg 
- invasion
- pokemon
- pokestop
- reward
  - item
  - stardust
  - candy
  - xl_candy
  - mega_resource
  - Subfolders can be added without approval as long as the follow exact [Proto names](https://github.com/Furtif/POGOProtos/blob/a53979d6bba81df45b1f09f7c1aa8185cb999959/base/base.proto#L16087)
- station
- team
- type
- nest
- weather
- device
- spawnpoint
- misc 

### Mandatory image keys are wrapped in `< >`
### Optional flags are wrapped in `{ }`

### Pokemon icons

  - `<pokemon id>[_e{temp evolution id}][_f{form id}][_c{costume id}][_g{gender id}][_a{alignment_id}][_s{shiny}].png`
    - Example: `3.png` Regular Venusaur
    - Example: `3_e1_s.png` Mega Venusaur Shiny
    - Example: `3_f950.png` Venusaur Clone Form
    - Example: `3_a1.png` Shadow Venusaur

### Reward icons
  - item: `<item id>[_a{amount}].png`
  - stardust:`<amount>.png`
  - mega_resouce:`<pokemon id>[_a{amount}].png`
  - candy: `<pokemon id>[_a{amount}].png`
  - xl_candy:`<pokemon id>[_a{amount}].png`
### Gym icons
  - gym: `<team id>[_t{trainer count}][_b][_ex][_ar][_p{1-3}].png` (`_b` in active battle, `_ex` ex gym, `_ar` ar eligible (no flag means false), `_p` Power Up Level from AR Scan submissions)
### Raid icons 
  - egg: `<egg level>[_h][_ex].png` (`_h` hatched egg `_ex` ex gym (no flag means false))
### Invasion icons
  - invasion: `<grunt id>[_i{incident_display_type}]_u.png` (`_u` unconfirmed giovanni)
### Pokestop icons
  - pokestop: `<lure id**>[_i{incident_display_type}][_q{with_ar}][_ar][_p{1-3}].png` ( `_i` incident active, `_q` quest active, `_ar` ar eligible, `_p` Power Up Level from AR Scan submissions) images from invasion and reward folder can be used as overlay
  - ** Not lured is ID `0` further follow proto's
  - `_q`: Any or both AR and non-AR quests are active
  - `_q0`: Non-AR quest active
  - `_q1`: AR quest active
  - `_i`: Default incident active (Team Rocket)
  - `_i7`: Generic (Type 7) incident active (Gold Pokestop)
### Team Icons
  - team: `<team id>.png` (Team badges not to be confused with Gym icons)
### Type Icons
  - type: `<type id>.png`
### Nest Icons
  - nest: `<type id>.png` 
### Weather Icons
  - weather: `<weather id>[_l{severity level}][_d][_n].png`
### Spawnpoint Icons
  - `0` - without TTH
  - `1` - with TTH
### Device Icons
  - `0` - offline
  - `1` - online
### Misc Icons
  - Folder to for any icons that don't fit any category and do not pose the need for additional category.
  - Following files are required:
    - `0.png`
    - `1500.png`
    - `2500.png`
    - `500.png`
    - `ar.png`
    - `ex.png`
    - `first.png`
    - `grass.png`
    - `second.png`
    - `sparkles.png`
    - `sponsor.png`
    - `third.png`
### Station Icons
  - station: `0.png`

## Credits:  
- [Mygod](https://github.com/Mygod/pokemon-icon-postprocessor) for basic concept
