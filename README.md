# rbx-animation-lib
Play any animation in game with any executor.

Thanks to the guy who made the [KeyframeSequence to Animation converter](https://devforum.roblox.com/t/keyframesequance-to-animation-v4/3137384).

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

# Guide
1. To use an animation just place the [Animation serializer script](https://github.com/loglizzy/rbx-animation-lib/blob/main/Animation%20serializer%20script.rbxm) in a roblox studio place, put your animation KeyframeSequence inside the script, run it and check the console(F9) for the results.

2. Once you have the animation you can upload the raw result to somewhere like [pastebin.com](https://pastebin.com/) and load it like in the example by just switching it to your uploaded animation url.
```lua
local animation = game:HttpGet("YOUR_ANIMATION_URL_HERE")
-- ... do just like in the example
```

Got any bugs? Open an issue at this repository and i may fix it in the same day.
