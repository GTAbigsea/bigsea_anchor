## 已锚定

## 描述

返回当前船只是否可以停泊，车辆是否需要通过。

## 参数

* **车辆**：当前车辆

## 例子


```lua
    local IsAnchored = exports.bigsea_anchor:IsAnchored(GetVehiclePedIsIn(PlayerPedId(), true))

    if IsAnchored then
        -- is anchored
        return
    end

    -- isn't anchored
    return false

```
