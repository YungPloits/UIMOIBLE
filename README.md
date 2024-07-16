# GETTING THE UI READY
```lua
local Lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/YungPloits/UIMOIBLE/main/ui",true))()
local Table = {}
local window = Lib:CreateWindow("CustomZyro")
```
# Creating Section
```lua
window:Section("Section")
```
# Creating Button
```lua
window:Button("Button",function()
   print("Nice")
end)
```
# Creating Toggle
```lua
window:Toggle("Toggle",{location = Table, flag = "Toggle"},function()
   print(Table["Toggle"])
end)
```
# Creating Slider
```lua
window:Slider("Slider",{location = Table, min = 1, max = 64, default = 32, precise = true --[[ 0.00 instead of 0 ]], flag = "Slider"},function()
   print(Table["Slider"])
end)
```
# Creating Dropdown
```lua
window:Dropdown("Dropdown",{location = Table,flag = "Dropdown",search = true --[[AddsSearchBar]], list = {"1","2","3","4","5","6","7","8","9","0"} --[[Wont work when PlayerList = true]], PlayerList = true --[[ Turns the list into the players in the server ]]},function()
   print(Table["Dropdown"])
end)
```
# Creating Keybind
```lua
window:Bind("KeyBind",{location = Table, flag = "KeyBind", default = Enum.KeyCode.B},function() -- Automatically stops when the gui is removed
   print(Table["KeyBind"])
end)
```
# Creating TextNUMBERBox
```lua
window:Box("Box",{location = Table,flag = "Box", type = "number" --[[ Only Numbers automatically on false ]], hold = "Numbers" --[[ PlaceHolderText ]]},function()
   print(Table["Box"])
end)
```
# Creating ColorPicker
```lua
window:Search(Color3.fromRGB(255,0,255) --[[nil = Yellow]]) -- Ez searcher for if you have a lot of things
window:String({string = "String"})
```
