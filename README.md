Use string:split("||") to get a table of all the emotes.

Example:

```lua
local string1 = game:HttpGet('https://raw.githubusercontent.com/antonl000/AllRobloxEmotesID/main/ids.lua',true)

local table1 = string1:split("||")
local newtable = { }

local x = 0

for _, v in pairs(table1) do
	if tonumber(v) ~= nil then
		table.insert(newtable, v)
	end
end

for _, v in pairs(newtable) do
	print(v)
end
```
