# loaf_headshot_base64
Convert FiveM ped headshot / mugshot to base64

## Usage
Here's an example usage of getting the base64 image of the local player ped
```lua
CreateThread(function()
    local result = exports["loaf_headshot_base64"]:getBase64(PlayerPedId())
    if result.success then
        print("^2Base64:^0",result.base64)
    else
        print("^1Error:^0",result.error)
    end
end)
```
