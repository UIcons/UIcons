# UIcons Universal Icons

UIcons is an attempt to create a universal and cooperative standard for Icons used across different PoGo projects. Full standard and its changes will be discussed openly and to every creator adopting the standard.

Join the discussion @ [Discord](https://discord.gg/cG8JwrJB6Z)

## Repo's that have adopted or have agreed to adopt

* [nileplumb](https://github.com/nileplumb) Shuffle and Home iconsets
* [whitewillem](https://github.com/whitewillem/PogoAssets) Ingame and Ingame outline iconsets
* [geekygreek7](https://github.com/geekygreek7) Shuffle shiny split iconset (**currently Pull Request)

### Main folder structure approved

- gym
- raid
  - egg 
- invasion
  - grunts
  - display types
- pokemon
- pokestop
- reward
  - item
  - stardust
  - candy
  - xl_candy
  - mega_resource
  - Subfolders can be added without approval as long as the follow exact [Proto names](https://github.com/Furtif/POGOProtos/blob/a53979d6bba81df45b1f09f7c1aa8185cb999959/base/base.proto#L16087)
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

  - `<pokemon id>[_e{temp evolution id}][_f{form id}][_c{costume id}][_g{gender id}][_s{shiny}].png`
    - Example: `3.png` Regular Venusaur
    - Example: `3_e1_s.png` Mega Venusaur Shiny
    - Example: `3_f950.png` Venusaur Clone Form

### Reward icons
  - item: `<item id>[_a{amount}].png`
  - stardust:`<amount>.png`
  - mega_resouce:`<pokemon id>[_a{amount}].png`
  - candy: `<pokemon id>[_a{amount}].png`
  - xl_candy:`<pokemon id>[_a{amount}].png`
### Gym icons
  - gym: `<team id>[_t{trainer count}][_b][_ex][_ar].png` (`_b` in active battle, `_ex` ex gym, `_ar` ar eligible (no flag means false))
### Raid icons 
  - egg: `<egg level>[_h][_ex].png` (`_h` hatched egg `_ex` ex gym (no flag means false))
### Invasion icons
  - invasion: `<grunt id>.png`
  - display types: `<display type>.png`
### Pokestop icons
  - pokestop: `<lure id**>[_g][_d][_q{with_ar}][_ar].png` ( `_g` grunt invasion active, `_d` display type invasion active, `_q` quest active, `_ar` ar eligible ) images from invasion and reward folder can be used as overlay
  - ** Not lured is ID `0` further follow proto's
  - Upcoming Pokestop levels might change perspective on pokestop icon naming.. TBC
  - `_q`: any or both AR and non-AR quests are active 
  - `_q0`: Non-AR quest active
  - `_q1`: AR quest active
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

## Credits:  
- [Mygod](https://github.com/Mygod/pokemon-icon-postprocessor) for basic concept
