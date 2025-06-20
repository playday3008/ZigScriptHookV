# ZigScriptHookV

ScriptHookV wrapper for Zig.

## Usage

Add this module as a dependency to your Zig project. You can do this by adding the following to your `build.zig` file:

```zig
/// build.zig
// ...
const lib = b.addLibrary(.{ ... }); // Your library configuration

const script_hook_v = b.dependency(
    "ZigScriptHookV",
    .{
        .target = target,
        .optimize = optimize,
    },
);
lib.root_module.addImport(
    "ScriptHookV",
    script_hook_v.module("ZigScriptHookV"),
);
// ...
```

Then you can use the `ScriptHookV` module in your Zig code:

```zig
const ScriptHookV = @import("ScriptHookV");
```

With:

<details><summary>Enums</summary>
<p>

```zig
_ = ScriptHookV.Enums.eAudioFlag;
_ = ScriptHookV.Enums.eBlipColor;
_ = ScriptHookV.Enums.eBlipSprite;
_ = ScriptHookV.Enums.eCameraShake;
_ = ScriptHookV.Enums.eControl;
_ = ScriptHookV.Enums.eRadioStation;
_ = ScriptHookV.Enums.eWindowTitle;
_ = ScriptHookV.Enums.eGender;
_ = ScriptHookV.Enums.eDrivingStyle;
_ = ScriptHookV.Enums.eBone;
_ = ScriptHookV.Enums.eFiringPattern;
_ = ScriptHookV.Enums.eFont;
_ = ScriptHookV.Enums.eVehicleColor;
_ = ScriptHookV.Enums.eVehicleDoor;
_ = ScriptHookV.Enums.eVehicleLockStatus;
_ = ScriptHookV.Enums.eVehicleLandingGear;
_ = ScriptHookV.Enums.eVehicleMod;
_ = ScriptHookV.Enums.eVehicleNeonLight;
_ = ScriptHookV.Enums.eVehicleRoofState;
_ = ScriptHookV.Enums.eVehicleSeat;
_ = ScriptHookV.Enums.eVehicleToggleMod;
_ = ScriptHookV.Enums.eVehicleWheelType;
_ = ScriptHookV.Enums.eVehicleWindow;
_ = ScriptHookV.Enums.eVehicleWindowTint;
_ = ScriptHookV.Enums.eNumberPlateMounting;
_ = ScriptHookV.Enums.eNumberPlateType;
_ = ScriptHookV.Enums.eVehicleClass;
_ = ScriptHookV.Enums.eExplosionType;
_ = ScriptHookV.Enums.eIntersectFlags;
_ = ScriptHookV.Enums.eMarkerType;
_ = ScriptHookV.Enums.eRelationship;
_ = ScriptHookV.Enums.eRopeType;
_ = ScriptHookV.Enums.eWeapon;
_ = ScriptHookV.Enums.eWeaponGroup;
_ = ScriptHookV.Enums.eWeaponTint;
_ = ScriptHookV.Enums.ePickupType;
_ = ScriptHookV.Enums.eHudComponent;
```

</p>
</details>

<details><summary>Types</summary>
<p>

```zig
_ = ScriptHookV.Types.Void;
_ = ScriptHookV.Types.Any;
_ = ScriptHookV.Types.uint;
_ = ScriptHookV.Types.Hash;
_ = ScriptHookV.Types.Blip;
_ = ScriptHookV.Types.Cam;
_ = ScriptHookV.Types.Camera;
_ = ScriptHookV.Types.CarGenerator;
_ = ScriptHookV.Types.ColourIndex;
_ = ScriptHookV.Types.CoverPoint;
_ = ScriptHookV.Types.Entity;
_ = ScriptHookV.Types.FireId;
_ = ScriptHookV.Types.Group;
_ = ScriptHookV.Types.Interior;
_ = ScriptHookV.Types.Object;
_ = ScriptHookV.Types.Ped;
_ = ScriptHookV.Types.Pickup;
_ = ScriptHookV.Types.Player;
_ = ScriptHookV.Types.ScrHandle;
_ = ScriptHookV.Types.Sphere;
_ = ScriptHookV.Types.TaskSequence;
_ = ScriptHookV.Types.Texture;
_ = ScriptHookV.Types.TextureDict;
_ = ScriptHookV.Types.Train;
_ = ScriptHookV.Types.Vehicle;
_ = ScriptHookV.Types.Weapon;
_ = ScriptHookV.Types.Vector2;
_ = ScriptHookV.Types.Vector3;
_ = ScriptHookV.Types.Vector4;
```

</p>
</details>

<details><summary>Invoker</summary>
<p>

```zig
_ = ScriptHookV.Invoker.push;
_ = ScriptHookV.Invoker.invoke;
```

</p>
</details>

```zig
_ = ScriptHookV.createTexture;
_ = ScriptHookV.drawTexture;
_ = ScriptHookV.PresentCallback;
_ = ScriptHookV.presentCallbackRegister;
_ = ScriptHookV.presentCallbackUnregister;
_ = ScriptHookV.KeyboardHandler;
_ = ScriptHookV.keyboardHandlerRegister;
_ = ScriptHookV.keyboardHandlerUnregister;
_ = ScriptHookV.scriptWait;
_ = ScriptHookV.scriptRegister;
_ = ScriptHookV.scriptRegisterAdditionalThread;
_ = ScriptHookV.scriptUnregister;
_ = ScriptHookV._scriptUnregister; // Deprecated
_ = ScriptHookV.nativeInit;
_ = ScriptHookV.nativePush64;
_ = ScriptHookV.nativeCall;
_ = ScriptHookV.wait;
_ = ScriptHookV.terminate;
_ = ScriptHookV.getGlobalPtr;
_ = ScriptHookV.worldGetAllVehicles;
_ = ScriptHookV.worldGetAllPeds;
_ = ScriptHookV.worldGetAllObjects;
_ = ScriptHookV.worldGetAllPickups;
_ = ScriptHookV.getScriptHandleBaseAddress;
_ = ScriptHookV.eGameVersion;
_ = ScriptHookV.getGameVersion;
```

## Contributing

If you want to contribute to this project, feel free to open an issue or a pull request. Contributions are welcome!
