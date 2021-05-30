# UIcons Universal Icons

UIcons is an attempt to create a universal and cooperative standard for Icons used across different PoGo projects. Full standard and its changes will be discussed openly and to every creator adopting the standard.

Join the discussion @ [Discord](https://discord.gg/cG8JwrJB6Z)

## UIcons folder structure

To provide each project with expectable folder structure it will be fixed in the standard 

### Main folder structure approved ([Approving Poll](https://discord.com/channels/795728654566817812/795778114139586590/796050026689855538))

- gym
- raid
- invasion
- pokemon
- pokestop
- reward  ([Approving Poll](https://discord.com/channels/795728654566817812/795778114139586590/796468427228315648))
  - item
  - stardust
  - mega_resource
  - Subfolders can be added without approval as long as the follow exact [Proto names](https://github.com/Furtif/POGOProtos/blob/a53979d6bba81df45b1f09f7c1aa8185cb999959/base/base.proto#L16087) ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/797834489861767178))
- team
- type
- weather
- misc

## UIcons Object Naming

To provide each project with expectable file name it will be fixed in the standard 

### Mandatory image keys are wrapped in `< >`
### Optional flags are wrapped in `{ }`

### Pokemon icons ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/804151316460601375))
- ~~Hyphen~~, ### Underscore ### or ~~Nothing~~ ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/805465450863394847))
- Order of variables ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/805466387342426114))

  - `<pokemon id>[_e{temp evolution id}][_f{form id}][_c{costume id}][_g{gender id}][_s{shiny}].png`
    - Example: `3.png` Regular Venusaur
    - Example: `3_e1_s.png` Mega Venusaur Shiny
    - Example: `3_f950.png` Venusaur Clone Form

### Reward icons ( ALL BELOW IS A PROPOSAL )
  - item: `<item id>[_a{amount}].png`
  - stardust:`<amount>.png`
  - mega_resouce:`<pokemon id>.png`
### Gym icons
  - gym: `<team id>[_t{trainer count}][_b][_ex].png` (`_b` in active battle `_ex` ex gym (no flag means false))
### Raid icons
  - raid: `<egg level>[_h][_ex].png` (`_h` hatched egg `_ex` ex gym (no flag means false))
### Invasion icons
  - invasion: `<grunt id>.png`
### Pokestop icons
  - pokestop: `<lure id**>[_i][_q].png` ( `_i` invasion active `_q` quest active ) images from invasion and reward folder can be used as overlay
  - ** Not lured is ID `0` further follow proto's
  - Upcoming Pokestop levels might change perspective on pokestop icon naming.. TBC
### Team Icons
  - team: `<team id>.png` (Team badges not to be confused with Gym icons)
### Type Icons
  - type: `<type id>.png` 
### Weather Icons
  - weather: `<weather id>[_l{severity level}].png`
### Misc Icons
  - Folder to for any icons that dont fit any category and do not pose the need for additional category.
