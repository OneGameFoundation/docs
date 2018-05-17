---
layout: single
sidebar:
  nav: "docs"
---

### Scripts
-----------------------------

**What are scripts?**
Scripts help developers define customized rules on their land parcel as well as generate new games. Developers can use scripts to override the default physical rules in the platform, create own plots or stories, make None Player Characters (NPCs) come alive through AI algorithms, or define the
starting and ending conditions of their games on their land.


**What scripts can you use?**
Developers can use scripts to override the default physical
rules in the One Game platform, create own plots or stories, make None Player Characters (NPCs) come alive through AI algorithms, or define the starting and ending conditions of their games on their land.

**Example of a Lua Script**
For example below is a simple Lua script for simple chaser. When you attach this script to an entity, it will move the entity towards the game player.

```lua
speed = 2

function start()

end

function update(dt)
  -- Fetch the target
  local target = player.position

  -- Rotate the entity towards the player
  entity.RotateTowards(target, dt * 2)

  -- Move towards the target
  local pos = entity.position
  pos = pos + entity.forward * dt * speed
  entity.position = pos
end
```

**Can developers make their scripts?**
Yes, we will open source many scripts and we will allow developers to write embeddable Lua scripts which can extend or modify our open source scripts or write these scripts entirely from scratch.
