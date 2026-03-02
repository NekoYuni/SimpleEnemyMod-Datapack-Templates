# SimpleEnemyMod-Datapack-Templates
Example datapack for creating custom unit loadouts.

### What is this?
With this datapack, you can modify or extend the default unit loadouts.

***

### Override or Add Weapons? 
- If you want to override the default loadouts, you need to name the file:
`loadouts.json`
- If you want to **add new loadouts while keeping the default ones**, you can use any other filename.

Make sure your ZIP file follows this folder path:

`data/simpleenemymod/unit_loadouts/[type of units]/loadouts.json`

[type of units]
- `pmc_units`
- `ru_units`
- `us_units`

Then place the ZIP file inside:

`.minecraft/saves/[name of your world]/datapacks`

***

### How to Create New Loadouts?
Create a `.json` file using the following structure:

- A root object named "loadouts"
- Inside it, add a reference name for your loadout
  
Then define:

- gun_id
- ammo_count
- fire_mode
- scope_id (optional)
- muzzle_id (optional)
- grip_id (optional)

### Examples
 
```
{
  "loadouts": {
    "rpk": {
      "gun_id": "tacz:rpk",
      "ammo_count": 40,
      "fire_mode": "AUTO",
      "scope_id": "tacz:sight_t2",
      "muzzle_id": "tacz:muzzle_silencer_ursus"
    },

    "type_81": {
      "gun_id": "tacz:type_81",
      "ammo_count": 30,
      "fire_mode": "SEMI"
    },

    "ak47": {
      "gun_id": "tacz:ak47",
      "ammo_count": 30,
      "fire_mode": "SEMI",
      "scope_id": "tacz:sight_t2"
    }
  }
}
```
