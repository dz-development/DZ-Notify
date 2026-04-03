# DZ-Notify
How to add DZ-Notify to any of your existing fivem scripts

# Exports
```lua
local function Notify(msg, type)
    if type == 'success' then
        exports['DZ-Notify']:Success('Success', msg)
    elseif type == 'error' then
        exports['DZ-Notify']:Error('Error', msg)
    else
        exports['DZ-Notify']:Alert('Alert', msg)
    end
end
```

