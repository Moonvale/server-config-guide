# server-config-guide
Guide on how to install and config a new server


## Survival
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
```
