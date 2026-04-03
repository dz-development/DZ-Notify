# DZ-Notify
How to add DZ-Notify to any of your existing fivem scripts

The name of the Resource **MUST** stay as 'DZ-Notify'

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

# Useage in other scripts
```lua
Notify('Vehicle spawned', 'success')
Notify('Vehicle despawned', 'error')
Notify('You are now in the car', 'alert')
```
