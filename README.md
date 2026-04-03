# DZ-Notify
How to add DZ-Notify to your existing FiveM scripts.

The resource name **must** stay as `DZ-Notify`.

## Exports
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

# Usage in other scripts
```lua
Notify('Action completed successfully', 'success')
Notify('Action failed', 'error')
Notify('You cannot do this here', 'alert')
```
