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
  - mega_resouce
  - Subfolders can be added without approval as long as the follow exact [Proto names](https://github.com/Furtif/POGOProtos/blob/old_master/src/POGOProtos/Data/Quests/QuestReward.proto#L26) ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/797834489861767178))
- team
- type
- weather
- misc

## UIcons Object Naming

To provide each project with expectable file name it will be fixed in the standard 

### Pokemon icons ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/804151316460601375))
- ~~Hyphen~~, ### Underscore ### or ~~Nothing~~ ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/805465450863394847))
- Order of variables ([Approving Poll](https://discord.com/channels/795728654566817812/797833971332415529/805466387342426114))

  - `<pokemon id>[_e<temp evolution id>][_f<form id>][_c<costume id>][_g<gender id>][_s].png`
    - Example: `3.png` Regular Venusaur
    - Example: `3_e1_s.png` Mega Venusaur Shiny
    - Example: `3_f950.png` Venusaur Clone Form

### Reward icons ( ALL BELOW IS A PROPOSAL )
  - item: `<item id>[_a<ammount>].png`
  - stardust:`<amount>.png`
  - mega_resouce:`<pokemon id>.png`
### Gym icons
  - gym: `<team id>[_t<trainer count>][_b{battle}][_e{ex}].png`  (`_b` `_e` flag optional)
### Raid icons
  - raid: `<egg level>[-h{hatched}][_e {ex}].png` (`_h` `_e` flag optional)
### Invasion icons
  - invasion: `<grunt id>.png`
### Pokestop icons
  - pokestop: `<lure id**>[_g<grunt id>][_q<quest id>].png
  ** Not lured is ID `0` further follow proto's
  *** To be considered `[_s{small}][_b{big}]` (Small icons minimal details eg marker use. Big icons full details eg label notification use)
### Team Icons
  - team: `<team id>.png` (Team badges not to be confused with Gym icons)
### Type Icons
  - type: `<type id>.png` 
### Weather Icons
  - weather: `<weather id>[_l<severity level>].png`
### Misc Icons
  - Folder to for any icons that dont fit any category and do not pose the need for additional category.
