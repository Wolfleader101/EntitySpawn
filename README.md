## Permissions

* `entityspawn.use` -- Allows player to throw projectiles to spawn entities

## Configuration

The plugins config allows for you to have as little or many projectiles as you want.

* `Spawns` - Contains the objects. Each projectile should be it's own object.
* `Enabled` - Enables or disables the projectile
* `permission` - Individual permission for each item
* `prefabs` - An array of prefabs it can spawn in (defaults to first one if random is disabled)
* `random` - Get random prefab from the array


Example Config:
```json
{
  "Spawns": {
    "snowball": {
      "enabled": false,
      "permission": "entityspawn.snowball",
      "prefabs": [
        "assets/prefabs/npc/scientist/htn/scientist_full_any.prefab"
      ],
      "random": false
    },
	"machete": {
      "enabled": true,
	  "permission": "entityspawn.machete",
      "prefabs": [
        "assets/prefabs/npc/scientist/htn/scientist_full_any.prefab",
        "assets/rust.ai/agents/npcplayer/humannpc/heavyscientist/heavyscientist.prefab"
      ],
      "random": true
    }
  }
}
```