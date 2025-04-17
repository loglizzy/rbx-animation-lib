# rbx-animation-lib
Library to play any animation in game with an executor.

Works virtually any roblox game.

# Example
Using an punch animation.
```lua
local AnimationLib = require(108128765219659)

-- Gets an serialized animation from the project repo
local animation = game:HttpGet("https://raw.githubusercontent.com/loglizzy/rbx-animation-lib/refs/heads/main/animations/Rock%20Breaking%20Punch.txt")

-- Loads & play the animation
animation = AnimationLib.UnserializeToAnimation(workspace.Rig, animation)
animation:Play()
```
