local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Tubaro Hub|Blade Ball", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})
local Tab = Window:MakeTab({
	Name = "Combat",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddButton({
	Name = "Auto Parry",
	Callback = function()
      		print("button pressed")       getgenv().config = getgenv().config or {
    hit_time = 0.7, -- // recommended 0.25 to 0.75 \ --
 
    mode = 'Always', -- // Hold , Toggle , Always \ --
    deflect_type = 'Remote', -- // Key Press , Remote \ --
    notifications = true,
    keybind = Enum.KeyCode.V
}
 
loadstring(game:HttpGet("https://raw.githubusercontent.com/Hosvile/Refinement/main/MC%3ABlade%20Ball%20Parry%20V4.0.0",true))()
  	end    
})


Tab:AddButton({
	Name = "Auto Spam",
	Callback = function()
      		print("button pressed")                                    loadstring(game:HttpGet("https://pastebin.com/raw/t2391h1A"))()
  	end    
})


Tab:AddButton({
	Name = "Hold Block for spam",
	Callback = function()
      		print("button pressed")           getgenv().SpamSpeed = 1
loadstring(game:HttpGet("https://raw.githubusercontent.com/Hosvile/Refinement/main/MC%3ABlade%20Ball%20Spam",true))()
  	end    
})

OrionLib:Init()
