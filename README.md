# rbx-animation-lib
Library to play any animation in game with an executor.

Works virtually any roblox game.

# Example
Using an punch animation.
```lua
-- Requires the AnimationLib MainModule from roblox
local AnimationLib = require(108128765219659)

-- Gets an serialized example animation from the project repo
local animation = game:HttpGet("https://raw.githubusercontent.com/loglizzy/rbx-animation-lib/refs/heads/main/animations/Rock%20Breaking%20Punch.txt")

-- Loads & play the animation
animation = AnimationLib.UnserializeToAnimation(workspace.Rig, animation)
animation:Play()
```

To use another animation just grab (Animation serializer script)[https://github.com/loglizzy/rbx-animation-lib/blob/main/Animation%20serializer%20script.rbxm] and run it in a roblox studio place.

Once you have the animation you can upload it somewhere like [https://pastebin.com/] and load it like in the example by just applying your uploaded animation url.
