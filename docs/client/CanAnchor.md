
## CanAnchor

## Description

返回当前船只是否可以停泊，车辆是否需要通过。

## Parameters

* **vehicle**: 当前车辆

## Examples

```lua
    local ped = PlayerPedId()
    local vehicle = GetVehiclePedIsIn(ped, true)
    local isDriver = GetPedInVehicleSeat(vehicle, -1) == ped


    local canAnchor = exports.bigsea_anchor:CanAnchor(vehicle)

    if canAnchor and isDriver then
        -- 可以锚定
        return
    end

    -- 无法锚定
    return false

```
