# server-config-guide
Guide on how to install and config a new server. Also keeps track of the changes we did to the servers over time, clearly communicating differing server settings to the players.

This repository will also be reworked soon!

## Survival (Minecraft Empires)
### server.properties
```
allow-nether=true
difficulty=hard
enable-command-block=false
enforce-secure-profile=true
gamemode=survival
generate-structures=true
level-name=world
level-seed=(Seed)
level-type=minecraft\:normal
log-ips=false
max-players=200
network-compression-threshold=256
online-mode=false
region-file-compression=lz4
simulation-distance=10
view-distance=10
spawn-animals=true
spawn-monsters=true
spawn-npcs=true
spawn-protection=0
```

### bukkit.yml
```
allow-end: false
use-map-color-cache: true
spawn-limits:
  monsters: 70
  animals: 10
  water-animals: 5
  water-ambient: 20
  water-underground-creature: 5
  axolotls: 5
  ambient: 15
chunk-gc:
  period-in-ticks: 600
ticks-per:
  animal-spawns: 400
  monster-spawns: 1
  water-spawns: 1
  water-ambient-spawns: 1
  water-underground-creature-spawns: 1
  axolotl-spawns: 1
  ambient-spawns: 1
  autosave: 6000
```

### spigot.yml
```
advancements:
  disable-saving: true
  disabled:
  - minecraft:story/disabled
bungeecord: false
netty-threads: 4
log-villager-deaths: false
log-named-deaths: true
players:
  disable-saving: true
stats:
  disable-saving: true
world-settings:
  below-zero-generation-in-existing-chunks: true
  view-distance: default
  simulation-distance: default
  merge-radius:
      item: 3.5
      exp: 4.0
  mob-spawn-range: 8
  nerf-spawner-mobs: true
  wither-spawn-sound-radius: 150
  end-portal-sound-radius: 150
  dragon-death-sound-radius: 150
  ticks-per:
      hopper-transfer: 8
      hopper-check: 1
  hopper-amount: 1
  entity-activation-range:
    tick-inactive-villagers: false
    ignore-spectators: true
```

### paper-world-defaults.yml
```
anticheat:
  anti-xray:
    enabled: true
    engine-mode: 3
    hidden-blocks:
    - coal_ore
    - deepslate_coal_ore
    - copper_ore
    - deepslate_copper_ore
    - raw_copper_block
    - diamond_ore
    - deepslate_diamond_ore
    - gold_ore
    - deepslate_gold_ore
    - iron_ore
    - deepslate_iron_ore
    - raw_iron_block
    - lapis_ore
    - deepslate_lapis_ore
    - redstone_ore
    - deepslate_redstone_ore
    lava-obscures: false
    max-block-height: 320
    replacement-blocks:
    - diamond_ore
    - deepslate_diamond_ore
    - amethyst_block
    - copper_ore
    - deepslate_copper_ore
    - raw_copper_block
    - andesite
    - budding_amethyst
    - calcite
    - coal_ore
    - deepslate_coal_ore
    - deepslate
    - diorite
    - dirt
    - emerald_ore
    - deepslate_emerald_ore
    - granite
    - gravel
    - oak_planks
    - smooth_basalt
    - stone
    - tuff
    update-radius: 3
    use-permission: false
  obfuscation:
    items:
      hide-durability: false
      hide-itemmeta: false
      hide-itemmeta-with-visual-effects: false
tick-rates:
  behavior:
    villager:
      validatenearbypoi: -1
  container-update: 1
  dry-farmland: 1
  grass-spread: 4
  mob-spawner: 2
  sensor:
    villager:
      secondarypoisensor: 40
  wet-farmland: 1
misc:
  alternate-current-update-order: HORIZONTAL_FIRST_OUTWARD
  disable-end-credits: true
  disable-relative-projectile-velocity: false
  disable-sprint-interruption-on-attack: false
  light-queue-size: 20
  max-leash-distance: default
  redstone-implementation: ALTERNATE_CURRENT
  shield-blocking-delay: 5
  show-sign-click-command-failure-msgs-to-player: false
  update-pathfinding-on-block-update: true
hopper:
  cooldown-when-full: true
  disable-move-event: true
```
