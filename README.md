# ZigScriptHookV

Zig wrapper for ScriptHookV.

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
_ = ScriptHookV.Enums.AudioFlag;
_ = ScriptHookV.Enums.BlipColor;
_ = ScriptHookV.Enums.BlipSprite;
_ = ScriptHookV.Enums.CameraShake;
_ = ScriptHookV.Enums.Control;
_ = ScriptHookV.Enums.RadioStation;
_ = ScriptHookV.Enums.WindowTitle;
_ = ScriptHookV.Enums.Gender;
_ = ScriptHookV.Enums.DrivingStyle;
_ = ScriptHookV.Enums.Bone;
_ = ScriptHookV.Enums.FiringPattern;
_ = ScriptHookV.Enums.Font;
_ = ScriptHookV.Enums.VehicleColor;
_ = ScriptHookV.Enums.VehicleDoor;
_ = ScriptHookV.Enums.VehicleLockStatus;
_ = ScriptHookV.Enums.VehicleLandingGear;
_ = ScriptHookV.Enums.VehicleMod;
_ = ScriptHookV.Enums.VehicleNeonLight;
_ = ScriptHookV.Enums.VehicleRoofState;
_ = ScriptHookV.Enums.VehicleSeat;
_ = ScriptHookV.Enums.VehicleToggleMod;
_ = ScriptHookV.Enums.VehicleWheelType;
_ = ScriptHookV.Enums.VehicleWindow;
_ = ScriptHookV.Enums.VehicleWindowTint;
_ = ScriptHookV.Enums.NumberPlateMounting;
_ = ScriptHookV.Enums.NumberPlateType;
_ = ScriptHookV.Enums.VehicleClass;
_ = ScriptHookV.Enums.ExplosionType;
_ = ScriptHookV.Enums.IntersectFlags;
_ = ScriptHookV.Enums.MarkerType;
_ = ScriptHookV.Enums.Relationship;
_ = ScriptHookV.Enums.RopeType;
_ = ScriptHookV.Enums.Weapon;
_ = ScriptHookV.Enums.WeaponGroup;
_ = ScriptHookV.Enums.WeaponTint;
_ = ScriptHookV.Enums.PickupType;
_ = ScriptHookV.Enums.HudComponent;
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

<details><summary>Functions</summary>
<p>

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

</p>
</details>

## Contributing

If you want to contribute to this project, feel free to open an issue or a pull request. Contributions are welcome!
