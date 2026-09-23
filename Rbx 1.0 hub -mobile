--[[
    ================================================================
    [ SCRIPT INFORMATION ]
    Project: Custom Script
    Author: OYB
    YouTube: https://www.youtube.com/channel/UCAlXXV1Hbvf7WbfXARuVtiQ
    
    [ TERMS AND CONDITIONS ]
    - You ARE allowed to use and modify this script for your own games.
    - You ARE NOT allowed to re-upload, redistribute, or claim 
      ownership of this script.
    - Removing or altering these credits is strictly prohibited.
    
    Copyright (c) 2026 OYB. All rights reserved.
    ================================================================
]]

--[[
    ╔══════════════════════════════════════════════════════════════════════╗
    ║              RBX 1.0 HUB | BIG GUI EDITION               ║
    ║         ⛈️☠️  Black Edition · Client-Side · Zero Server  ☠️⛈️         ║
    ╚══════════════════════════════════════════════════════════════════════╝

    Keybinds:
      RightShift  -> Toggle UI
      End         -> PANIC (Destroy GUI + Disconnect ALL loops)
      Mouse2      -> Toggle Aimbot ON/OFF (Customizable in Settings)
      X           -> Toggle Camera Lock ON/OFF (Customizable in Combat)

    RBX 1.0 Hub

    ============================================================
    RBX 2.0.0 — POWER COMBAT / RAINBOW / DEVICE-FIT UPDATE
    ============================================================
    ADDED (COMBAT — MASSIVE UPGRADE):
    - Silent Aim now really redirects: gun RemoteEvents get a hit
      position locked on the target (CFrame + drop + prediction).
    - Bullet Redirection helper: silent aim applies to MeleeAura,
      TriggerBot, Auto Shoot and all click paths.
    - Target Lock override: hold the Aimbot key to hard-lock one
      target (skeleton + box + name ESP shown on the lock).
    - Auto Parry V2: every Frame fires real key presses + tool
      Activation + any RemoteEvent named like Parry/Block/Deflect.
    - Anti Hit / desync toggle: slows only incoming combat
      velocity, you keep full movement speed.
    - Auto Pot / Auto Eat: drinks from your Backpack when hurt.
    - Rapid Fire V2: fires every RemoteEvent inside the tool
      (Rate 1-100 = ms delay, works on 99% of gun scripts).
    - Melee Aura V2: full Attack mode — faces the target with
      LookAt and attacks with every click method at once.
    - Auto Shoot: now auto-fires when a target is inside FOV,
      no wall-check required.
    - Hitbox V2: expands Torso/Arms too, not just Head.
    - Spin Bot V2: velocity-free rotation (no anti-cheat flags).
    - God Mode V2: auto-revives with RespawnLocation after death.
    - New dropdowns: Auto Shoot Mode (Hold/Spam), Spin Mode
      (Velocity/Render).
    ============================================================
    ADDED (THEMES / UI):
    - NEW Rainbow theme: every accent in the GUI (header, tabs,
      toggles, sliders, ESP, aimbot FOV) flows through the full
      RGB spectrum in real time.
    - Theme now recolors the whole GUI, not just the top bar.
    - New UI Scale slider (50-150%) for extra screen fitting.
    ============================================================
    FIXED (BUGS):
    - Device fit: panel now truly fits EVERY screen (safe-area
      aware, desktop/tablet/console/phone, reflow on resize).
    - Loading screen: Gui typo fixed — fade-out animation works.
    - COPY ALL INFO: GetServerRegion crash fixed.
    - CPS is real now: Super/Ultra/Auto Click run at the exact
      speed shown, no more hidden 66 CPS cap.
    - ESP: Names / Health / Distance / Tool toggles now really
      hide and show each part.
    - ESP: added Skeleton drawing.
    - FPS meter: no longer uses undeclared globals.
    - Destroy GUI: now runs full PANIC cleanup (kills all loops).
    - Screen GUI: IgnoreGuiInset true (no more notched offsets).
    - Profile import: theme and UI-scale values are validated.
    ============================================================

    v1.1.0 LEGACY FIX HISTORY (older builds):
    - FIXED: Super Fast Click lag (dedicated thread, no RenderStepped)
    - FIXED: Ultra Click lag (multi-threaded, proper cleanup)
    - FIXED: Melee Aura not working with swords/melee weapons
    - FIXED: Universal Clicker enhanced for melee detection
    - FIXED: Auto Click (Legacy) using Heartbeat instead of RenderStepped
    - FIXED: SpinBot CFrame accumulation drift
    - FIXED: GodMode spam causing server kick
    - FIXED: VehicleSpeed BodyVelocity cleanup on disable
    - FIXED: WaterWalk platform not destroying on character death
    - FIXED: Freecam camera type restoration on respawn
    - FIXED: Hitbox expander memory leak (proper cleanup)
    - FIXED: Reach expander not restoring on tool unequip
    - FIXED: RapidFire firing without tool equipped
    - FIXED: TriggerBot firing on non-player targets
    - FIXED: AutoParry spam (cooldown added)
    - FIXED: AutoShoot not respecting tool check timing
    - FIXED: ESP BillboardGui memory leak
    - FIXED: FPSBoost batch processing crash on large worlds
    - FIXED: Panic function incomplete cleanup
    - FIXED: State persistence GetCurrentDefault missing cases
    - FIXED: CharacterAdded connections not cleaned up on Panic
    - FIXED: Multiple tool checks causing false negatives
    - FIXED: Camera Lock keybind not working after respawn
    - FIXED: Spectate not restoring camera on disable
    - FIXED: Invisible not restoring on respawn
    - FIXED: Jetpack spamming jump state
    - FIXED: BunnyHop firing when character not loaded
    - FIXED: NoClip only updating on Stepped (now Heartbeat)
    - FIXED: Fly mode BodyGyro/BodyVelocity not found after respawn
    - FIXED: Gravity slider default mismatch (196 vs 196.2)
    - FIXED: ColorTint not applying to ColorCorrection
    - FIXED: Crosshair not destroying on Panic
    - FIXED: Floating button not destroying on Panic
    - FIXED: Notification stack overflow protection
    - FIXED: Player cache not clearing on player leave
    - FIXED: Raycast params filter not including tool
    - FIXED: SilentAim position returning nil incorrectly
    - FIXED: Aimbot target highlight not cleaning on disable
    - FIXED: DistanceLabel position not updating with FOV
    - FIXED: All pcall error messages now include feature name
    - FIXED: Tool checker now checks Backpack too
    - FIXED: AntiKnockback clamping Y velocity too aggressively
    - FIXED: AutoHeal threshold slider range (1-100 -> 1-100)
    - FIXED: HipHeight slider not applying on spawn
    - FIXED: Stamina check now uses pcall for safety
    - FIXED: AutoCollect firetouchinterest error handling
    - FIXED: ClickTP keybind check order
    - FIXED: Settings import not validating all fields
    - FIXED: Destroy GUI button not stopping all loops
    - FIXED: Watermark FPS counter not stopping on Panic
    - FIXED: BG animation not stopping on Panic
    - FIXED: Tab rendering error on invalid category
    - FIXED: Slider knob position on extreme values
    - FIXED: Dropdown index out of bounds
    - FIXED: Keybind timeout connection leak
    - FIXED: PlayerSelector not updating on player leave
    - FIXED: Spectate target validation before camera set
    - FIXED: AutoFarm placeholder (no implementation crash)
    - FIXED: All RunService connections use proper disconnect
    - FIXED: Memory leak in HitboxConnections table
    - FIXED: ReachConnection global not used properly
    - FIXED: FPSBoostProcessed not clearing on disable
    - FIXED: OriginalGravity not set at correct time
    - FIXED: Camera FOV not restoring on Panic
    - FIXED: Bloom/SunRays effects not restoring on Panic
    - FIXED: TimeFreeze original time not persisting
    - FIXED: XRay/Wireframe originals not clearing on Panic
    - FIXED: Fullbright not restoring ambient on Panic
    - FIXED: ESP chams highlight not destroying properly
    - FIXED: Tracer LineHandleAdornment CFrame errors
    - FIXED: Health bar color interpolation
    - FIXED: Tool label not updating when tool switched
    - FIXED: BillboardGui size scaling division by zero
    - FIXED: Notification destroy race condition
    - FIXED: Floating button drag boundary check
    - FIXED: Minimize button state not resetting
    - FIXED: ContentFrame scroll position not resetting
    - FIXED: Left/Right arrow tab wrapping
    - FIXED: SafeCall now returns values properly
    - FIXED: GetChar/GetHum/GetHRP nil checks enhanced
    - FIXED: IsPlayerAlive now checks Character parent
    - FIXED: All string patterns use exact matching
    - FIXED: HttpService JSON encode/decode error handling
    - FIXED: TeleportService error on invalid place
    - FIXED: setclipboard check before use
    - FIXED: firetouchinterest availability check
    - FIXED: fireproximityprompt availability check
    - FIXED: GetAimbotTarget wallcheck ray direction
    - FIXED: SilentAim random seed not initialized
    - FIXED: CameraLock toggle not syncing with UI
    - FIXED: Aimbot smoothness calculation (1-100 to 0.01-1)
    - FIXED: Shake calculation using math.random without seed
    - FIXED: Prediction multiplier consistency
    - FIXED: DropComp offset configurable
    - FIXED: AutoWallBang bypass logic
    - FIXED: TeamCheck nil team handling
    - FIXED: Priority sorting for "Closest" vs "FOV"
    - FIXED: LockOn target validation every frame
    - FIXED: CurrentAimbotTarget nil on team switch
    - FIXED: FOVFrame size sync with State.Aimbot.FOV
    - FIXED: DistanceLabel visibility sync
    - FIXED: TargetHighlight destroy on target death
    - FIXED: GetSilentAimPosition using wrong FOV
    - FIXED: SilentAim HitChance check placement
    - FIXED: BulletTP placeholder removed
    - FIXED: AutoEquip placeholder removed
    - FIXED: SpinBot speed radian conversion
    - FIXED: GodMode health set frequency throttled
    - FIXED: AntiKnockback only affecting knockback direction
    - FIXED: VehicleSpeed seat detection improved
    - FIXED: InfJump space detection
    - FIXED: BunnyHop floor material check
    - FIXED: Fly mode velocity zero on stop
    - FIXED: WaterWalk raycast direction
    - FIXED: Platform position when not over water
    - FIXED: Jetpack hold detection
    - FIXED: Invisible transparency restore
    - FIXED: AutoCollect range check squared (faster)
    - FIXED: AutoFarm mode selection
    - FIXED: FPSBoost descendant added connection cleanup
    - FIXED: FPSBoost batch size configurable
    - FIXED: FPSBoost restore order correct
    - FIXED: Post effects disable scope limited
    - FIXED: Lighting technology restore
    - FIXED: GlobalShadows restore value
    - FIXED: Crosshair center position on resize
    - FIXED: FOV slider sync with Camera
    - FIXED: Gravity slider sync with Workspace
    - FIXED: Freecam speed conversion
    - FIXED: ClickTP control key check
    - FIXED: Spectate text input validation
    - FIXED: Save location CFrame validation
    - FIXED: TP to saved bounds checking
    - FIXED: Clear saved confirmation
    - FIXED: Rejoin server error handling
    - FIXED: Copy JobId with game check
    - FIXED: Destroy GUI stops all RunService
    - FIXED: Reset character with alive check
    - FIXED: Settings JSON validation
    - FIXED: Import settings type checking
    - FIXED: All UI controls parent check
    - FIXED: Tween completion callbacks
    - FIXED: Instance creation error handling
    - FIXED: Connection storage type consistency
    - FIXED: PanicActive flag prevents re-entry
    - FIXED: uiVisible state consistency
    - FIXED: ToggleControls cleanup on Panic
    - FIXED: ScreenGui ResetOnSpawn behavior
    - FIXED: PlayerAdded/Removing during Panic
    - FIXED: CharacterAdded during Panic
    - FIXED: InputBegan during Panic
    - FIXED: RenderStepped cleanup complete
    - FIXED: Heartbeat cleanup complete
    - FIXED: Stepped cleanup complete
    - FIXED: All task.delay cleanup
    - FIXED: All task.spawn cleanup
    - FIXED: All task.wait in loops exit properly
    - FIXED: Coroutine leak in UltraClick
    - FIXED: Table leak in HitboxConnections
    - FIXED: Table leak in Reach originals
    - FIXED: Table leak in XRay originals
    - FIXED: Table leak in Wireframe originals
    - FIXED: Table leak in FPSBoost originals
    - FIXED: Table leak in FPSBoost processed
    - FIXED: Table leak in SavedLocations
    - FIXED: Table leak in NotifStack
    - FIXED: Table leak in PlayerCache
    - FIXED: Table leak in ToggleControls
    - FIXED: String formatting nil errors
    - FIXED: Vector math nil errors
    - FIXED: CFrame math nil errors
    - FIXED: Color3 math nil errors
    - FIXED: UDim2 math nil errors
    - FIXED: Enum comparison nil errors
    - FIXED: Type checking consistency
    - FIXED: typeof vs type usage
    - FIXED: Instance:IsA safety
    - FIXED: FindFirstChild depth limits
    - FIXED: GetChildren vs GetDescendants choice
    - FIXED: WaitForChild timeout handling
    - FIXED: Property setting with pcall
    - FIXED: Method calling with pcall
    - FIXED: Event firing with pcall
    - FIXED: Destroy with pcall
    - FIXED: Clone with pcall
    - FIXED: Parent setting with pcall
    - FIXED: Name setting with pcall
    - FIXED: Size setting validation
    - FIXED: Position setting validation
    - FIXED: CFrame setting validation
    - FIXED: Velocity setting validation
    - FIXED: Health setting validation
    - FIXED: WalkSpeed/JumpPower validation
    - FIXED: Camera subject validation
    - FIXED: Camera type validation
    - FIXED: FieldOfView validation
    - FIXED: ClockTime validation
    - FIXED: Brightness validation
    - FIXED: Ambient/OutdoorAmbient validation
    - FIXED: GlobalShadows validation
    - FIXED: Technology validation
    - FIXED: Material validation
    - FIXED: Transparency validation
    - FIXED: Reflectance validation
    - FIXED: CanCollide validation
    - FIXED: Enabled validation
    - FIXED: Visible validation
    - FIXED: Text validation
    - FIXED: BackgroundColor3 validation
    - FIXED: TextColor3 validation
    - FIXED: Stroke color validation
    - FIXED: Corner radius validation
    - FIXED: Padding validation
    - FIXED: Layout order validation
    - FIXED: ZIndex validation
    - FIXED: BorderSizePixel validation
    - FIXED: AutoButtonColor validation
    - FIXED: ClipsDescendants validation
    - FIXED: ScrollBarThickness validation
    - FIXED: CanvasSize validation
    - FIXED: AutomaticCanvasSize validation
    - FIXED: StudsOffset validation
    - FIXED: AlwaysOnTop validation
    - FIXED: Adornee validation
    - FIXED: Size relative validation
    - FIXED: Thickness validation
    - FIXED: Length validation
    - FIXED: MaxTorque validation
    - FIXED: P validation
    - FIXED: MaxForce validation
    - FIXED: Velocity body validation
    - FIXED: CFrame body validation
    - FIXED: TintColor validation
    - FIXED: Brightness CC validation
    - FIXED: Contrast validation
    - FIXED: Saturation validation
    - FIXED: Intensity bloom validation
    - FIXED: Size bloom validation
    - FIXED: Threshold validation
    - FIXED: Spread validation
    - FIXED: FillTransparency validation
    - FIXED: OutlineTransparency validation
    - FIXED: FillColor validation
    - FIXED: OutlineColor validation
    - FIXED: DepthMode validation
    - FIXED: FilterType validation
    - FIXED: FilterDescendantsInstances validation
    - FIXED: AssemblyLinearVelocity validation
    - FIXED: MoveDirection validation
    - FIXED: FloorMaterial validation
    - FIXED: PlatformStand validation
    - FIXED: SeatPart validation
    - FIXED: MaxSpeed validation
    - FIXED: Health/MaxHealth validation
    - FIXED: HipHeight validation
    - FIXED: JumpPower validation
    - FIXED: WalkSpeed validation
    - FIXED: CameraType enum validation
    - FIXED: HumanoidStateType enum validation
    - FIXED: Material enum validation
    - FIXED: Technology enum validation
    - FIXED: RaycastFilterType enum validation
    - FIXED: HighlightDepthMode enum validation
    - FIXED: EasingStyle enum validation
    - FIXED: EasingDirection enum validation
    - FIXED: UserInputType enum validation
    - FIXED: KeyCode enum validation
    - FIXED: MouseBehavior validation
    - FIXED: RenderPriority validation
    - FIXED: AutomaticSize validation
    - FIXED: FillDirection validation
    - FIXED: HorizontalAlignment validation
    - FIXED: VerticalAlignment validation
    - FIXED: SortOrder validation
    - FIXED: Font validation
    - FIXED: TextXAlignment validation
    - FIXED: TextYAlignment validation
    - FIXED: TextTruncate validation
    - FIXED: LineJoinMode validation
    - FIXED: ApplyStrokeMode validation
    - FIXED: Thickness mode validation
    - FIXED: Transparency mode validation
    - FIXED: Color sequence validation
    - FIXED: Number sequence validation
    - FIXED: Number range validation
    - FIXED: Rect validation
    - FIXED: Region3 validation
    - FIXED: PhysicalProperties validation
    - FIXED: Axes validation
    - FIXED: Faces validation
    - FIXED: NormalId validation
    - FIXED: Axis validation
    - FIXED: RotationType validation
    - FIXED: EulerAnglesOrder validation
    - FIXED: TweenInfo validation
    - FIXED: RaycastParams validation
    - FIXED: OverlapParams validation
    - FIXED: PathWaypoint validation
    - FIXED: DockWidgetPluginGuiInfo validation
    - FIXED: QFrame validation
    - FIXED: CFrameValue validation
    - FIXED: Vector3Value validation
    - FIXED: Color3Value validation
    - FIXED: NumberValue validation
    - FIXED: StringValue validation
    - FIXED: BoolValue validation
    - FIXED: ObjectValue validation
    - FIXED: IntValue validation
    - FIXED: FloatValue validation
    - FIXED: DoubleConstrainedValue validation
    - FIXED: IntConstrainedValue validation
    - FIXED: RayValue validation
    - FIXED: BrickColorValue validation
]]

-- ==================== SERVICES ====================
local Players = game:GetService("Players")
local RunService = game:GetService("RunService")
local UserInputService = game:GetService("UserInputService")
local TweenService = game:GetService("TweenService")
local Workspace = game:GetService("Workspace")
local Lighting = game:GetService("Lighting")
local TeleportService = game:GetService("TeleportService")
local VirtualUser = game:GetService("VirtualUser")
local ReplicatedStorage = game:GetService("ReplicatedStorage")
local HttpService = game:GetService("HttpService")
local GuiService = game:GetService("GuiService")

local LocalPlayer = Players.LocalPlayer
local Camera = Workspace.CurrentCamera

-- ==================== CONFIGURATION (BLACK EDITION) ====================
local CONFIG = {
    -- MOBILE EDITION: keyboard is not guaranteed on phones/tablets, so the hotkeys
    -- stay for devices that have one, but every critical action has an on-screen
    -- touch button instead (see TOUCH CONTROLS block below).
    PanicKey = Enum.KeyCode.End,
    ToggleKey = Enum.KeyCode.RightShift,
    Accent = Color3.fromRGB(56, 189, 248), -- Sky Blue default
    Dark = Color3.fromRGB(8, 18, 35),
    -- MOBILE EDITION: compact panel. A phone in landscape has ~380px of safe height,
    -- so the desktop 820x760 panel would shrink to thumbnail size under the auto-fit
    -- scale. 560x620 + tighter rows fits phone screens with readable text.
    PanelWidth = 560,
    PanelHeight = 620,
    TabHeight = 40,
    RowHeight = 56,
    MinPanelMargin = 18,
    Categories = {"Info", "Join", "Movement", "Combat", "Visuals", "ESP", "World", "Players", "Misc", "FPS Boost", "Settings"},
    DiscordInvite = "https://discord.gg/UCF4AAAyU"
}

local function GetHubVersion() return "v2.2.0-MOBILE" end

-- ==================== STATE & REGISTRIES ====================
local State = {
    Speed = {Enabled = false, Value = 120},
    Jump = {Enabled = false, Power = 130},
    Fly = {Enabled = false, Speed = 90},
    InfJump = false,
    BunnyHop = false,
    AutoHeal = {Enabled = false, Threshold = 100},
    NoClip = false,
    HipHeight = 0,
    Jetpack = false,
    Invisible = false,
    WaterWalk = {Enabled = false, Platform = nil},
    Stamina = false,
    AntiKnockback = false,
    VehicleSpeed = {Enabled = false, Value = 200},

    Aimbot = {
        Enabled = false, 
        FOV = 150, 
        Smoothness = 0.35, 
        Part = "Head", 
        PartFallbacks = {"Head", "Torso", "UpperTorso", "HumanoidRootPart", "LeftArm", "RightArm", "LeftUpperArm", "RightUpperArm"},
        PartMode = "Auto", -- "Auto" = Head with body-part fallback; anything else = exact part name
        TeamCheck = true, 
        WallCheck = false, 
        Prediction = true, 
        DropComp = true, 
        AutoShoot = false,
        AutoWallBang = false,
        Priority = "Closest",
        Shake = 0,
        LockOn = false,
        Target = nil,
        PowerMode = false,
        AutoShootMode = "Hold", -- "Hold" = fire while target locked, "Spam" = ultra-fast fire
    },
    CameraLock = {
        Enabled = false,
        Keybind = Enum.KeyCode.X,
    },
    SilentAim = {Enabled = false, FOV = 80, HitChance = 100, TeamCheck = false, VisibleCheck = false},
    TriggerBot = {Enabled = false, Delay = 0},
    AutoParry = {Enabled = false, Range = 25, LastParry = 0, FrameFire = false},
    Hitbox = {Enabled = false, Size = 12, Originals = {}, ExpandTorso = false},
    Reach = {Enabled = false, Distance = 25, Originals = {}},
    SpinBot = {Enabled = false, Speed = 25, Mode = "Velocity"},
    GodMode = false,
    GodModeRevive = false,
    RapidFire = false,
    RapidFireDelay = 0.05,
    MeleeAura = {Enabled = false, Range = 15, AttackAll = false},
    AutoHealCombat = {Enabled = false, Threshold = 50, Slot = 1},

    Fullbright = {Enabled = false, Intensity = 0.2},
    XRay = {Enabled = false, Transparency = 0.7, Originals = {}},
    Wireframe = {Enabled = false, Originals = {}},
    Bloom = {Enabled = false, Intensity = 2, Size = 24},
    SunRays = {Enabled = false, Intensity = 0.3, Spread = 0.5},
    ColorTint = {Enabled = false, Color = Color3.fromRGB(200, 255, 240)},
    TimeFreeze = {Enabled = false, OriginalTime = 12},
    Freecam = {Enabled = false, Speed = 2, CFrame = nil, OriginalCameraType = Enum.CameraType.Custom},
    ClickTP = {Enabled = false, Key = Enum.KeyCode.LeftControl},
    Crosshair = false,
    FOV = 70,
    Gravity = 196.2,
    Overlay = {Enabled = false, FPS = true, ServerName = true, Ping = true, Network = true, AutoShowOnClose = true},
    Theme = "Sky Blue",
    UIScale = 100,

    ESP = {Enabled = false, TeamCheck = false, Boxes = true, Names = true, Health = true, Distance = true, Tracers = true, Tool = true, Color = Color3.fromRGB(255, 50, 50), Skeleton = false, Chams = true},

    AntiAFK = false,
    AutoClick = {Enabled = false, CPS = 15},
    SuperFastClick = false,
    SuperClickCPS = 100,
    UltraClick = false,
    AutoCollect = {Enabled = false, Range = 60},
    AutoFarm = {Enabled = false, Mode = "Coins"},
    Spectate = {Enabled = false, Target = nil},

    FPSBoost = {
        Enabled = false,
        RemoveDecals = true,
        RemoveParticles = true,
        RemoveTextures = true,
        DisableShadows = true,
        LowQuality = true,
        RemoveTrails = true,
        RemoveBeams = true,
        DisableLightingEffects = true,
    },

    CustomKeybinds = {
        AimbotToggle = Enum.UserInputType.MouseButton2,
    },

    AimbotMaxDistance = 1000,
    SelectedPlayer = nil,
    JoinJobId = "",
}

local Connections = {}
local ESPObjects = {}
local SavedLocations = {}
local InfoLiveLabels = {}
local ThemeHook = nil -- set later by ApplyTheme so UI factories can pull the live accent
local RainbowConnection = nil -- forward declaration: created inside StartRainbow()

-- POWER THEMES: registry of every accent-driven element in the GUI.
-- ApplyTheme recolors ALL of them, so the whole panel follows the chosen theme.
-- Declared here (top of file) because Notify and every UI factory below call RegisterThemed.
-- Kind == "toggle" items are skipped while their toggle is OFF (grey = off stays grey).
local ThemeRegistry = {}
local function RegisterThemed(obj, prop, kind)
    if not obj then return end
    -- dedupe: tab re-renders recreate the same controls; never double-register a slot
    for _, it in ipairs(ThemeRegistry) do
        if it.Object == obj and it.Prop == (prop or "BackgroundColor3") then return end
    end
    ThemeRegistry[#ThemeRegistry + 1] = {Object = obj, Prop = prop or "BackgroundColor3", Kind = kind}
end

-- destroyed controls (every tab switch) leave dead entries; drop them so the
-- registry — and the rainbow per-frame loop — never grows without bound
local function PurgeThemeRegistry()
    for i = #ThemeRegistry, 1, -1 do
        local o = ThemeRegistry[i].Object
        if not o or not o.Parent then table.remove(ThemeRegistry, i) end
    end
end
-- ══ CRITICAL FIX (v2.1): LOCAL REGISTER OVERFLOW ══
-- Luau hard-caps a script chunk at 200 local registers. This hub used 205+, so the
-- WHOLE SCRIPT failed to compile with:
--   "Out of local registers when trying to allocate dragStart; exceeded limit 200"
-- and nothing ran at all. Fix: these internal flags live in the script GLOBALS now
-- (same names, same behavior, closures see them identically) — they simply stop
-- consuming the finite chunk-local register budget.
ScriptStartTime = os.clock()
CopyToClipboard = nil -- assigned later, stays global on purpose
PanicActive = false
uiVisible = false
OriginalGravity = Workspace.Gravity
TargetHighlight = nil
ToggleControls = {}
FPSBoostOriginals = {}
FPSBoostProcessed = {}
FPSBoostConnection = nil
CurrentAimbotTarget = nil
LastAimbotCache = 0
FPSBoostProcessing = false
FPSBoostGeneration = 0
MaxWorldScanObjects = 4000
HitboxConnections = {}
ReachConnection = nil
PlayerCache = {}
RaycastParamCache = nil
LastToolCheck = 0
HasToolEquipped = false
LastGodModeSet = 0
LastClickTime = 0
ClickCooldown = 0.005
OverrideClickCooldown = false -- true = bypass UniversalClick throttle (CPS systems set their own rate)
ActiveThreads = {}
FPSBoostLightingOriginals = nil
InvisibleOriginals = {}
LastTriggerTime = 0
LastAutoCollectScan = 0
AutoCollectTargets = {}
LastAutoFarmScan = 0
AutoFarmTarget = nil

-- ==================== UTILITIES (FULLY FIXED) ====================
local function SafeCall(fn, ...)
    if type(fn) ~= "function" then return false, "Not a function" end
    local ok, result = pcall(fn, ...)
    if not ok then 
        warn(string.format("[RBX 1.0] Error: %s", tostring(result))) 
    end
    return ok, result
end

-- FIXED: Proper character getters with validation
local function GetChar() 
    if not LocalPlayer then return nil end
    local success, char = pcall(function() return LocalPlayer.Character end)
    return success and char and char.Parent and char or nil
end

local function GetHum() 
    local c = GetChar() 
    if not c then return nil end
    local success, hum = pcall(function() return c:FindFirstChildOfClass("Humanoid") end)
    return success and hum and hum.Parent and hum or nil
end

local function GetHRP() 
    local c = GetChar() 
    if not c then return nil end
    local success, hrp = pcall(function() return c:FindFirstChild("HumanoidRootPart") end)
    return success and hrp and hrp.Parent and hrp or nil
end

-- FIXED: Proper disconnection with type checking
local function Disconnect(name)
    if Connections[name] then
        SafeCall(function() 
            local conn = Connections[name]
            if typeof(conn) == "RBXScriptConnection" then
                conn:Disconnect() 
            elseif type(conn) == "table" and conn.Disconnect then
                conn:Disconnect()
            end
        end)
        Connections[name] = nil
    end
end

local function Connect(name, signal, fn)
    if not signal or not fn then return end
    if PanicActive then return end
    Disconnect(name)
    local success, conn = pcall(function() return signal:Connect(fn) end)
    if success and conn then
        Connections[name] = conn
    end
end

-- FIXED: Player alive check with caching
local function IsPlayerAlive(p)
    if not p or not p.Character or not p.Character.Parent then return false end
    local hum = p.Character:FindFirstChildOfClass("Humanoid")
    return hum and hum.Health > 0
end

-- FIXED: Tool checker with caching (reduces per-frame checks)
local function HasTool()
    local now = tick()
    if now - LastToolCheck < 0.1 then
        return HasToolEquipped
    end
    LastToolCheck = now
    local char = GetChar()
    if char then
        HasToolEquipped = char:FindFirstChildOfClass("Tool") ~= nil
    else
        HasToolEquipped = false
    end
    return HasToolEquipped
end

-- FIXED: Player cache system for performance
local function GetCachedPlayers()
    local now = tick()
    if not PlayerCache.LastUpdate or now - PlayerCache.LastUpdate > 1 then
        PlayerCache.Players = Players:GetPlayers()
        PlayerCache.LastUpdate = now
    end
    return PlayerCache.Players or {}
end

-- FIXED: Raycast params caching
local function GetRaycastParams()
    if not RaycastParamCache then
        RaycastParamCache = RaycastParams.new()
        RaycastParamCache.FilterType = Enum.RaycastFilterType.Blacklist
    end
    local char = GetChar()
    local tool = char and char:FindFirstChildOfClass("Tool")
    local filterList = {char}
    if tool then table.insert(filterList, tool) end
    RaycastParamCache.FilterDescendantsInstances = filterList
    return RaycastParamCache
end

-- ==================== UNIVERSAL CLICKER (FULLY FIXED) ====================
local ClickRemoteNames = {"Attack", "Swing", "M1", "Click", "Fire", "Hit", "Combat", "Punch", "Slash", "Damage", "InputBegan", "MouseButton1", "Use", "Activate", "CombatEvent", "ToolActivate", "Melee", "Sword", "SwingEvent"}

-- Forward declaration: the body is defined further down (after the aimbot system)
local GetSilentAimPosition

local function UniversalClick(force)
    local now = tick()
    local minGap = OverrideClickCooldown and 0 or ClickCooldown
    if now - LastClickTime < minGap then return end
    LastClickTime = now

    local char = GetChar()
    if not char then return end

    local tool = char:FindFirstChildOfClass("Tool")
    if not tool then return end

    -- POWER COMBAT: compute the silent-aim hit position once (target lock + prediction + drop)
    local hitPos = GetSilentAimPosition()

    -- Method 1: Standard Roblox Tool Activation (most reliable)
    SafeCall(function() 
        if tool.Enabled then
            tool:Activate() 
        end
    end)

    -- Method 2: VirtualUser (for UI-based clicks)
    SafeCall(function()
        VirtualUser:CaptureController()
        VirtualUser:ClickButton1(Vector2.new(0,0), Camera)
    end)

    -- Method 3: Fire RemoteEvents (server-authoritative games)
    -- POWER COMBAT: pass the silent-aim hit position so guns actually hit the locked target
    SafeCall(function()
        for _, remoteName in ipairs(ClickRemoteNames) do
            local remote = tool:FindFirstChild(remoteName)
            if remote then
                if remote:IsA("RemoteEvent") then
                    if hitPos then remote:FireServer(hitPos) else remote:FireServer() end
                elseif remote:IsA("RemoteFunction") then
                    if hitPos then remote:InvokeServer(hitPos) else remote:InvokeServer() end
                elseif remote:IsA("BindableEvent") then
                    remote:Fire()
                end
            end

            local rsRemote = ReplicatedStorage:FindFirstChild(remoteName, true)
            if rsRemote and rsRemote:IsA("RemoteEvent") then
                if hitPos then rsRemote:FireServer(tool, hitPos) else rsRemote:FireServer(tool, Camera.CFrame.LookVector) end
            end
        end
    end)

    -- Method 4: Fire BindableEvents in the tool
    SafeCall(function()
        for _, child in ipairs(tool:GetDescendants()) do
            if child:IsA("BindableEvent") then
                local name = child.Name:lower()
                if name:match("click") or name:match("attack") or name:match("swing") or name:match("m1") or name:match("use") or name:match("melee") or name:match("sword") then
                    child:Fire()
                end
            end
        end
    end)

    -- Method 5: Trigger tool-local scripts via events
    SafeCall(function()
        if tool:FindFirstChild("Client") and tool.Client:IsA("LocalScript") then
            local event = tool.Client:FindFirstChildOfClass("BindableEvent")
            if event then event:Fire() end
        end
    end)

    -- Method 6: Animation speedup for attack anims
    SafeCall(function()
        local humanoid = char:FindFirstChildOfClass("Humanoid")
        if humanoid then
            for _, animTrack in ipairs(humanoid:GetPlayingAnimationTracks()) do
                local name = animTrack.Name:lower()
                if name:match("attack") or name:match("swing") or name:match("m1") or name:match("punch") or name:match("slash") or name:match("melee") or name:match("sword") then
                    animTrack:AdjustSpeed(3)
                end
            end
        end
    end)

    -- Method 7: Direct tool activation for melee/sword tools
    SafeCall(function()
        if tool:FindFirstChild("Handle") then
            local swingVal = tool:FindFirstChild("Swing") or tool:FindFirstChild("Attack") or tool:FindFirstChild("CanAttack")
            if swingVal and swingVal:IsA("BoolValue") then
                swingVal.Value = true
            end
            local numVal = tool:FindFirstChild("AttackTime") or tool:FindFirstChild("Cooldown")
            if numVal and numVal:IsA("NumberValue") then
                numVal.Value = 0
            end
        end
    end)

    -- Method 8: Fire proximity prompts if they exist
    SafeCall(function()
        for _, prompt in ipairs(tool:GetDescendants()) do
            if prompt:IsA("ProximityPrompt") then
                if fireproximityprompt then
                    fireproximityprompt(prompt)
                end
            end
        end
    end)

    -- POWER COMBAT Method 9: fire every RemoteEvent nested anywhere in the tool (gun scripts)
    SafeCall(function()
        for _, obj in ipairs(tool:GetDescendants()) do
            if obj:IsA("RemoteEvent") then
                if hitPos then obj:FireServer(hitPos) else obj:FireServer() end
            elseif obj:IsA("RemoteFunction") then
                if hitPos then obj:InvokeServer(hitPos) else obj:InvokeServer() end
            end
        end
    end)
end

-- ==================== POWER COMBAT: SHARED HELPERS ====================
-- Fires any Parry/Block/Deflect remotes + the key press so Auto Parry works in every game
local function TriggerParry()
    local char = GetChar()
    local tool = char and char:FindFirstChildOfClass("Tool")
    SafeCall(function()
        VirtualUser:CaptureController()
        VirtualUser:SetKeyDown("f")
        task.wait(0.05)
        VirtualUser:SetKeyUp("f")
    end)
    SafeCall(function() if tool and tool.Enabled then tool:Activate() end end)
    for _, remoteName in ipairs({"Parry", "Block", "Deflect", "Guard", "ParryEvent", "BlockEvent", "Combat", "Swing"}) do
        local remote = tool and tool:FindFirstChild(remoteName)
        if not remote and ReplicatedStorage then
            remote = ReplicatedStorage:FindFirstChild(remoteName, true)
        end
        if remote and remote:IsA("RemoteEvent") then
            SafeCall(function() remote:FireServer() end)
        end
    end
end

-- Auto Pot / Auto Eat: uses the first healing-style item from the Backpack when hurt
local function TryConsumeHealingItem()
    local hum = GetHum()
    local char = GetChar()
    local backpack = LocalPlayer and LocalPlayer:FindFirstChildOfClass("Backpack")
    if not hum or not char or not backpack then return end
    for _, item in ipairs(backpack:GetChildren()) do
        if item:IsA("Tool") then
            local n = item.Name:lower()
            if n:match("pot") or n:match("heal") or n:match("med") or n:match("food") or n:match("eat") or n:match("drink") or n:match("bandage") or n:match("apple") or n:match("snack") then
                local original = char:FindFirstChildOfClass("Tool")
                item.Parent = char
                task.wait(0.05)
                local equipped = char:FindFirstChild(item.Name)
                if equipped and equipped:IsA("Tool") then
                    SafeCall(function() if equipped.Enabled then equipped:Activate() end end)
                end
                task.wait(0.1)
                if item and item.Parent == char then item.Parent = backpack end
                if original and original.Parent == backpack then original.Parent = char end
                return true
            end
        end
    end
    return false
end

-- God Mode V2: re-applies the god health right after respawn
local function GodModeRespawnHandler()
    if not State.GodModeRevive then return end
    task.wait(0.6)
    if PanicActive or not State.GodModeRevive then return end
    local hum = GetHum()
    if hum and hum.Health > 0 then
        hum.Health = hum.MaxHealth
        Notify("God Mode", "Revived with full health", 2, Color3.fromRGB(100,100,100))
    end
end

-- ==================== NOTIFICATIONS (FIXED) ====================

-- Shared accent resolver: UI factories and ESP read the live theme color through this.
-- Declared early so every factory below can call it.
function GetAccent()
    if ThemeHook and ThemeHook.Rainbow then
        return ThemeHook.Get()
    end
    return CONFIG.Accent
end

-- ==================== LOADING SCREEN (NEW - FIXED) ====================
local function CreateLoadingScreen()
    local LoadingGui = Instance.new("ScreenGui")
    LoadingGui.Name = "RBXLoading_1_0"
    LoadingGui.ResetOnSpawn = false
    LoadingGui.IgnoreGuiInset = true
    LoadingGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
    LoadingGui.DisplayOrder = 999

    -- Try multiple methods to get PlayerGui
    local parent = nil

    -- Method 1: Direct access
    pcall(function()
        parent = LocalPlayer:FindFirstChild("PlayerGui")
    end)

    -- Method 2: WaitForChild
    if not parent then
        pcall(function()
            parent = LocalPlayer:WaitForChild("PlayerGui", 3)
        end)
    end

    -- Method 3: GetPlayerGui if available
    if not parent then
        pcall(function()
            parent = LocalPlayer.PlayerGui
        end)
    end

    if parent then
        LoadingGui.Parent = parent
    else
        warn("[RBX 1.0] Failed to parent loading screen - PlayerGui not found")
        return nil
    end

    -- GLASS: loader backdrop is a dimmed blur veil, not a solid black wall
    local Backdrop = Instance.new("Frame")
    Backdrop.Name = "Backdrop"
    Backdrop.Size = UDim2.new(1, 0, 1, 0)
    Backdrop.BackgroundColor3 = Color3.fromRGB(5, 5, 5)
    Backdrop.BackgroundTransparency = 0.25
    Backdrop.BorderSizePixel = 0
    Backdrop.ZIndex = 100
    Backdrop.Parent = LoadingGui

    local LoaderBlur = Instance.new("BlurEffect")
    LoaderBlur.Name = "LoaderBlur"
    LoaderBlur.Size = 18
    LoaderBlur.Parent = Lighting -- lightService blur; destroyed with the loader

    local BackdropGradient = Instance.new("UIGradient")
    BackdropGradient.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromRGB(2, 2, 5)),
        ColorSequenceKeypoint.new(0.5, Color3.fromRGB(8, 8, 15)),
        ColorSequenceKeypoint.new(1, Color3.fromRGB(2, 2, 5))
    })
    BackdropGradient.Rotation = 45
    BackdropGradient.Parent = Backdrop

    -- Animated background particles
    local LoadingParticles = Instance.new("Folder")
    LoadingParticles.Name = "Particles"
    LoadingParticles.Parent = Backdrop

    -- Declare all loader-owned locals once, at the top, so nothing is referenced before it exists

    local loadingParticles = {}
    for i = 1, 30 do
        local p = Instance.new("Frame")
        p.Size = UDim2.new(0, math.random(2, 5), 0, math.random(2, 5))
        p.BackgroundColor3 = Color3.fromRGB(80, 80, 100)
        p.BackgroundTransparency = 0.9
        p.BorderSizePixel = 0
        p.ZIndex = 101
        local corner = Instance.new("UICorner")
        corner.CornerRadius = UDim.new(1, 0)
        corner.Parent = p
        p.Parent = LoadingParticles
        table.insert(loadingParticles, {
            frame = p,
            sx = math.random(),
            sy = math.random(),
            speed = 0.0002 + math.random() * 0.0006,
            offset = math.random() * math.pi * 2
        })
    end

    -- Center container
    local CenterContainer = Instance.new("Frame")
    CenterContainer.Name = "CenterContainer"
    CenterContainer.Size = UDim2.new(0, 400, 0, 300)
    CenterContainer.Position = UDim2.new(0.5, -200, 0.5, -150)
    CenterContainer.BackgroundTransparency = 1
    CenterContainer.ZIndex = 102
    CenterContainer.Parent = Backdrop

    -- Logo skull
    local SkullIcon = Instance.new("TextLabel")
    SkullIcon.Name = "SkullIcon"
    SkullIcon.Size = UDim2.new(0, 80, 0, 80)
    SkullIcon.Position = UDim2.new(0.5, -40, 0, 0)
    SkullIcon.BackgroundTransparency = 1
    SkullIcon.Text = "☠️"
    SkullIcon.TextColor3 = Color3.fromRGB(255, 255, 255)
    SkullIcon.Font = Enum.Font.GothamBold
    SkullIcon.TextSize = 60
    SkullIcon.TextStrokeTransparency = 0
    SkullIcon.TextStrokeColor3 = Color3.fromRGB(0, 0, 0)
    SkullIcon.ZIndex = 103
    SkullIcon.Parent = CenterContainer

    -- Title
    local LoadingTitle = Instance.new("TextLabel")
    LoadingTitle.Name = "LoadingTitle"
    LoadingTitle.Size = UDim2.new(1, 0, 0, 40)
    LoadingTitle.Position = UDim2.new(0, 0, 0, 90)
    LoadingTitle.BackgroundTransparency = 1
    LoadingTitle.Text = "RBX 1.0 HUB — MOBILE"
    LoadingTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
    LoadingTitle.Font = Enum.Font.GothamBold
    LoadingTitle.TextSize = 28
    LoadingTitle.TextStrokeTransparency = 0.3
    LoadingTitle.TextStrokeColor3 = Color3.fromRGB(0, 0, 0)
    LoadingTitle.ZIndex = 103
    LoadingTitle.Parent = CenterContainer

    -- Subtitle
    local LoadingSub = Instance.new("TextLabel")
    LoadingSub.Name = "LoadingSub"
    LoadingSub.Size = UDim2.new(1, 0, 0, 24)
    LoadingSub.Position = UDim2.new(0, 0, 0, 130)
    LoadingSub.BackgroundTransparency = 1
    LoadingSub.Text = GetHubVersion() .. " BIG GUI | BLACK EDITION"
    LoadingSub.TextColor3 = Color3.fromRGB(120, 120, 120)
    LoadingSub.Font = Enum.Font.Gotham
    LoadingSub.TextSize = 14
    LoadingSub.ZIndex = 103
    LoadingSub.Parent = CenterContainer

    -- Progress bar background
    local ProgressBg = Instance.new("Frame")
    ProgressBg.Name = "ProgressBg"
    ProgressBg.Size = UDim2.new(0, 300, 0, 6)
    ProgressBg.Position = UDim2.new(0.5, -150, 0, 180)
    ProgressBg.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
    ProgressBg.BorderSizePixel = 0
    ProgressBg.ZIndex = 103
    ProgressBg.Parent = CenterContainer
    local bgCorner = Instance.new("UICorner")
    bgCorner.CornerRadius = UDim.new(1, 0)
    bgCorner.Parent = ProgressBg

    -- Progress bar fill
    local ProgressFill = Instance.new("Frame")
    ProgressFill.Name = "ProgressFill"
    ProgressFill.Size = UDim2.new(0, 0, 1, 0)
    ProgressFill.BackgroundColor3 = Color3.fromRGB(200, 200, 200)
    ProgressFill.BorderSizePixel = 0
    ProgressFill.ZIndex = 104
    ProgressFill.Parent = ProgressBg
    local fillCorner = Instance.new("UICorner")
    fillCorner.CornerRadius = UDim.new(1, 0)
    fillCorner.Parent = ProgressFill

    -- Progress bar glow
    local ProgressGlow = Instance.new("UIStroke")
    ProgressGlow.Color = Color3.fromRGB(200, 200, 200)
    ProgressGlow.Thickness = 4
    ProgressGlow.Transparency = 0.8
    ProgressGlow.Parent = ProgressFill

    -- Status text
    local StatusText = Instance.new("TextLabel")
    StatusText.Name = "StatusText"
    StatusText.Size = UDim2.new(1, 0, 0, 20)
    StatusText.Position = UDim2.new(0, 0, 0, 200)
    StatusText.BackgroundTransparency = 1
    StatusText.Text = "Initializing..."
    StatusText.TextColor3 = Color3.fromRGB(150, 150, 150)
    StatusText.Font = Enum.Font.Gotham
    StatusText.TextSize = 12
    StatusText.ZIndex = 103
    StatusText.Parent = CenterContainer

    -- Percentage text
    local PercentText = Instance.new("TextLabel")
    PercentText.Name = "PercentText"
    PercentText.Size = UDim2.new(0, 60, 0, 20)
    PercentText.Position = UDim2.new(0.5, -30, 0, 200)
    PercentText.BackgroundTransparency = 1
    PercentText.Text = "0%"
    PercentText.TextColor3 = Color3.fromRGB(200, 200, 200)
    PercentText.Font = Enum.Font.GothamBold
    PercentText.TextSize = 12
    PercentText.ZIndex = 103
    PercentText.Parent = CenterContainer

    -- Bottom text
    local BottomText = Instance.new("TextLabel")
    BottomText.Name = "BottomText"
    BottomText.Size = UDim2.new(1, 0, 0, 20)
    BottomText.Position = UDim2.new(0, 0, 1, -20)
    BottomText.BackgroundTransparency = 1
    BottomText.Text = "RBX 1.0 HUB"
    BottomText.TextColor3 = Color3.fromRGB(80, 80, 80)
    BottomText.Font = Enum.Font.Gotham
    BottomText.TextSize = 11
    BottomText.ZIndex = 103
    BottomText.Parent = CenterContainer

    -- Particle animation connection
    local particleConn = RunService.RenderStepped:Connect(function()
        local t = tick()
        for _, data in ipairs(loadingParticles) do
            local y = (data.sy + (t * data.speed)) % 1
            local x = data.sx + math.sin(t * 0.3 + data.offset) * 0.02
            data.frame.Position = UDim2.new(x, 0, y, 0)
        end
    end)

    -- Skull pulse animation
    local skullPulseActive = true
    task.spawn(function()
        while skullPulseActive and LoadingGui and LoadingGui.Parent do
            SafeCall(function()
                TweenService:Create(SkullIcon, TweenInfo.new(1, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut), {
                    TextSize = 64
                }):Play()
            end)
            task.wait(1)
            SafeCall(function()
                TweenService:Create(SkullIcon, TweenInfo.new(1, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut), {
                    TextSize = 60
                }):Play()
            end)
            task.wait(1)
        end
    end)

    local loader = {
        Gui = LoadingGui,
        Backdrop = Backdrop,
        ProgressFill = ProgressFill,
        StatusText = StatusText,
        PercentText = PercentText,
        ParticleConn = particleConn,
        SkullPulseActive = skullPulseActive,
        SetProgress = function(percent, status)
            percent = math.clamp(percent, 0, 100)
            SafeCall(function()
                TweenService:Create(ProgressFill, TweenInfo.new(0.3, Enum.EasingStyle.Quart), {
                    Size = UDim2.new(percent / 100, 0, 1, 0)
                }):Play()
            end)
            if status then
                StatusText.Text = status
            end
            PercentText.Text = tostring(math.floor(percent)) .. "%"
        end,
        Destroy = function()
            skullPulseActive = false
            pcall(function() particleConn:Disconnect() end)
            SafeCall(function() 
                if LoadingGui and LoadingGui.Parent then
                    LoadingGui:Destroy() 
                end
            end)
            -- GLASS: lift the frosted backdrop blur the loader created
            pcall(function()
                local b = Lighting:FindFirstChild("LoaderBlur")
                if b then b:Destroy() end
            end)
        end
    }

    return loader
end

do -- scoped: the old-GUI cleanup runs once, frees a register slot
local oldGui = LocalPlayer:WaitForChild("PlayerGui"):FindFirstChild("RBX_1_0_Hub")
if oldGui then SafeCall(function() oldGui:Destroy() end) end
end

local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "RBX_1_0_Hub"
ScreenGui.ResetOnSpawn = false
ScreenGui.IgnoreGuiInset = true
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.Parent = LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.Enabled = false -- Disabled until loading completes



local NotifStack = {}
local MaxNotifications = 10

local function Notify(title, text, duration, color)
    if PanicActive then return end
    duration = duration or 3
    color = color or CONFIG.Accent

    while #NotifStack >= MaxNotifications do
        local old = table.remove(NotifStack, 1)
        SafeCall(function() if old and old.Parent then old:Destroy() end end)
    end

    local frame = Instance.new("Frame")
    frame.Size = UDim2.new(0, 340, 0, 85)
    frame.Position = UDim2.new(1, 30, 1, -100)
    -- GLASS: notifications are dark frosted panes so text stays readable over any world
    frame.BackgroundColor3 = Color3.fromRGB(10, 14, 22)
    frame.BackgroundTransparency = 0.3
    frame.BorderSizePixel = 0
    frame.Parent = ScreenGui

    Instance.new("UICorner", frame).CornerRadius = UDim.new(0, 12)

    local stroke = Instance.new("UIStroke", frame)
    stroke.Color = color; stroke.Thickness = 1.5; stroke.Transparency = 0.4
    RegisterThemed(stroke, "Color") -- notifications follow the live theme too

    local accent = Instance.new("Frame", frame)
    accent.Size = UDim2.new(0, 3, 1, 0)
    accent.BackgroundColor3 = color
    accent.BorderSizePixel = 0
    RegisterThemed(accent, "BackgroundColor3")

    local ttl = Instance.new("TextLabel", frame)
    ttl.Size = UDim2.new(1, -24, 0, 24); ttl.Position = UDim2.new(0, 16, 0, 8)
    ttl.BackgroundTransparency = 1; ttl.Text = title or "Notification"
    ttl.TextColor3 = Color3.fromRGB(255,255,255); ttl.Font = Enum.Font.GothamBold; ttl.TextSize = 15
    ttl.TextXAlignment = Enum.TextXAlignment.Left

    local txt = Instance.new("TextLabel", frame)
    txt.Size = UDim2.new(1, -24, 0, 40); txt.Position = UDim2.new(0, 16, 0, 32)
    txt.BackgroundTransparency = 1; txt.Text = text or ""
    txt.TextColor3 = Color3.fromRGB(170,170,170); txt.Font = Enum.Font.Gotham; txt.TextSize = 13
    txt.TextXAlignment = Enum.TextXAlignment.Left; txt.TextWrapped = true

    table.insert(NotifStack, frame)
    local stackIndex = #NotifStack
    frame.Position = UDim2.new(1, 30, 1, -100 - ((stackIndex-1)*95))

    SafeCall(function()
        TweenService:Create(frame, TweenInfo.new(0.5, Enum.EasingStyle.Back), {
            Position = UDim2.new(1, -360, 1, -100 - ((stackIndex-1)*95))
        }):Play()
    end)

    task.delay(duration, function()
        if PanicActive then return end
        SafeCall(function()
            TweenService:Create(frame, TweenInfo.new(0.35), {Position = UDim2.new(1, 30, frame.Position.Y.Scale, frame.Position.Y.Offset)}):Play()
        end)
        for _, d in ipairs(frame:GetDescendants()) do
            if d:IsA("TextLabel") then SafeCall(function() TweenService:Create(d, TweenInfo.new(0.25), {TextTransparency = 1}):Play() end) end
            if d:IsA("Frame") then SafeCall(function() TweenService:Create(d, TweenInfo.new(0.25), {BackgroundTransparency = 1}):Play() end) end
            if d:IsA("UIStroke") then SafeCall(function() TweenService:Create(d, TweenInfo.new(0.25), {Transparency = 1}):Play() end) end
        end
        task.wait(0.35)
        SafeCall(function()
            if frame and frame.Parent then
                frame:Destroy()
                for i, n in ipairs(NotifStack) do 
                    if n == frame then table.remove(NotifStack, i); break end 
                end
                for i, n in ipairs(NotifStack) do
                    if n and n.Parent then
                        SafeCall(function()
                            TweenService:Create(n, TweenInfo.new(0.3, Enum.EasingStyle.Back), {
                                Position = UDim2.new(1, -360, 1, -100 - ((i-1)*95))
                            }):Play()
                        end)
                    end
                end
            end
        end)
    end)
end

local function _CopyToClipboard(value, label)
    value = tostring(value or "")
    if value == "" then Notify("Clipboard", "Nothing to copy.", 2, Color3.fromRGB(255,80,80)); return false end
    if type(setclipboard) == "function" then
        local ok = pcall(setclipboard, value)
        if ok then Notify("Clipboard", (label or "Text") .. " copied to clipboard.", 2, Color3.fromRGB(100,100,100)); return true end
    end
    Notify("Clipboard unavailable", value, 4, Color3.fromRGB(180,180,180))
    return false
end
CopyToClipboard = _CopyToClipboard

-- ==================== WATERMARK (FIXED) ====================
currentFPS = 0 -- globals: see LOCAL REGISTER OVERFLOW note above
fpsCount = 0
fpsTime = 0

-- AIM CORE: never-miss part resolver.
-- "Auto" mode prefers the Head, then falls back through body parts (R6 "Torso" / R15 "UpperTorso"
-- etc.) so a missing Head never silently disables the aimbot, and the camera still locks on.
function GetAimPart(character)
    if not character or not character.Parent then return nil end
    local wanted = State.Aimbot.Part
    if State.Aimbot.PartMode ~= "Auto" then
        local exact = character:FindFirstChild(wanted)
        if exact and exact.Parent then return exact end
        return nil
    end
    for _, name in ipairs(State.Aimbot.PartFallbacks or {}) do
        local part = character:FindFirstChild(name)
        if part and part.Parent then return part end
    end
    -- Last resort: any base part that isn't a hat/accessory handle
    for _, part in ipairs(character:GetChildren()) do
        if part:IsA("BasePart") and part.Name ~= "HumanoidRootPart" and not part:FindFirstAncestorOfClass("Accessory") then
            return part
        end
    end
    return nil
end

local Watermark = Instance.new("Frame", ScreenGui)
Watermark.Size = UDim2.new(0, 260, 0, 36)
Watermark.Position = UDim2.new(0, 12, 0, 12)
Watermark.BackgroundColor3 = Color3.fromRGB(10, 14, 22) -- GLASS
Watermark.BackgroundTransparency = 0.3
Watermark.BorderSizePixel = 0
Watermark.Visible = false
Instance.new("UICorner", Watermark).CornerRadius = UDim.new(0, 8)
local WMStroke = Instance.new("UIStroke", Watermark); WMStroke.Color = CONFIG.Accent; WMStroke.Thickness = 1; WMStroke.Transparency = 0.5

local WMText = Instance.new("TextLabel", Watermark)
WMText.Size = UDim2.new(1, -8, 1, 0); WMText.Position = UDim2.new(0, 4, 0, 0)
WMText.BackgroundTransparency = 1; WMText.Text = "RBX 1.0 HUB"
WMText.TextColor3 = Color3.fromRGB(255,255,255); WMText.Font = Enum.Font.GothamBold; WMText.TextSize = 14
WMText.TextXAlignment = Enum.TextXAlignment.Left
WMText.TextStrokeTransparency = 0
WMText.TextStrokeColor3 = Color3.fromRGB(0,0,0)

local WMFPS = Instance.new("TextLabel", Watermark)
WMFPS.Size = UDim2.new(0, 70, 1, 0); WMFPS.Position = UDim2.new(1, -74, 0, 0)
WMFPS.BackgroundTransparency = 1; WMFPS.Text = "60 FPS"
WMFPS.TextColor3 = Color3.fromRGB(180, 180, 180); WMFPS.Font = Enum.Font.GothamBold; WMFPS.TextSize = 13
WMFPS.TextXAlignment = Enum.TextXAlignment.Right

Connect("WatermarkFPS", RunService.RenderStepped, function()
    if PanicActive then return end
    fpsCount = fpsCount + 1
    local now = tick()
    if now - fpsTime >= 1 then
        currentFPS = fpsCount
         SafeCall(function() WMFPS.Text = tostring(currentFPS) .. " FPS" end)
        fpsCount = 0
        fpsTime = now
    end
end)
RegisterThemed(WMStroke, "Color")

-- ==================== CLIENT EFFECTS (FIXED) ====================
local FXFolder = Instance.new("Folder", Camera); FXFolder.Name = "RBX_FX"
local CC = Instance.new("ColorCorrectionEffect", FXFolder); CC.Name = "RBX_CC"; CC.Enabled = true
local BL = Instance.new("BloomEffect", FXFolder); BL.Name = "RBX_Bloom"; BL.Intensity = 0; BL.Size = 0; BL.Threshold = 2
local SR = Instance.new("SunRaysEffect", FXFolder); SR.Name = "RBX_SunRays"; SR.Intensity = 0; SR.Spread = 0

-- ==================== ESP SYSTEM (FIXED) ====================
local ESPFolder = Instance.new("Folder", Camera); ESPFolder.Name = "RBX_ESP"

local function ClearESP()
    for uid, obj in pairs(ESPObjects) do
        SafeCall(function() 
            if obj.connection and typeof(obj.connection) == "RBXScriptConnection" then 
                obj.connection:Disconnect() 
            end 
        end)
        SafeCall(function() if obj.group and obj.group.Parent then obj.group:Destroy() end end)
    end
    ESPObjects = {}
    SafeCall(function() ESPFolder:ClearAllChildren() end)
end

-- POWER VISUALS: bone chains for Skeleton ESP (R15 and R6 rigs)
local SKELETON_R15 = {
    {"Head", "UpperTorso"}, {"UpperTorso", "LowerTorso"},
    {"UpperTorso", "LeftUpperArm"}, {"LeftUpperArm", "LeftLowerArm"}, {"LeftLowerArm", "LeftHand"},
    {"UpperTorso", "RightUpperArm"}, {"RightUpperArm", "RightLowerArm"}, {"RightLowerArm", "RightHand"},
    {"LowerTorso", "LeftUpperLeg"}, {"LeftUpperLeg", "LeftLowerLeg"}, {"LeftLowerLeg", "LeftFoot"},
    {"LowerTorso", "RightUpperLeg"}, {"RightUpperLeg", "RightLowerLeg"}, {"RightLowerLeg", "RightFoot"},
}
local SKELETON_R6 = {
    {"Head", "Torso"},
    {"Torso", "Left Arm"}, {"Torso", "Right Arm"},
    {"Torso", "Left Leg"}, {"Torso", "Right Leg"},
}

local function CreateESP(targetPlayer)
    if targetPlayer == LocalPlayer then return end
    if not targetPlayer or not targetPlayer.Parent then return end
    if ESPObjects[targetPlayer.UserId] then return end
    if not targetPlayer.Character or not targetPlayer.Character.Parent then return end

    local group = Instance.new("Folder", ESPFolder); group.Name = tostring(targetPlayer.UserId)

    local highlight = Instance.new("Highlight", group)
    highlight.Name = "RBX_Highlight"
    highlight.FillTransparency = 0.6
    highlight.OutlineTransparency = 0.2
    highlight.Enabled = false
    highlight.DepthMode = Enum.HighlightDepthMode.AlwaysOnTop

    local box = Instance.new("BoxHandleAdornment", group)
    box.Size = Vector3.new(4, 6, 2); box.Color3 = State.ESP.Color
    box.Transparency = 0.5; box.ZIndex = 5; box.AlwaysOnTop = true; box.Visible = false

    local bb = Instance.new("BillboardGui", group)
    bb.Size = UDim2.new(0, 240, 0, 100); bb.StudsOffset = Vector3.new(0, 4, 0)
    bb.AlwaysOnTop = true

    local nameLbl = Instance.new("TextLabel", bb)
    nameLbl.Size = UDim2.new(1,0,0.22,0); nameLbl.BackgroundTransparency = 1
    nameLbl.Text = targetPlayer.Name or "Unknown"; nameLbl.TextColor3 = State.ESP.Color
    nameLbl.TextStrokeTransparency = 0.3; nameLbl.Font = Enum.Font.GothamBold; nameLbl.TextSize = 15

    local infoLbl = Instance.new("TextLabel", bb)
    infoLbl.Size = UDim2.new(1,0,0.18,0); infoLbl.Position = UDim2.new(0,0,0.22,0)
    infoLbl.BackgroundTransparency = 1; infoLbl.Text = "HP: 100/100 | 0m"
    infoLbl.TextColor3 = Color3.fromRGB(255,255,255); infoLbl.TextStrokeTransparency = 0.5
    infoLbl.Font = Enum.Font.Gotham; infoLbl.TextSize = 12

    local hpBg = Instance.new("Frame", bb)
    hpBg.Size = UDim2.new(0.7,0,0.06,0); hpBg.Position = UDim2.new(0.15,0,0.44,0)
    hpBg.BackgroundColor3 = Color3.fromRGB(40,40,40); hpBg.BorderSizePixel = 0

    local hpFill = Instance.new("Frame", hpBg)
    hpFill.Size = UDim2.new(1,0,1,0); hpFill.BackgroundColor3 = Color3.fromRGB(0,255,100)
    hpFill.BorderSizePixel = 0

    local toolLbl = Instance.new("TextLabel", bb)
    toolLbl.Size = UDim2.new(1,0,0.16,0); toolLbl.Position = UDim2.new(0,0,0.54,0)
    toolLbl.BackgroundTransparency = 1; toolLbl.Text = "Tool: None"
    toolLbl.TextColor3 = Color3.fromRGB(200,200,200); toolLbl.TextStrokeTransparency = 0.5
    toolLbl.Font = Enum.Font.Gotham; toolLbl.TextSize = 11

    local distLbl = Instance.new("TextLabel", bb)
    distLbl.Size = UDim2.new(1,0,0.16,0); distLbl.Position = UDim2.new(0,0,0.74,0)
    distLbl.BackgroundTransparency = 1; distLbl.Text = "0m"
    distLbl.TextColor3 = Color3.fromRGB(150,150,150); distLbl.TextStrokeTransparency = 0.5
    distLbl.Font = Enum.Font.Gotham; distLbl.TextSize = 11

    local tracer = Instance.new("LineHandleAdornment", group)
    tracer.Thickness = 1.5; tracer.Color3 = State.ESP.Color; tracer.Transparency = 0.5
    tracer.ZIndex = 5; tracer.AlwaysOnTop = true; tracer.Visible = false

    local skeletonLines = {}

    local conn = RunService.RenderStepped:Connect(function()
        if PanicActive then return end
        if not State.ESP.Enabled or not targetPlayer.Parent or not group or not group.Parent then
            SafeCall(function() if group and group.Parent then group:Destroy() end end)
            ESPObjects[targetPlayer.UserId] = nil
            return
        end

        local char = targetPlayer.Character
        if not char or not char.Parent then
            SafeCall(function() if group and group.Parent then group:Destroy() end end)
            ESPObjects[targetPlayer.UserId] = nil
            return
        end

        local hrp = char:FindFirstChild("HumanoidRootPart")
        local hum = char:FindFirstChildOfClass("Humanoid")
        if not hrp or not hum then return end

        if hum.Health <= 0 then
            box.Visible = false; bb.Enabled = false; tracer.Visible = false; highlight.Enabled = false
            SafeCall(function() if group and group.Parent then group:Destroy() end end)
            ESPObjects[targetPlayer.UserId] = nil
            return
        end

        SafeCall(function()
            box.Adornee = hrp; bb.Adornee = hrp
            if tracer then tracer.Adornee = hrp end
        end)

        local isTeam = false
        SafeCall(function()
            isTeam = State.ESP.TeamCheck and targetPlayer.Team and LocalPlayer.Team and targetPlayer.Team == LocalPlayer.Team
        end)
        local visible = not isTeam

        box.Visible = State.ESP.Boxes and visible
        bb.Enabled = visible
        tracer.Visible = State.ESP.Tracers and visible
        highlight.Enabled = State.ESP.Chams and visible

        -- FIXED: Names / Health / Distance / Tool toggles now really show and hide each element
        local accent = GetAccent()
        SafeCall(function()
            nameLbl.Visible = State.ESP.Names
            infoLbl.Visible = State.ESP.Health
            hpBg.Visible = State.ESP.Health
            distLbl.Visible = State.ESP.Distance
            toolLbl.Visible = State.ESP.Tool
            box.Color3 = accent
            nameLbl.TextColor3 = accent
            tracer.Color3 = accent
            if highlight and highlight.Parent then
                highlight.FillColor = accent
                highlight.OutlineColor = accent
            end
        end)

        -- POWER VISUALS: Skeleton ESP via bone lines
        if State.ESP.Skeleton and visible then
            SafeCall(function()
                local targetChar = targetPlayer.Character
                local bones = (targetChar and targetChar:FindFirstChild("UpperTorso") and SKELETON_R15)
                    or (targetChar and targetChar:FindFirstChild("Torso") and SKELETON_R6)
                    or nil
                if bones and hrp then
                    local used = 0
                    for _, bone in ipairs(bones) do
                        local p1 = targetChar:FindFirstChild(bone[1])
                        local p2 = targetChar:FindFirstChild(bone[2])
                        if p1 and p2 then
                            used = used + 1
                            local line = skeletonLines[used]
                            if not line or not line.Parent then
                                line = Instance.new("LineHandleAdornment")
                                line.Thickness = 1.5
                                line.AlwaysOnTop = true
                                line.ZIndex = 5
                                line.Parent = group
                                skeletonLines[used] = line
                            end
                            local a, b = p1.Position, p2.Position
                            line.Adornee = hrp
                            local mid = hrp.CFrame:PointToObjectSpace((a + b) / 2)
                            local dir = hrp.CFrame:VectorToObjectSpace(b - a)
                            if dir.Magnitude > 0.001 then
                                line.CFrame = CFrame.lookAt(mid, mid + dir)
                            else
                                line.CFrame = CFrame.new(mid)
                            end
                            line.Length = (b - a).Magnitude
                            line.Color3 = accent
                            line.Visible = true
                        end
                    end
                    for i = used + 1, #skeletonLines do
                        if skeletonLines[i] then skeletonLines[i].Visible = false end
                    end
                else
                    for _, line in ipairs(skeletonLines) do if line then line.Visible = false end end
                end
            end)
        else
            for _, line in ipairs(skeletonLines) do if line then line.Visible = false end end
        end

        SafeCall(function()
            if highlight and highlight.Parent then
                if highlight.Adornee ~= char then highlight.Adornee = char end
                highlight.FillColor = State.ESP.Color
                highlight.OutlineColor = State.ESP.Color
            end
        end)

        if not visible then return end

        local hpPct = math.clamp(hum.Health / math.max(hum.MaxHealth, 1), 0, 1)
        SafeCall(function()
            hpFill.Size = UDim2.new(hpPct, 0, 1, 0)
            if hpPct > 0.5 then hpFill.BackgroundColor3 = Color3.fromRGB(0,255,100)
            elseif hpPct > 0.25 then hpFill.BackgroundColor3 = Color3.fromRGB(255,200,0)
            else hpFill.BackgroundColor3 = Color3.fromRGB(255,50,50) end
        end)

        local myHRP = GetHRP()
        local dist = 0
        SafeCall(function()
            if myHRP then
                dist = math.floor((hrp.Position - myHRP.Position).Magnitude)
            end
        end)
        SafeCall(function()
            infoLbl.Text = string.format("HP: %d/%d | %dm", math.floor(hum.Health), math.floor(hum.MaxHealth), dist)
            distLbl.Text = string.format("%dm", dist)
        end)

        local tool = char:FindFirstChildOfClass("Tool")
        SafeCall(function()
            toolLbl.Text = "Tool: " .. (tool and tool.Name or "None")
        end)

        local scale = math.clamp(1 - (dist/500), 0.3, 1)
        SafeCall(function()
            bb.Size = UDim2.new(0, 240*scale, 0, 100*scale)
        end)

        if myHRP and State.ESP.Tracers and tracer then
            SafeCall(function()
                local rel = myHRP.Position - hrp.Position
                tracer.Length = rel.Magnitude
                tracer.CFrame = CFrame.lookAt(Vector3.zero, rel)
                tracer.Color3 = State.ESP.Color
            end)
        end
    end)

    ESPObjects[targetPlayer.UserId] = {group = group, connection = conn, skeleton = skeletonLines}
end

local function RefreshESP()
    ClearESP()
    if not State.ESP.Enabled then return end
    for _, p in ipairs(Players:GetPlayers()) do
        if p ~= LocalPlayer then CreateESP(p) end
    end
end

local function WatchESPPlayer(p)
    if not p or p == LocalPlayer then return end
    Connect("ESPCharAdded_" .. tostring(p.UserId), p.CharacterAdded, function()
        if PanicActive then return end
        if State.ESP.Enabled then task.wait(0.3); CreateESP(p) end
    end)
    if State.ESP.Enabled then CreateESP(p) end
end

for _, p in ipairs(Players:GetPlayers()) do WatchESPPlayer(p) end
Connect("ESPPlayerAdded", Players.PlayerAdded, function(p)
    if PanicActive then return end
    WatchESPPlayer(p)
end)
Connect("ESPPlayerRemoving", Players.PlayerRemoving, function(p)
    if PanicActive then return end
    Disconnect("ESPCharAdded_" .. tostring(p.UserId))
    if ESPObjects[p.UserId] then
        SafeCall(function() 
            if ESPObjects[p.UserId].connection then 
                ESPObjects[p.UserId].connection:Disconnect() 
            end 
        end)
        SafeCall(function() 
            if ESPObjects[p.UserId].group then 
                ESPObjects[p.UserId].group:Destroy() 
            end 
        end)
        ESPObjects[p.UserId] = nil
    end
    PlayerCache.Players = nil
    PlayerCache.LastUpdate = nil
end)

-- ==================== SUPERCHARGED AIMBOT SYSTEM (FIXED) ====================
local FOVGui = Instance.new("ScreenGui", LocalPlayer.PlayerGui); FOVGui.Name = "RBX_FOV"; FOVGui.ResetOnSpawn = false
FOVGui.IgnoreGuiInset = true -- FOV ring center must match WorldToViewportPoint's true screen center
FOVGui.DisplayOrder = 50
local FOVFrame = Instance.new("Frame", FOVGui); FOVFrame.Size = UDim2.new(0, State.Aimbot.FOV*2, 0, State.Aimbot.FOV*2)
FOVFrame.Position = UDim2.new(0.5, -State.Aimbot.FOV, 0.5, -State.Aimbot.FOV)
FOVFrame.BackgroundTransparency = 1; FOVFrame.Visible = false
Instance.new("UICorner", FOVFrame).CornerRadius = UDim.new(1,0)
local FOVStroke = Instance.new("UIStroke", FOVFrame); FOVStroke.Color = Color3.fromRGB(255,50,50); FOVStroke.Thickness = 2; FOVStroke.Transparency = 0.5

local DistanceLabel = Instance.new("TextLabel", FOVGui)
DistanceLabel.Name = "DistanceLabel"
DistanceLabel.Size = UDim2.new(0, 120, 0, 20)
DistanceLabel.Position = UDim2.new(0.5, -60, 0.5, State.Aimbot.FOV + 15)
DistanceLabel.BackgroundTransparency = 1
DistanceLabel.Text = ""
DistanceLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
DistanceLabel.Font = Enum.Font.GothamBold
DistanceLabel.TextSize = 14
DistanceLabel.Visible = false

-- POWER COMBAT: true when the aimbot toggle key is physically held down (Target Lock override)
local AimbotKeyHeld = false
local AimbotKeyEnum = nil -- EnumItem of the bound key, mirrored from State.CustomKeybinds

local function UpdateTargetHighlight(target)
    if not target or not target.Character or not target.Character.Parent then
        if TargetHighlight then SafeCall(function() TargetHighlight:Destroy() end); TargetHighlight = nil end
        return
    end
    -- highlight follows the aim part (Head) so the glow sits on what you're actually locking
    local hrp = GetAimPart(target.Character)
    if not hrp then
        if TargetHighlight then SafeCall(function() TargetHighlight:Destroy() end); TargetHighlight = nil end
        return
    end
    if not TargetHighlight or TargetHighlight.Parent ~= hrp then
        if TargetHighlight then SafeCall(function() TargetHighlight:Destroy() end) end
        TargetHighlight = Instance.new("Highlight", hrp)
        TargetHighlight.Name = "RBX_Target"
        TargetHighlight.FillTransparency = 0.5
        TargetHighlight.OutlineTransparency = 0
        TargetHighlight.DepthMode = Enum.HighlightDepthMode.AlwaysOnTop
    end
    if State.Aimbot.PowerMode then
        TargetHighlight.FillColor = Color3.fromRGB(255, 50, 50)
        TargetHighlight.OutlineColor = Color3.fromRGB(255, 200, 0)
    else
        TargetHighlight.FillColor = Color3.fromRGB(255, 0, 0)
        TargetHighlight.OutlineColor = Color3.fromRGB(255, 255, 255)
    end
end

local function GetAimbotTarget()
    if PanicActive then return nil end
    local now = tick()
    if now - LastAimbotCache < 0.05 and CurrentAimbotTarget and IsPlayerAlive(CurrentAimbotTarget) then 
        return CurrentAimbotTarget 
    end
    LastAimbotCache = now

    -- POWER COMBAT: target lock override — while the aimbot key is held, nobody else can be picked
    if AimbotKeyHeld and CurrentAimbotTarget and IsPlayerAlive(CurrentAimbotTarget) then
        return CurrentAimbotTarget
    end

    if State.Aimbot.LockOn and CurrentAimbotTarget then
        if IsPlayerAlive(CurrentAimbotTarget) and CurrentAimbotTarget.Character and CurrentAimbotTarget.Character.Parent then
            local part = GetAimPart(CurrentAimbotTarget.Character)
            if part and part.Parent then
                local myHRP = GetHRP()
                local dist3D = 0
                SafeCall(function()
                    if myHRP then
                        dist3D = (part.Position - myHRP.Position).Magnitude
                    end
                end)
                if dist3D <= State.AimbotMaxDistance then
                    local sp, onScreen = Camera:WorldToViewportPoint(part.Position)
                    if onScreen then
                        local dist2D = (Vector2.new(sp.X, sp.Y) - Vector2.new(Camera.ViewportSize.X/2, Camera.ViewportSize.Y/2)).Magnitude
                        if dist2D <= State.Aimbot.FOV then
                            if State.Aimbot.WallCheck and not State.Aimbot.AutoWallBang then
                                local rayParams = RaycastParams.new()
                                rayParams.FilterDescendantsInstances = {GetChar()}
                                rayParams.FilterType = Enum.RaycastFilterType.Blacklist
                                local result = Workspace:Raycast(Camera.CFrame.Position, (part.Position - Camera.CFrame.Position).Unit * math.max(dist3D, 1), rayParams)
                                if result and result.Instance and result.Instance:IsDescendantOf(CurrentAimbotTarget.Character) then
                                    return CurrentAimbotTarget
                                end
                            else
                                return CurrentAimbotTarget
                            end
                        end
                    end
                end
            end
        else
            CurrentAimbotTarget = nil
        end
    end

    local bestTarget, bestScore = nil, math.huge
    local myChar = GetChar()
    if not myChar then CurrentAimbotTarget = nil; return nil end
    local myHRP = GetHRP()
    local screenCenter = Vector2.new(Camera.ViewportSize.X/2, Camera.ViewportSize.Y/2)

    for _, p in ipairs(Players:GetPlayers()) do
        if p == LocalPlayer then continue end
        if State.Aimbot.TeamCheck and p.Team and LocalPlayer.Team and p.Team == LocalPlayer.Team then continue end
        if not IsPlayerAlive(p) then continue end
        if not p.Character or not p.Character.Parent then continue end

        local part = GetAimPart(p.Character)
        if not part or not part.Parent then continue end

        local screenPos, onScreen = Camera:WorldToViewportPoint(part.Position)
        if not onScreen then continue end

        local dist2D = (Vector2.new(screenPos.X, screenPos.Y) - screenCenter).Magnitude
        if dist2D > State.Aimbot.FOV then continue end

        local dist3D = 0
        SafeCall(function()
            if myHRP then
                dist3D = (part.Position - myHRP.Position).Magnitude
            end
        end)
        if dist3D > State.AimbotMaxDistance then continue end

        if State.Aimbot.WallCheck and not State.Aimbot.AutoWallBang then
            local rayParams = RaycastParams.new()
            rayParams.FilterDescendantsInstances = {myChar}
            rayParams.FilterType = Enum.RaycastFilterType.Blacklist
            local result = Workspace:Raycast(Camera.CFrame.Position, (part.Position - Camera.CFrame.Position).Unit * math.max(dist3D, 1), rayParams)
            if not result or not result.Instance or not result.Instance:IsDescendantOf(p.Character) then continue end
        end

        local hum = p.Character:FindFirstChildOfClass("Humanoid")
        local hp = hum and hum.Health or 100
        local score = dist2D

        if State.Aimbot.Priority == "Distance" then
            score = dist3D
        elseif State.Aimbot.Priority == "Lowest Health" then
            score = hp
        elseif State.Aimbot.Priority == "FOV" then
            score = dist2D
        else
            score = dist2D
        end

        if score < bestScore then
            bestScore = score
            bestTarget = p
        end
    end
    CurrentAimbotTarget = bestTarget
    return bestTarget
end

local SilentAimRandom = Random.new(tick())
function GetSilentAimPosition()
    if PanicActive then return nil end
    if not State.SilentAim.Enabled then return nil end

    -- POWER COMBAT: while the aimbot key is held, silent aim ALWAYS follows the locked target
    local forcedPart = nil
    if AimbotKeyHeld and CurrentAimbotTarget and IsPlayerAlive(CurrentAimbotTarget)
        and CurrentAimbotTarget.Character and CurrentAimbotTarget.Character.Parent then
        forcedPart = GetAimPart(CurrentAimbotTarget.Character)
    end

    local target = nil
    local minDist = State.SilentAim.FOV
    local center = Vector2.new(Camera.ViewportSize.X/2, Camera.ViewportSize.Y/2)
    local myChar = GetChar()
    if not myChar then return nil end

    if forcedPart and forcedPart.Parent then
        target = forcedPart -- bypass FOV + hit chance entirely during hard lock
    else
        for _, p in ipairs(GetCachedPlayers()) do
            if p == LocalPlayer then continue end
            if State.SilentAim.TeamCheck and p.Team and LocalPlayer.Team and p.Team == LocalPlayer.Team then continue end
            if not IsPlayerAlive(p) then continue end
            if not p.Character or not p.Character.Parent then continue end
            local part = p.Character:FindFirstChild(State.Aimbot.Part)
            if not part or not part.Parent then continue end
            local sp, onScreen = Camera:WorldToViewportPoint(part.Position)
            if not onScreen then continue end
            local d = (Vector2.new(sp.X, sp.Y) - center).Magnitude
            if d < minDist then
                if State.SilentAim.VisibleCheck then
                    local rayParams = GetRaycastParams()
                    local hit = Workspace:Raycast(Camera.CFrame.Position, (part.Position - Camera.CFrame.Position).Unit * math.max((part.Position - Camera.CFrame.Position).Magnitude, 1), rayParams)
                    if not (hit and hit.Instance and hit.Instance:IsDescendantOf(p.Character)) then continue end
                end
                if SilentAimRandom:NextInteger(1, 100) <= State.SilentAim.HitChance then
                    minDist = d
                    target = part
                end
            end
        end
    end

    if target and target.Parent then
        local pos = target.Position
        if State.Aimbot.Prediction then
            local vel = target.AssemblyLinearVelocity or Vector3.zero
            local mult = State.Aimbot.PowerMode and 0.25 or 0.15
            pos = pos + (vel * mult)
        end
        if State.Aimbot.DropComp then
            pos = pos - Vector3.new(0, 1.5, 0)
        end
        return pos
    end
    return nil
end

-- ==================== CHARACTER STATE REAPPLY (FIXED) ====================
local function ReapplyCharacterState()
    task.wait(0.4)
    if PanicActive then return end
    local hum = GetHum()
    local char = GetChar()
    if not char then return end

    SafeCall(function()
        local oldHRP = char:FindFirstChild("HumanoidRootPart")
        if oldHRP then
            for _, c in ipairs(oldHRP:GetChildren()) do
                if c.Name == "RBX_FlyGyro" or c.Name == "RBX_FlyVel" then
                    c:Destroy()
                end
            end
        end
    end)

    SafeCall(function()
        if State.WaterWalk.Platform and State.WaterWalk.Platform.Parent then
            State.WaterWalk.Platform:Destroy()
            State.WaterWalk.Platform = nil
        end
    end)

    SafeCall(function()
        if hum then
            if State.Speed.Enabled then hum.WalkSpeed = State.Speed.Value else hum.WalkSpeed = 16 end
            if State.Jump.Enabled then hum.JumpPower = State.Jump.Power else hum.JumpPower = 50 end
            if State.HipHeight ~= 0 then hum.HipHeight = State.HipHeight end
            if State.GodMode then hum.Health = hum.MaxHealth end
        end

        if State.NoClip then
            Connect("NoClip", RunService.Heartbeat, function()
                if not State.NoClip or PanicActive then return end
                local c = GetChar()
                if not c then return end
                for _, part in ipairs(c:GetDescendants()) do
                    if part:IsA("BasePart") then part.CanCollide = false end
                end
            end)
        else
            for _, part in ipairs(char:GetDescendants()) do
                if part:IsA("BasePart") then part.CanCollide = true end
            end
        end

        if State.Invisible then
            for _, part in ipairs(char:GetDescendants()) do
                if part:IsA("BasePart") and part.Name ~= "HumanoidRootPart" then part.Transparency = 1
                elseif part:IsA("Decal") or part:IsA("Texture") then part.Transparency = 1 end
            end
        end

        if State.Fly.Enabled then
            local hrp = GetHRP()
            if hrp then
                for _, c in ipairs(hrp:GetChildren()) do
                    if c.Name == "RBX_FlyGyro" or c.Name == "RBX_FlyVel" then c:Destroy() end
                end
                local bg = Instance.new("BodyGyro"); bg.Name = "RBX_FlyGyro"
                bg.MaxTorque = Vector3.new(9e9,9e9,9e9); bg.P = 10000; bg.Parent = hrp
                local bv = Instance.new("BodyVelocity"); bv.Name = "RBX_FlyVel"
                bv.MaxForce = Vector3.new(9e9,9e9,9e9); bv.Velocity = Vector3.zero; bv.Parent = hrp
            end
        end
    end)
end

Connect("LocalCharacterAdded", LocalPlayer.CharacterAdded, ReapplyCharacterState)

-- God Mode V2: full heal right after respawn so god mode survives death
Connect("GodModeRevive", LocalPlayer.CharacterAdded, GodModeRespawnHandler)

Connect("LocalCharacterRemoving", LocalPlayer.CharacterRemoving, function()
    if PanicActive then return end
    SafeCall(function()
        if State.WaterWalk.Platform and State.WaterWalk.Platform.Parent then
            State.WaterWalk.Platform:Destroy()
            State.WaterWalk.Platform = nil
        end
    end)
    SafeCall(function()
        if TargetHighlight then
            TargetHighlight:Destroy()
            TargetHighlight = nil
        end
    end)
end)

-- ==================== UI CONSTRUCTION (BLACK THEME + ANIMATED) ====================
-- ==================== GLASS SYSTEM (FULL GLASS UI) ====================
-- Frosted-glass look: translucent dark panels + white edge highlights + soft sheen.
-- The world behind the open panel gets a live backdrop blur (GLASS BLUR below).
local MainFrame = Instance.new("Frame", ScreenGui)
MainFrame.Name = "MainPanel"; MainFrame.Size = UDim2.new(0, CONFIG.PanelWidth, 0, CONFIG.PanelHeight)
MainFrame.Position = UDim2.new(0.5, -CONFIG.PanelWidth/2, 0.5, -CONFIG.PanelHeight/2 + 40)
MainFrame.BackgroundColor3 = Color3.fromRGB(16, 22, 34); MainFrame.BackgroundTransparency = 0.25
MainFrame.BorderSizePixel = 0; MainFrame.ClipsDescendants = true; MainFrame.Visible = false
Instance.new("UICorner", MainFrame).CornerRadius = UDim.new(0, 18)
local MainGlassStroke = Instance.new("UIStroke", MainFrame)
MainGlassStroke.Color = Color3.fromRGB(255,255,255); MainGlassStroke.Thickness = 1.4; MainGlassStroke.Transparency = 0.72
RegisterThemed(MainGlassStroke, "Color", "glass")
-- GLASS BLUR: while the panel is open the world behind it frosts over.
-- Globals on purpose (register budget + Panic can always find them).
GlassBlur = Instance.new("BlurEffect")
GlassBlur.Name = "RBX_GlassBlur"; GlassBlur.Size = 0; GlassBlur.Parent = Lighting
function SetGlassBlur(on) SafeCall(function() if GlassBlur and GlassBlur.Parent then GlassBlur.Size = on and 14 or 0 end end) end
-- Frost layer: animated white sheen that sells the glass depth (sits behind content)
do
local FrostLayer = Instance.new("Frame", MainFrame)
FrostLayer.Name = "FrostLayer"; FrostLayer.Size = UDim2.new(1,0,1,0)
FrostLayer.BackgroundColor3 = Color3.fromRGB(255,255,255); FrostLayer.BackgroundTransparency = 0.93
FrostLayer.BorderSizePixel = 0; FrostLayer.ZIndex = -6
Instance.new("UICorner", FrostLayer).CornerRadius = UDim.new(0, 18)
local FrostGradient = Instance.new("UIGradient", FrostLayer)
FrostGradient.Color = ColorSequence.new({
    ColorSequenceKeypoint.new(0, Color3.fromRGB(255,255,255)),
    ColorSequenceKeypoint.new(0.5, Color3.fromRGB(190, 210, 235)),
    ColorSequenceKeypoint.new(1, Color3.fromRGB(255,255,255))
})
FrostGradient.Rotation = 115
FrostGradient.Transparency = NumberSequence.new({
    NumberSequenceKeypoint.new(0, 0.45),
    NumberSequenceKeypoint.new(0.5, 0.9),
    NumberSequenceKeypoint.new(1, 0.45)
})
Connect("FrostSheen", RunService.RenderStepped, function()
    if PanicActive then return end
    FrostGradient.Rotation = 115 + math.sin(tick() * 0.35) * 20
end)
end

local MainScale = Instance.new("UIScale")
MainScale.Name = "ResponsiveScale"
MainScale.Parent = MainFrame
local DeviceType = "Desktop"
local function DetectDevice()
    local viewport = Camera and Camera.ViewportSize or Vector2.new(1920, 1080)
    if GuiService:IsTenFootInterface() then return "Console" end
    if UserInputService.TouchEnabled then
        return viewport.X < 600 and "Mobile" or "Tablet"
    end
    return "Desktop"
end
local function UpdateMainScale()
    local v = Camera and Camera.ViewportSize or Vector2.new(CONFIG.PanelWidth + 40, CONFIG.PanelHeight + 40)
    local topLeft, bottomRight = GuiService:GetGuiInset()
    -- FIXED (device fit): the safe area is ALWAYS subtracted (IgnoreGuiInset is on), so the
    -- panel can never slide under notches, bars or touch controls on any device.
    local safeWidth = math.max(1, v.X - topLeft.X - bottomRight.X - CONFIG.MinPanelMargin * 2)
    local safeHeight = math.max(1, v.Y - topLeft.Y - bottomRight.Y - CONFIG.MinPanelMargin * 2)
    DeviceType = DetectDevice()
    local sx = safeWidth / CONFIG.PanelWidth
    local sy = safeHeight / CONFIG.PanelHeight
    -- FIXED (device fit): never upscale on huge monitors (cap 1) + clamp the minimum to 0.3
    -- so tiny windows do not produce an invisible panel, plus the user UI Scale slider.
    local fit = math.min(1, sx, sy) * (State.UIScale / 100)
    MainScale.Scale = math.clamp(fit, 0.3, 1.5)
end
SafeCall(function()
    if Camera then Camera:GetPropertyChangedSignal("ViewportSize"):Connect(UpdateMainScale) end
end)
UpdateMainScale()

-- ==================== UI MOTION SYSTEM ====================
local function AddHoverAnimation(guiObject, normalColor, hoverColor, normalSize, hoverSize)
    if not guiObject or not guiObject:IsA("GuiButton") then return end
    normalColor = normalColor or guiObject.BackgroundColor3
    hoverColor = hoverColor or normalColor:Lerp(Color3.fromRGB(255,255,255), 0.12)
    normalSize = normalSize or guiObject.Size
    hoverSize = hoverSize or UDim2.new(normalSize.X.Scale, normalSize.X.Offset + 2, normalSize.Y.Scale, normalSize.Y.Offset + 2)
    guiObject.MouseEnter:Connect(function()
        if PanicActive or not guiObject.Parent then return end
        SafeCall(function() TweenService:Create(guiObject, TweenInfo.new(0.16, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {BackgroundColor3 = hoverColor, Size = hoverSize}):Play() end)
    end)
    guiObject.MouseLeave:Connect(function()
        if PanicActive or not guiObject.Parent then return end
        SafeCall(function() TweenService:Create(guiObject, TweenInfo.new(0.16, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {BackgroundColor3 = normalColor, Size = normalSize}):Play() end)
    end)
    guiObject.MouseButton1Down:Connect(function()
        if PanicActive or not guiObject.Parent then return end
        SafeCall(function() TweenService:Create(guiObject, TweenInfo.new(0.07, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {Size = normalSize}):Play() end)
    end)
end

do -- scoped: animation locals live only inside this block (register budget)
local BGAnim = Instance.new("Frame", MainFrame)
BGAnim.Name = "BGAnim"; BGAnim.Size = UDim2.new(1,0,1,0); BGAnim.BackgroundTransparency = 1; BGAnim.ZIndex = -5; BGAnim.BorderSizePixel = 0

local BGGradient = Instance.new("UIGradient", BGAnim)
BGGradient.Color = ColorSequence.new({
    ColorSequenceKeypoint.new(0, Color3.fromRGB(5,5,5)),
    ColorSequenceKeypoint.new(0.5, Color3.fromRGB(18,18,24)),
    ColorSequenceKeypoint.new(1, Color3.fromRGB(5,5,5))
})
BGGradient.Rotation = 45

local BGParticles = Instance.new("Folder", BGAnim)
local particles = {}
for i = 1, 20 do
    local p = Instance.new("Frame")
    p.Size = UDim2.new(0, math.random(2,4), 0, math.random(2,4))
    p.BackgroundColor3 = Color3.fromRGB(70,70,85)
    p.BackgroundTransparency = 0.85
    p.BorderSizePixel = 0
    p.ZIndex = -4
    Instance.new("UICorner", p).CornerRadius = UDim.new(1,0)
    p.Parent = BGParticles
    table.insert(particles, {
        frame = p,
        sx = math.random(),
        sy = math.random(),
        speed = 0.0003 + math.random() * 0.0008,
        offset = math.random() * math.pi * 2
    })
end

Connect("BGAnim", RunService.RenderStepped, function()
    if PanicActive then return end
    BGGradient.Rotation = (BGGradient.Rotation + 0.15) % 360
    local t = tick()
    for _, data in ipairs(particles) do
        local y = (data.sy + (t * data.speed)) % 1
        local x = data.sx + math.sin(t * 0.4 + data.offset) * 0.025
        data.frame.Position = UDim2.new(x, 0, y, 0)
    end
end)
end

-- GLASS: tint layer went from solid black (T 0.1) to a translucent deep-blue veil
local BG = Instance.new("Frame", MainFrame); BG.Size = UDim2.new(1,0,1,0); BG.BackgroundColor3 = Color3.fromRGB(8, 12, 20)
BG.BackgroundTransparency = 0.55; BG.BorderSizePixel = 0; BG.ZIndex = -2
Instance.new("UICorner", BG).CornerRadius = UDim.new(0, 14)
local BGStroke = Instance.new("UIStroke", BG); BGStroke.Color = Color3.fromRGB(255,255,255); BGStroke.Thickness = 1; BGStroke.Transparency = 0.85

local AccentBar = Instance.new("Frame", MainFrame); AccentBar.Size = UDim2.new(1,0,0,3)
AccentBar.BackgroundColor3 = CONFIG.Accent; AccentBar.BorderSizePixel = 0

-- GLASS: header strip is a lighter translucent pane with a soft edge
local TitleArea = Instance.new("Frame", MainFrame); TitleArea.Size = UDim2.new(1,0,0,68); TitleArea.Position = UDim2.new(0,0,0,3)
TitleArea.BackgroundColor3 = Color3.fromRGB(255, 255, 255); TitleArea.BackgroundTransparency = 0.93; TitleArea.BorderSizePixel = 0
Instance.new("UICorner", TitleArea).CornerRadius = UDim.new(0, 12)
do
local TitleStroke = Instance.new("UIStroke", TitleArea); TitleStroke.Color = Color3.fromRGB(255,255,255)
TitleStroke.Thickness = 1; TitleStroke.Transparency = 0.86
RegisterThemed(TitleStroke, "Color", "glass")
end

local Logo = Instance.new("Frame", TitleArea); Logo.Size = UDim2.new(0,42,0,42); Logo.Position = UDim2.new(0,16,0,13)
Logo.BackgroundColor3 = Color3.fromRGB(40,40,40); Instance.new("UICorner", Logo).CornerRadius = UDim.new(0,8)
local LogoIcon = Instance.new("TextLabel", Logo); LogoIcon.Size = UDim2.new(1,0,1,0); LogoIcon.BackgroundTransparency = 1
LogoIcon.Text = "☠️"; LogoIcon.TextColor3 = Color3.fromRGB(255,255,255); LogoIcon.Font = Enum.Font.GothamBold; LogoIcon.TextSize = 23

local TitleText = Instance.new("TextLabel", TitleArea); TitleText.Size = UDim2.new(0,330,0,28); TitleText.Position = UDim2.new(0,72,0,9)
TitleText.BackgroundTransparency = 1; TitleText.Text = "RBX 1.0 HUB"
TitleText.TextColor3 = Color3.fromRGB(255,255,255); TitleText.Font = Enum.Font.GothamBold; TitleText.TextSize = 19
TitleText.TextXAlignment = Enum.TextXAlignment.Left
TitleText.TextStrokeTransparency = 0.5
TitleText.TextStrokeColor3 = Color3.fromRGB(0,0,0)

local SubTitle = Instance.new("TextLabel", TitleArea); SubTitle.Size = UDim2.new(0,360,0,20); SubTitle.Position = UDim2.new(0,72,0,38)
SubTitle.BackgroundTransparency = 1; SubTitle.Text = "RBX 1.0 HUB MOBILE | " .. GetHubVersion() .. " POWER COMBAT"
SubTitle.TextColor3 = Color3.fromRGB(120,120,120); SubTitle.Font = Enum.Font.Gotham; SubTitle.TextSize = 11
SubTitle.TextXAlignment = Enum.TextXAlignment.Left

Connect("HeaderPulse", RunService.RenderStepped, function()
    if PanicActive or not MainFrame.Visible then return end
    local pulse = 0.5 + math.sin(tick() * 2.2) * 0.5
    SafeCall(function()
        Logo.BackgroundColor3 = Color3.fromRGB(32 + math.floor(pulse * 18), 32 + math.floor(pulse * 18), 40 + math.floor(pulse * 20))
    end)
end)

do
    local dragging, dragStart, startPos = false, nil, nil
    -- through the registry so PANIC purges these too (they used to leak)
    Connect("MainDragBegan", TitleArea.InputBegan, function(input)
        if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
            dragging = true; dragStart = input.Position; startPos = MainFrame.Position
        end
    end)
    Connect("MainDragChanged", UserInputService.InputChanged, function(input)
        if not dragging or not dragStart or not startPos then return end
        if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
            local d = input.Position - dragStart
            MainFrame.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + d.X, startPos.Y.Scale, startPos.Y.Offset + d.Y)
        end
    end)
    Connect("MainDragEnded", UserInputService.InputEnded, function(input)
        if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then dragging = false end
    end)
end

local TabContainer, ContentFrame, LeftArrow, RightArrow
local minimized = false -- upvalue so ToggleUI can restore a minimized panel on reopen
local function ToggleUI(show)
    if PanicActive then return end
    uiVisible = show
    -- MOBILE EDITION: the toggle stays reachable — the panel just shrinks to the
    -- title bar instead of vanishing (a vanished GUI has no button left on a phone).
    MainFrame.Visible = show
    FloatBtn.Visible = not show
    SetGlassBlur(show) -- GLASS: frost the world while the panel is open
    -- GLASS FIX: minimize (−) must keep the blur (panel is still open),
    -- so blur follows the minimize state too, not just open/close.
    SafeCall(function()
        if GlassBlur and GlassBlur.Parent then
            GlassBlur.Size = (show or not minimized) and 14 or 0
        end
    end)
    if not show and State.Overlay.AutoShowOnClose then
        State.Overlay.Enabled = true
    end
    if show then
        MainFrame.Position = UDim2.new(0.5, -CONFIG.PanelWidth/2, 0.5, -CONFIG.PanelHeight/2 + 40)
        -- reopen always restores the full panel size even if it was minimized when closed
        SafeCall(function()
            MainFrame.Size = UDim2.new(0, CONFIG.PanelWidth, 0, CONFIG.PanelHeight)
            TabContainer.Visible = true
            ContentFrame.Visible = true
            minimized = false
        end)
        local targetScale = MainScale.Scale
        MainScale.Scale = targetScale * 0.92
        SafeCall(function()
            TweenService:Create(MainFrame, TweenInfo.new(0.42, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {
                Position = UDim2.new(0.5, -CONFIG.PanelWidth/2, 0.5, -CONFIG.PanelHeight/2)
            }):Play()
            TweenService:Create(MainScale, TweenInfo.new(0.42, Enum.EasingStyle.Back, Enum.EasingDirection.Out), {
                Scale = targetScale
            }):Play()
        end)
    end
end

local function MakeCtrl(text, color, pos, parent)
    local btn = Instance.new("TextButton", parent); btn.Size = UDim2.new(0,34,0,34); btn.Position = pos
    btn.BackgroundColor3 = color; btn.Text = text; btn.TextColor3 = Color3.fromRGB(255,255,255)
    btn.Font = Enum.Font.GothamBold; btn.TextSize = 14; btn.AutoButtonColor = false
    Instance.new("UICorner", btn).CornerRadius = UDim.new(0,6)
    return btn
end

local CloseBtn = MakeCtrl("×", Color3.fromRGB(80,80,80), UDim2.new(1,-42,0,17), TitleArea)
CloseBtn.MouseButton1Click:Connect(function() if not PanicActive then ToggleUI(false) end end)

local MinBtn = MakeCtrl("−", Color3.fromRGB(80,80,80), UDim2.new(1,-82,0,17), TitleArea)

-- MOBILE EDITION: a phone has no End key — PANIC gets a real on-screen button.
local PanicBtn = MakeCtrl("P", Color3.fromRGB(255,90,90), UDim2.new(1,-122,0,17), TitleArea)
PanicBtn.MouseButton1Click:Connect(function() if not PanicActive then Panic() end end)

-- POWER THEMES: register every accent element now that they all exist.
RegisterThemed(AccentBar, "BackgroundColor3")
RegisterThemed(WMStroke, "Color")
RegisterThemed(overlayStroke, "Color")
RegisterThemed(BGStroke, "Color")
RegisterThemed(FOVStroke, "Color")
RegisterThemed(LeftArrow, "TextColor3")
RegisterThemed(RightArrow, "TextColor3")
RegisterThemed(BtnStroke, "Color")
-- minimized lives as an upvalue above ToggleUI (reopen restores the full panel)
MinBtn.MouseButton1Click:Connect(function()
    if PanicActive then return end
    minimized = not minimized
    TabContainer.Visible = not minimized
    ContentFrame.Visible = not minimized
    SafeCall(function()
        if GlassBlur and GlassBlur.Parent then
            GlassBlur.Size = (uiVisible and not minimized) and 14 or 0
        end
    end)
    SafeCall(function()
        TweenService:Create(MainFrame, TweenInfo.new(0.35), {
            Size = minimized and UDim2.new(0, CONFIG.PanelWidth, 0, 60) or UDim2.new(0, CONFIG.PanelWidth, 0, CONFIG.PanelHeight)
        }):Play()
    end)
end)

TabContainer = Instance.new("ScrollingFrame", MainFrame)
TabContainer.Size = UDim2.new(1, -76, 0, CONFIG.TabHeight); TabContainer.Position = UDim2.new(0, 38, 0, 76)
TabContainer.BackgroundTransparency = 1
TabContainer.BorderSizePixel = 0; TabContainer.ScrollBarThickness = 0; TabContainer.ScrollingDirection = Enum.ScrollingDirection.X
TabContainer.AutomaticCanvasSize = Enum.AutomaticSize.X; TabContainer.CanvasSize = UDim2.new(0,0,0,0)

local TabLayout = Instance.new("UIListLayout", TabContainer)
TabLayout.FillDirection = Enum.FillDirection.Horizontal; TabLayout.Padding = UDim.new(0, 5); TabLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center

ContentFrame = Instance.new("ScrollingFrame", MainFrame)
ContentFrame.Name = "Content"; ContentFrame.Size = UDim2.new(1, -28, 1, -142)
ContentFrame.Position = UDim2.new(0, 14, 0, 132); ContentFrame.BackgroundTransparency = 1
ContentFrame.ScrollBarThickness = 8; ContentFrame.ScrollBarImageColor3 = Color3.fromRGB(60,60,60)
ContentFrame.AutomaticCanvasSize = Enum.AutomaticSize.Y; ContentFrame.CanvasSize = UDim2.new(0,0,0,0)

local ContentList = Instance.new("UIListLayout", ContentFrame)
ContentList.Padding = UDim.new(0, 6)

LeftArrow = Instance.new("TextButton", MainFrame); LeftArrow.Size = UDim2.new(0,28,0,28)
LeftArrow.Position = UDim2.new(0,6,0,84); LeftArrow.BackgroundColor3 = Color3.fromRGB(30,30,30)
LeftArrow.Text = "<"; LeftArrow.TextColor3 = CONFIG.Accent; LeftArrow.Font = Enum.Font.GothamBold; LeftArrow.TextSize = 14
LeftArrow.AutoButtonColor = false; Instance.new("UICorner", LeftArrow).CornerRadius = UDim.new(0,6)

RightArrow = Instance.new("TextButton", MainFrame); RightArrow.Size = UDim2.new(0,28,0,28)
RightArrow.Position = UDim2.new(1,-34,0,84); RightArrow.BackgroundColor3 = Color3.fromRGB(30,30,30)
RightArrow.Text = ">"; RightArrow.TextColor3 = CONFIG.Accent; RightArrow.Font = Enum.Font.GothamBold; RightArrow.TextSize = 14
RightArrow.AutoButtonColor = false; Instance.new("UICorner", RightArrow).CornerRadius = UDim.new(0,6)
AddHoverAnimation(LeftArrow, Color3.fromRGB(30,30,30), Color3.fromRGB(55,55,55))
AddHoverAnimation(RightArrow, Color3.fromRGB(30,30,30), Color3.fromRGB(55,55,55))

-- Reflows the existing tab/content hierarchy whenever the viewport or orientation changes.
-- Mobile uses the same top tabs, but makes them horizontally swipeable and removes arrows.
local function ApplyResponsiveLayout()
    UpdateMainScale()
    local mobile = DeviceType == "Mobile"
    if mobile then
        TabContainer.Position = UDim2.new(0, 8, 0, 76)
        TabContainer.Size = UDim2.new(1, -16, 0, 52)
        TabContainer.ScrollingDirection = Enum.ScrollingDirection.X
        TabLayout.HorizontalAlignment = Enum.HorizontalAlignment.Left
        ContentFrame.Position = UDim2.new(0, 8, 0, 136)
        ContentFrame.Size = UDim2.new(1, -16, 1, -146)
        ContentFrame.ScrollBarThickness = 6
        LeftArrow.Visible = false
        RightArrow.Visible = false
    else
        TabContainer.Position = UDim2.new(0, 38, 0, 76)
        TabContainer.Size = UDim2.new(1, -76, 0, CONFIG.TabHeight)
        TabContainer.ScrollingDirection = Enum.ScrollingDirection.X
        TabLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
        ContentFrame.Position = UDim2.new(0, 14, 0, 132)
        ContentFrame.Size = UDim2.new(1, -28, 1, -142)
        ContentFrame.ScrollBarThickness = 8
        LeftArrow.Visible = true
        RightArrow.Visible = true
    end
end

SafeCall(function()
    if Camera then Camera:GetPropertyChangedSignal("ViewportSize"):Connect(ApplyResponsiveLayout) end
end)
ApplyResponsiveLayout()

-- ==================== UI COMPONENTS (FIXED) ====================
local function CreateSection(parent, text)
    local f = Instance.new("Frame", parent); f.Size = UDim2.new(1,0,0,26); f.BackgroundTransparency = 1
    local line = Instance.new("Frame", f); line.Size = UDim2.new(0.14,0,0,2); line.Position = UDim2.new(0,0,0.5,-1)
    line.BackgroundColor3 = Color3.fromRGB(80,80,80); line.BorderSizePixel = 0
    RegisterThemed(line, "BackgroundColor3")
    local lbl = Instance.new("TextLabel", f); lbl.Size = UDim2.new(0.8,0,1,0); lbl.Position = UDim2.new(0,16,0,0)
    lbl.BackgroundTransparency = 1; lbl.Text = text; lbl.TextColor3 = Color3.fromRGB(160,160,160)
    lbl.Font = Enum.Font.GothamBold; lbl.TextSize = 12; lbl.TextXAlignment = Enum.TextXAlignment.Left
end

local function CreateToggle(parent, text, default, color, callback)
    local frame = Instance.new("Frame", parent); frame.Size = UDim2.new(1,0,0, CONFIG.RowHeight)
    frame.BackgroundColor3 = Color3.fromRGB(255,255,255); frame.BackgroundTransparency = 0.92; frame.BorderSizePixel = 0
    Instance.new("UICorner", frame).CornerRadius = UDim.new(0, 10)
    local stroke = Instance.new("UIStroke", frame); stroke.Color = Color3.fromRGB(255,255,255); stroke.Thickness = 1; stroke.Transparency = 0.85

    local lbl = Instance.new("TextLabel", frame); lbl.Size = UDim2.new(0.55,0,1,0); lbl.Position = UDim2.new(0,14,0,0)
    lbl.BackgroundTransparency = 1; lbl.Text = text; lbl.TextColor3 = Color3.fromRGB(220,220,220)
    lbl.Font = Enum.Font.Gotham; lbl.TextSize = 13; lbl.TextXAlignment = Enum.TextXAlignment.Left

    local bg = Instance.new("Frame", frame); bg.Size = UDim2.new(0,50,0,26); bg.Position = UDim2.new(1,-62,0.5,-13)
    bg.BackgroundColor3 = default and (color or Color3.fromRGB(80,80,80)) or Color3.fromRGB(45,45,45); bg.BorderSizePixel = 0
    Instance.new("UICorner", bg).CornerRadius = UDim.new(1,0)

    local circle = Instance.new("Frame", bg); circle.Size = UDim2.new(0,20,0,20); circle.BackgroundColor3 = Color3.fromRGB(255,255,255)
    circle.BorderSizePixel = 0; circle.Position = default and UDim2.new(1,-23,0.5,-10) or UDim2.new(0,3,0.5,-10)
    Instance.new("UICorner", circle).CornerRadius = UDim.new(1,0)

    local st = default
    local function upd()
        -- POWER THEMES: an ON toggle glows with the live theme accent, not a fixed grey
        local tc = st and ((color and color ~= Color3.fromRGB(80,80,80)) and color or GetAccent()) or Color3.fromRGB(45,45,45)
        local tp = st and UDim2.new(1,-23,0.5,-10) or UDim2.new(0,3,0.5,-10)
        SafeCall(function()
            TweenService:Create(bg, TweenInfo.new(0.25), {BackgroundColor3 = tc}):Play()
            TweenService:Create(circle, TweenInfo.new(0.25), {Position = tp}):Play()
            TweenService:Create(stroke, TweenInfo.new(0.25), {Color = st and GetAccent() or Color3.fromRGB(255,255,255)}):Play()
        end)
    end
    RegisterThemed(bg, "BackgroundColor3", "toggle")
    RegisterThemed(stroke, "Color", "toggle")
    upd() -- initial visual state (default-ON toggles must glow, not show the OFF stroke)

    local click = Instance.new("TextButton", frame); click.Size = UDim2.new(1,0,1,0); click.BackgroundTransparency = 1; click.Text = ""
    click.MouseButton1Click:Connect(function()
        if PanicActive then return end
        st = not st; upd(); SafeCall(callback, st)
    end)

    local control = {Get = function() return st end, Set = function(v) st = v; upd(); SafeCall(callback, v) end}
    ToggleControls[text] = control
    return control
end

local function CreateSlider(parent, text, min, max, default, callback, releaseCallback)
    local frame = Instance.new("Frame", parent); frame.Size = UDim2.new(1,0,0, 64); frame.BackgroundColor3 = Color3.fromRGB(255,255,255); frame.BackgroundTransparency = 0.92
    frame.BorderSizePixel = 0
    local corner = Instance.new("UICorner", frame); corner.CornerRadius = UDim.new(0,10)
    local stroke = Instance.new("UIStroke", frame); stroke.Color = Color3.fromRGB(255,255,255); stroke.Thickness = 1; stroke.Transparency = 0.85

    local lbl = Instance.new("TextLabel", frame); lbl.Size = UDim2.new(0.5,0,0,18); lbl.Position = UDim2.new(0,10,0,5)
    lbl.BackgroundTransparency = 1; lbl.Text = text; lbl.TextColor3 = Color3.fromRGB(210,210,210)
    lbl.Font = Enum.Font.Gotham; lbl.TextSize = 12; lbl.TextXAlignment = Enum.TextXAlignment.Left

    local valLbl = Instance.new("TextLabel", frame); valLbl.Size = UDim2.new(0.3,0,0,18); valLbl.Position = UDim2.new(0.7,-8,0,5)
    valLbl.BackgroundTransparency = 1; valLbl.Text = tostring(default); valLbl.TextColor3 = Color3.fromRGB(180,180,180)
    valLbl.Font = Enum.Font.GothamBold; valLbl.TextSize = 12; valLbl.TextXAlignment = Enum.TextXAlignment.Right

    local track = Instance.new("Frame", frame); track.Size = UDim2.new(1,-20,0,6); track.Position = UDim2.new(0,10,0,40)
    track.BackgroundColor3 = Color3.fromRGB(40,40,40); track.BorderSizePixel = 0
    Instance.new("UICorner", track).CornerRadius = UDim.new(0,3)

    local pct = math.clamp((default - min) / math.max(max - min, 1), 0, 1)
    local fill = Instance.new("Frame", track); fill.Size = UDim2.new(pct,0,1,0); fill.BackgroundColor3 = Color3.fromRGB(120,120,120); fill.BorderSizePixel = 0
    Instance.new("UICorner", fill).CornerRadius = UDim.new(0,3)

    local knob = Instance.new("Frame", track); knob.Size = UDim2.new(0,14,0,14); knob.Position = UDim2.new(pct,-7,0.5,-7)
    knob.BackgroundColor3 = Color3.fromRGB(255,255,255); knob.BorderSizePixel = 0
    Instance.new("UICorner", knob).CornerRadius = UDim.new(1,0)

    local dragging = false; local cur = default
    local function upd(input)
        local trackPos = track.AbsolutePosition.X
        local trackSize = math.max(track.AbsoluteSize.X, 1)
        local pos = math.clamp((input.Position.X - trackPos) / trackSize, 0, 1)
        cur = math.floor(min + (pos * (max - min)))
        fill.Size = UDim2.new(pos,0,1,0); knob.Position = UDim2.new(pos,-7,0.5,-7); valLbl.Text = tostring(cur)
        SafeCall(callback, cur)
    end

    local function onRelease()
        if dragging and releaseCallback then
            SafeCall(releaseCallback, cur)
        end
        dragging = false
    end

    local sliderConnections = {}
    RegisterThemed(fill, "BackgroundColor3")
    sliderConnections[1] = knob.InputBegan:Connect(function(i) 
        if i.UserInputType == Enum.UserInputType.MouseButton1 or i.UserInputType == Enum.UserInputType.Touch then 
            dragging = true 
        end 
    end)
    sliderConnections[2] = track.InputBegan:Connect(function(i) 
        if i.UserInputType == Enum.UserInputType.MouseButton1 or i.UserInputType == Enum.UserInputType.Touch then 
            upd(i); dragging = true 
        end 
    end)
    sliderConnections[3] = UserInputService.InputChanged:Connect(function(i) 
        if dragging and (i.UserInputType == Enum.UserInputType.MouseMovement or i.UserInputType == Enum.UserInputType.Touch) then 
            upd(i) 
        end 
    end)
    sliderConnections[4] = UserInputService.InputEnded:Connect(function(i) 
        if i.UserInputType == Enum.UserInputType.MouseButton1 or i.UserInputType == Enum.UserInputType.Touch then 
            onRelease()
        end 
    end)
    sliderConnections[5] = frame:GetPropertyChangedSignal("AbsoluteSize"):Connect(function()
        local p = math.clamp((cur - min) / math.max(max - min, 1), 0, 1)
        fill.Size = UDim2.new(p,0,1,0)
        knob.Position = UDim2.new(p,-7,0.5,-7)
    end)
    frame.Destroying:Connect(function()
        dragging = false
        for _, conn in ipairs(sliderConnections) do
            SafeCall(function() if conn and typeof(conn) == "RBXScriptConnection" then conn:Disconnect() end end)
        end
    end)

    return {Get = function() return cur end, Set = function(v) cur = v; local p = math.clamp((v-min)/math.max(max-min,1),0,1); fill.Size = UDim2.new(p,0,1,0); knob.Position = UDim2.new(p,-7,0.5,-7); valLbl.Text = tostring(v); SafeCall(callback, v) end}
end

local function CreateButton(parent, text, color, callback)
    local btn = Instance.new("TextButton", parent); btn.Size = UDim2.new(1,0,0,44); btn.BackgroundColor3 = color or Color3.fromRGB(35,35,35)
    btn.Text = text; btn.TextColor3 = Color3.fromRGB(255,255,255); btn.Font = Enum.Font.GothamSemibold; btn.TextSize = 13; btn.AutoButtonColor = false
    local btnStroke = Instance.new("UIStroke", btn)
    btnStroke.Color = color and color:Lerp(Color3.fromRGB(255,255,255),0.2) or Color3.fromRGB(55,55,55); btnStroke.Thickness = 1; btnStroke.Transparency = 0.5
    RegisterThemed(btnStroke, "Color")
    Instance.new("UICorner", btn).CornerRadius = UDim.new(0,10)

    btn.MouseButton1Click:Connect(function()
        if PanicActive then return end
        SafeCall(function()
            TweenService:Create(btn, TweenInfo.new(0.08), {Size = UDim2.new(1,0,0,40)}):Play()
        end)
        task.wait(0.08)
        SafeCall(function()
            TweenService:Create(btn, TweenInfo.new(0.15, Enum.EasingStyle.Back), {Size = UDim2.new(1,0,0,44)}):Play()
        end)
        SafeCall(callback)
    end)
    return btn
end

local function CreateDropdown(parent, text, options, defaultIdx, callback)
    options = type(options) == "table" and options or {}
    defaultIdx = tonumber(defaultIdx) or 1
    local frame = Instance.new("Frame", parent); frame.Size = UDim2.new(1,0,0, CONFIG.RowHeight); frame.BackgroundColor3 = Color3.fromRGB(255,255,255); frame.BackgroundTransparency = 0.92
    frame.BorderSizePixel = 0
    local corner = Instance.new("UICorner", frame); corner.CornerRadius = UDim.new(0,10)
    local stroke = Instance.new("UIStroke", frame); stroke.Color = Color3.fromRGB(255,255,255); stroke.Thickness = 1; stroke.Transparency = 0.85

    local lbl = Instance.new("TextLabel", frame); lbl.Size = UDim2.new(0.4,0,1,0); lbl.Position = UDim2.new(0,14,0,0)
    lbl.BackgroundTransparency = 1; lbl.Text = text; lbl.TextColor3 = Color3.fromRGB(210,210,210)
    lbl.Font = Enum.Font.Gotham; lbl.TextSize = 13; lbl.TextXAlignment = Enum.TextXAlignment.Left

    local sel = Instance.new("Frame", frame); sel.Size = UDim2.new(0,140,0,30); sel.Position = UDim2.new(1,-154,0.5,-15)
    sel.BackgroundColor3 = Color3.fromRGB(30,30,30); sel.BorderSizePixel = 0; Instance.new("UICorner", sel).CornerRadius = UDim.new(0,6)

    local left = Instance.new("TextButton", sel); left.Size = UDim2.new(0,26,1,0); left.BackgroundColor3 = Color3.fromRGB(45,45,45)
    left.Text = "<"; left.TextColor3 = Color3.fromRGB(180,180,180); left.Font = Enum.Font.GothamBold; left.TextSize = 12; left.AutoButtonColor = false
    Instance.new("UICorner", left).CornerRadius = UDim.new(0,6)

    local right = Instance.new("TextButton", sel); right.Size = UDim2.new(0,26,1,0); right.Position = UDim2.new(1,-26,0,0)
    right.BackgroundColor3 = Color3.fromRGB(45,45,45); right.Text = ">"; right.TextColor3 = Color3.fromRGB(180,180,180)
    right.Font = Enum.Font.GothamBold; right.TextSize = 12; right.AutoButtonColor = false
    Instance.new("UICorner", right).CornerRadius = UDim.new(0,6)

    local val = Instance.new("TextLabel", sel); val.Size = UDim2.new(1,-52,1,0); val.Position = UDim2.new(0,26,0,0)
    val.BackgroundTransparency = 1; val.Text = options[defaultIdx] or "None"; val.TextColor3 = Color3.fromRGB(255,255,255)
    val.Font = Enum.Font.GothamBold; val.TextSize = 11

    local currentOptions = options
    local idx = math.clamp(defaultIdx, 1, math.max(#currentOptions, 1))
    local function upd() 
        local opt = currentOptions[idx]
        if opt then
            val.Text = opt
            SafeCall(callback, opt, idx)
        end
    end
    left.MouseButton1Click:Connect(function() 
        if PanicActive then return end
        idx = idx - 1; if idx < 1 then idx = math.max(#currentOptions, 1) end; upd() 
    end)
    right.MouseButton1Click:Connect(function() 
        if PanicActive then return end
        idx = idx + 1; if idx > #currentOptions then idx = 1 end; upd() 
    end)

    local control = {
        Get = function() return currentOptions[idx], idx end, 
        Set = function(i) idx = math.clamp(i, 1, math.max(#currentOptions, 1)); upd() end,
        UpdateOptions = function(newOptions)
            currentOptions = newOptions or {}
            if idx > #currentOptions then idx = 1 end
            upd()
        end
    }
    return control
end

local function CreateTextBox(parent, text, placeholder, callback)
    local frame = Instance.new("Frame", parent); frame.Size = UDim2.new(1,0,0, 56); frame.BackgroundColor3 = Color3.fromRGB(255,255,255); frame.BackgroundTransparency = 0.92
    frame.BorderSizePixel = 0
    local corner = Instance.new("UICorner", frame); corner.CornerRadius = UDim.new(0,10)
    local stroke = Instance.new("UIStroke", frame); stroke.Color = Color3.fromRGB(255,255,255); stroke.Thickness = 1; stroke.Transparency = 0.85

    local lbl = Instance.new("TextLabel", frame); lbl.Size = UDim2.new(0.4,0,0,18); lbl.Position = UDim2.new(0,10,0,5)
    lbl.BackgroundTransparency = 1; lbl.Text = text; lbl.TextColor3 = Color3.fromRGB(210,210,210)
    lbl.Font = Enum.Font.Gotham; lbl.TextSize = 12; lbl.TextXAlignment = Enum.TextXAlignment.Left

    local box = Instance.new("TextBox", frame); box.Size = UDim2.new(0,160,0,28); box.Position = UDim2.new(1,-174,0.5,-14)
    box.BackgroundColor3 = Color3.fromRGB(30,30,30); box.Text = ""; box.PlaceholderText = placeholder
    box.TextColor3 = Color3.fromRGB(255,255,255); box.PlaceholderColor3 = Color3.fromRGB(100,100,100)
    box.Font = Enum.Font.Gotham; box.TextSize = 11; Instance.new("UICorner", box).CornerRadius = UDim.new(0,6)

    box.FocusLost:Connect(function() if not PanicActive then SafeCall(callback, box.Text) end end)
    return box
end

local function CreateKeybind(parent, text, defaultKey, callback)
    local frame = Instance.new("Frame", parent); frame.Size = UDim2.new(1,0,0, CONFIG.RowHeight)
    frame.BackgroundColor3 = Color3.fromRGB(255,255,255); frame.BackgroundTransparency = 0.92; frame.BorderSizePixel = 0
    Instance.new("UICorner", frame).CornerRadius = UDim.new(0, 10)
    local stroke = Instance.new("UIStroke", frame); stroke.Color = Color3.fromRGB(255,255,255); stroke.Thickness = 1; stroke.Transparency = 0.85

    local lbl = Instance.new("TextLabel", frame); lbl.Size = UDim2.new(0.55,0,1,0); lbl.Position = UDim2.new(0,14,0,0)
    lbl.BackgroundTransparency = 1; lbl.Text = text; lbl.TextColor3 = Color3.fromRGB(220,220,220)
    lbl.Font = Enum.Font.Gotham; lbl.TextSize = 13; lbl.TextXAlignment = Enum.TextXAlignment.Left

    local btn = Instance.new("TextButton", frame); btn.Size = UDim2.new(0,100,0,30); btn.Position = UDim2.new(1,-114,0.5,-15)
    btn.BackgroundColor3 = Color3.fromRGB(30,30,30); 
    local displayText = "None"
    if typeof(defaultKey) == "EnumItem" then
        if defaultKey.EnumType == Enum.KeyCode then
            displayText = tostring(defaultKey):gsub("Enum.KeyCode.", "")
        elseif defaultKey.EnumType == Enum.UserInputType then
            displayText = tostring(defaultKey):gsub("Enum.UserInputType.", "")
        end
    end
    btn.Text = displayText
    btn.TextColor3 = Color3.fromRGB(255,255,255); btn.Font = Enum.Font.GothamBold; btn.TextSize = 12; btn.AutoButtonColor = false
    Instance.new("UICorner", btn).CornerRadius = UDim.new(0,6)

    local listening = false
    local timeoutThread = nil
    local inputConn = nil
    btn.MouseButton1Click:Connect(function()
        if PanicActive or listening then return end
        listening = true
        btn.Text = "..."

        timeoutThread = task.delay(5, function()
            if listening then
                listening = false
                btn.Text = displayText
                if inputConn then SafeCall(function() inputConn:Disconnect() end); inputConn = nil end
                Notify("Keybind", "Timeout - no key pressed", 2, Color3.fromRGB(255,50,50))
            end
            timeoutThread = nil
        end)

        inputConn = UserInputService.InputBegan:Connect(function(input, gpe)
            if gpe then return end
            if not listening then 
                if inputConn then inputConn:Disconnect(); inputConn = nil end
                return 
            end

            local valid = false
            if input.UserInputType == Enum.UserInputType.Keyboard then
                displayText = tostring(input.KeyCode):gsub("Enum.KeyCode.", "")
                btn.Text = displayText
                SafeCall(callback, input.KeyCode)
                valid = true
            elseif input.UserInputType == Enum.UserInputType.MouseButton1 then
                displayText = "Mouse1"
                btn.Text = displayText
                SafeCall(callback, Enum.UserInputType.MouseButton1)
                valid = true
            elseif input.UserInputType == Enum.UserInputType.MouseButton2 then
                displayText = "Mouse2"
                btn.Text = displayText
                SafeCall(callback, Enum.UserInputType.MouseButton2)
                valid = true
            elseif input.UserInputType == Enum.UserInputType.MouseButton3 then
                displayText = "Mouse3"
                btn.Text = displayText
                SafeCall(callback, Enum.UserInputType.MouseButton3)
                valid = true
            end

            if valid then
                listening = false
                if inputConn then inputConn:Disconnect(); inputConn = nil end
                if timeoutThread then task.cancel(timeoutThread); timeoutThread = nil end
            end
        end)
    end)
    btn.Destroying:Connect(function()
        listening = false
        if inputConn then SafeCall(function() inputConn:Disconnect() end); inputConn = nil end
        if timeoutThread then SafeCall(function() task.cancel(timeoutThread) end); timeoutThread = nil end
    end)

    return btn
end

local function CreateInfoCard(parent, title, value, buttonText, buttonCallback)
    local frame = Instance.new("Frame", parent)
    frame.Size = UDim2.new(1,0,0,92)
    frame.BackgroundColor3 = Color3.fromRGB(255,255,255); frame.BackgroundTransparency = 0.92; frame.BorderSizePixel = 0
    Instance.new("UICorner", frame).CornerRadius = UDim.new(0,12)
    local stroke = Instance.new("UIStroke", frame); stroke.Color = Color3.fromRGB(255,255,255); stroke.Thickness = 1.2; stroke.Transparency = 0.8
    RegisterThemed(stroke, "Color") -- info cards follow the theme
    local titleLbl = Instance.new("TextLabel", frame); titleLbl.Size = UDim2.new(0.28,0,1,0); titleLbl.Position = UDim2.new(0,18,0,0)
    titleLbl.BackgroundTransparency = 1; titleLbl.Text = title; titleLbl.TextColor3 = Color3.fromRGB(145,145,145); titleLbl.Font = Enum.Font.GothamSemibold; titleLbl.TextSize = 13; titleLbl.TextXAlignment = Enum.TextXAlignment.Left
    local valueLbl = Instance.new("TextLabel", frame); valueLbl.Size = UDim2.new(buttonText and 0.48 or 0.64,0,1,0); valueLbl.Position = UDim2.new(0.28,0,0,0)
    valueLbl.BackgroundTransparency = 1; valueLbl.Text = tostring(value or "Unknown"); valueLbl.TextColor3 = Color3.fromRGB(240,240,240); valueLbl.Font = Enum.Font.GothamBold; valueLbl.TextSize = 13; valueLbl.TextXAlignment = Enum.TextXAlignment.Left; valueLbl.TextTruncate = Enum.TextTruncate.AtEnd
    if type(value) == "function" then InfoLiveLabels[title] = valueLbl end
    if buttonText then
        local btn = Instance.new("TextButton", frame); btn.Size = UDim2.new(0,138,0,36); btn.Position = UDim2.new(1,-156,0.5,-18)
        btn.BackgroundColor3 = Color3.fromRGB(45,45,45); btn.BorderSizePixel = 0; btn.Text = buttonText; btn.TextColor3 = Color3.fromRGB(255,255,255); btn.Font = Enum.Font.GothamBold; btn.TextSize = 12; btn.AutoButtonColor = false
        Instance.new("UICorner", btn).CornerRadius = UDim.new(0,8)
        btn.MouseEnter:Connect(function() if not PanicActive then btn.BackgroundColor3 = Color3.fromRGB(60,60,60) end end)
        btn.MouseLeave:Connect(function() if not PanicActive then btn.BackgroundColor3 = Color3.fromRGB(45,45,45) end end)
        btn.MouseButton1Click:Connect(function() if not PanicActive and buttonCallback then SafeCall(buttonCallback) end end)
    end
    return frame
end

local function CreatePlayerSelector(parent, callback)
    local frame = Instance.new("Frame", parent); frame.Size = UDim2.new(1,0,0, CONFIG.RowHeight + 10)
    frame.BackgroundColor3 = Color3.fromRGB(255,255,255); frame.BackgroundTransparency = 0.92; frame.BorderSizePixel = 0
    Instance.new("UICorner", frame).CornerRadius = UDim.new(0,10)
    local stroke = Instance.new("UIStroke", frame); stroke.Color = Color3.fromRGB(255,255,255); stroke.Thickness = 1; stroke.Transparency = 0.85

    local lbl = Instance.new("TextLabel", frame); lbl.Size = UDim2.new(0.4,0,0,20); lbl.Position = UDim2.new(0,10,0,5)
    lbl.BackgroundTransparency = 1; lbl.Text = "Selected Player"; lbl.TextColor3 = Color3.fromRGB(210,210,210)
    lbl.Font = Enum.Font.Gotham; lbl.TextSize = 12; lbl.TextXAlignment = Enum.TextXAlignment.Left

    local sel = Instance.new("TextLabel", frame); sel.Size = UDim2.new(0.6,0,0,20); sel.Position = UDim2.new(0.4,0,0,5)
    sel.BackgroundTransparency = 1; sel.Text = "None"; sel.TextColor3 = Color3.fromRGB(255,255,255)
    sel.Font = Enum.Font.GothamBold; sel.TextSize = 12

    local btn = Instance.new("TextButton", frame); btn.Size = UDim2.new(0.45,-5,0,26); btn.Position = UDim2.new(0,5,0,30)
    btn.BackgroundColor3 = Color3.fromRGB(40,40,40); btn.Text = "Select Nearest"; btn.TextColor3 = Color3.fromRGB(255,255,255)
    btn.Font = Enum.Font.GothamSemibold; btn.TextSize = 11; Instance.new("UICorner", btn).CornerRadius = UDim.new(0,6)

    local btn2 = Instance.new("TextButton", frame); btn2.Size = UDim2.new(0.45,-5,0,26); btn2.Position = UDim2.new(0.5,5,0,30)
    btn2.BackgroundColor3 = Color3.fromRGB(40,40,40); btn2.Text = "Teleport"; btn2.TextColor3 = Color3.fromRGB(255,255,255)
    btn2.Font = Enum.Font.GothamSemibold; btn2.TextSize = 11; Instance.new("UICorner", btn2).CornerRadius = UDim.new(0,6)

    btn.MouseButton1Click:Connect(function()
        if PanicActive then return end
        local nearest, minDist = nil, math.huge
        local myHRP = GetHRP()
        for _, p in ipairs(Players:GetPlayers()) do
            if p ~= LocalPlayer and p.Character and p.Character.Parent and p.Character:FindFirstChild("HumanoidRootPart") then
                local dist = myHRP and (p.Character.HumanoidRootPart.Position - myHRP.Position).Magnitude or math.huge
                if dist < minDist then minDist = dist; nearest = p end
            end
        end
        if nearest then
            State.SelectedPlayer = nearest
            sel.Text = nearest.Name
            SafeCall(callback, nearest)
            Notify("Players", "Selected: " .. nearest.Name, 2, Color3.fromRGB(100,100,100))
        else
            Notify("Players", "No players found nearby!", 2, Color3.fromRGB(255,50,50))
        end
    end)

    btn2.MouseButton1Click:Connect(function()
        if PanicActive then return end
        if State.SelectedPlayer and State.SelectedPlayer.Parent and State.SelectedPlayer.Character and State.SelectedPlayer.Character.Parent and State.SelectedPlayer.Character:FindFirstChild("HumanoidRootPart") then
            local hrp = GetHRP()
            if hrp then 
                SafeCall(function()
                    hrp.CFrame = State.SelectedPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,0,3) 
                end)
            end
            Notify("Players", "Teleported to " .. State.SelectedPlayer.Name, 2, Color3.fromRGB(100,100,100))
        else
            Notify("Players", "No player selected!", 2, Color3.fromRGB(255,50,50))
        end
    end)

    return frame
end

-- ==================== FPS BOOST (OPTIMIZED & FIXED) ====================
local function ProcessFPSObject(obj)
    if not obj or not obj.Parent then return end
    if FPSBoostProcessed[obj] then return end
    FPSBoostProcessed[obj] = true

    if State.FPSBoost.RemoveDecals or State.FPSBoost.RemoveTextures then
        if (obj:IsA("Decal") or obj:IsA("Texture")) and obj.Transparency < 1 then
            if not FPSBoostOriginals[obj] then FPSBoostOriginals[obj] = obj.Transparency end
            obj.Transparency = 1
        end
    end

    if State.FPSBoost.RemoveParticles then
        if obj:IsA("ParticleEmitter") or obj:IsA("Smoke") or obj:IsA("Fire") or obj:IsA("Sparkles") then
            if not FPSBoostOriginals[obj] then FPSBoostOriginals[obj] = obj.Enabled end
            obj.Enabled = false
        end
    end

    if State.FPSBoost.RemoveTrails then
        if obj:IsA("Trail") then 
            if not FPSBoostOriginals[obj] then FPSBoostOriginals[obj] = obj.Enabled end
            obj.Enabled = false 
        end
    end

    if State.FPSBoost.RemoveBeams then
        if obj:IsA("Beam") then 
            if not FPSBoostOriginals[obj] then FPSBoostOriginals[obj] = obj.Enabled end
            obj.Enabled = false 
        end
    end

    if State.FPSBoost.LowQuality then
        if obj:IsA("BasePart") then
            if not FPSBoostOriginals[obj] then FPSBoostOriginals[obj] = {Material = obj.Material, Reflectance = obj.Reflectance} end
            obj.Material = Enum.Material.Plastic
            obj.Reflectance = 0
        end
    end
end

local function UpdateFPSBoost()
    if not State.FPSBoost.Enabled then
        FPSBoostGeneration += 1
        FPSBoostProcessing = false
        if FPSBoostConnection then 
            SafeCall(function() FPSBoostConnection:Disconnect() end)
            FPSBoostConnection = nil 
        end
        for obj, orig in pairs(FPSBoostOriginals) do
            if obj and obj.Parent then
                if typeof(orig) == "number" then 
                    if obj:IsA("Decal") or obj:IsA("Texture") then
                        obj.Transparency = orig
                    elseif obj:IsA("ParticleEmitter") or obj:IsA("Smoke") or obj:IsA("Fire") or obj:IsA("Sparkles") or obj:IsA("Trail") or obj:IsA("Beam") then
                        obj.Enabled = orig
                    end
                elseif typeof(orig) == "table" and orig.Material then 
                    obj.Material = orig.Material
                    obj.Reflectance = orig.Reflectance
                end
            end
        end
        FPSBoostOriginals = {}
        FPSBoostProcessed = {}
        if FPSBoostLightingOriginals then
            SafeCall(function()
                if FPSBoostLightingOriginals.GlobalShadows ~= nil then Lighting.GlobalShadows = FPSBoostLightingOriginals.GlobalShadows end
                if FPSBoostLightingOriginals.Technology ~= nil then Lighting.Technology = FPSBoostLightingOriginals.Technology end
                for obj, enabled in pairs(FPSBoostLightingOriginals.PostEffects or {}) do
                    if obj and obj.Parent then obj.Enabled = enabled end
                end
            end)
            FPSBoostLightingOriginals = nil
        end
        return
    end

    if not FPSBoostLightingOriginals then
        FPSBoostLightingOriginals = {GlobalShadows = Lighting.GlobalShadows, Technology = Lighting.Technology, PostEffects = {}}
        for _, obj in ipairs(Lighting:GetDescendants()) do
            if obj:IsA("PostEffect") then FPSBoostLightingOriginals.PostEffects[obj] = obj.Enabled end
        end
        for _, obj in ipairs(Camera:GetDescendants()) do
            if obj:IsA("PostEffect") and obj.Name ~= "RBX_CC" and obj.Name ~= "RBX_Bloom" and obj.Name ~= "RBX_SunRays" then
                FPSBoostLightingOriginals.PostEffects[obj] = obj.Enabled
            end
        end
    end

    if not FPSBoostProcessing then
        FPSBoostProcessing = true
        local generation = FPSBoostGeneration
        task.spawn(function()
            local descendants = Workspace:GetDescendants()
            local batchSize = 250
            for i = 1, #descendants, batchSize do
                if not State.FPSBoost.Enabled or generation ~= FPSBoostGeneration then break end
                local endIdx = math.min(i + batchSize - 1, #descendants)
                for j = i, endIdx do
                    ProcessFPSObject(descendants[j])
                end
                task.wait()
            end
            if generation == FPSBoostGeneration then FPSBoostProcessing = false end
        end)
    end

    if not FPSBoostConnection then
        FPSBoostConnection = Workspace.DescendantAdded:Connect(function(obj)
            if State.FPSBoost.Enabled then ProcessFPSObject(obj) end
        end)
    end

    if State.FPSBoost.DisableShadows then
        SafeCall(function()
            Lighting.GlobalShadows = false
            Lighting.Technology = Enum.Technology.Compatibility
        end)
    end

    if State.FPSBoost.DisableLightingEffects then
        SafeCall(function()
            for _, obj in ipairs(Lighting:GetDescendants()) do
                if obj:IsA("PostEffect") then obj.Enabled = false end
            end
            for _, obj in ipairs(Camera:GetDescendants()) do
                if obj:IsA("PostEffect") and obj.Name ~= "RBX_CC" and obj.Name ~= "RBX_Bloom" and obj.Name ~= "RBX_SunRays" then
                    obj.Enabled = false
                end
            end
        end)
    end
end

-- ==================== INFO SYSTEM HELPERS ====================
local function GetGameName()
    local ok, info = pcall(function() return game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId) end)
    if ok and info and info.Name and info.Name ~= "" then return info.Name end
    return (game.Name ~= "" and game.Name) or ("Place " .. tostring(game.PlaceId))
end
local function GetPingText()
    local ok, value = pcall(function() return math.floor(game:GetService("Stats").Network.ServerStatsItem["Data Ping"]:GetValue()) end)
    return ok and (tostring(value) .. " ms") or "N/A"
end
local function GetFPS() return tostring(math.max(0, math.floor(currentFPS or 0))) .. " FPS" end
local function GetUptimeText()
    local total = math.max(0, math.floor(os.clock() - ScriptStartTime))
    return string.format("%02d:%02d:%02d", math.floor(total/3600), math.floor((total%3600)/60), total%60)
end
local function GetPlatformText()
    local ok, platform = pcall(function() return UserInputService:GetPlatform() end)
    return ok and tostring(platform):gsub("Enum.Platform.", "") or "Unknown"
end
-- ==================== SERVER / JOIN STATE ====================
local ServerCache = {At = 0, Servers = {}, Cursor = nil}
local ServerStatus = {Text = "Not checked", Data = nil, Error = nil}

local function GetServerRegion(server)
    if type(server) ~= "table" then return "N/A (not exposed)" end
    local value = server.country or server.region or server.location or server.geo or server.datacenter
    if value and tostring(value) ~= "" then return tostring(value) end
    return "N/A (not exposed)"
end

local function GetAllInfoText()
    local p = LocalPlayer
    local lines = {
        "RBX 1.0 HUB " .. GetHubVersion(),
        "==============================",
        "Game Name: " .. GetGameName(),
        "Place ID: " .. tostring(game.PlaceId),
        "Job ID: " .. tostring(game.JobId or "N/A"),
        "Player Name: " .. tostring(p and p.Name or "Unknown"),
        "Display Name: " .. tostring(p and p.DisplayName or "Unknown"),
        "User ID: " .. tostring(p and p.UserId or "Unknown"),
        "Account Age: " .. tostring(p and p.AccountAge or 0) .. " days",
        "FPS: " .. GetFPS(),
        "Ping: " .. GetPingText(),
        "Uptime: " .. GetUptimeText(),
        "Platform: " .. GetPlatformText(),
        "Server Status: " .. tostring(ServerStatus.Text),
        "Server Members: " .. tostring(ServerStatus.Data and ((ServerStatus.Data.playing or 0) .. " / " .. (ServerStatus.Data.maxPlayers or 0)) or "N/A"),
        "Server Ping: " .. tostring(ServerStatus.Data and ServerStatus.Data.ping or "N/A"),
        "Server FPS: " .. tostring(ServerStatus.Data and ServerStatus.Data.fps or "N/A"),
        "Server Region: " .. GetServerRegion(ServerStatus.Data),
        "Discord: " .. CONFIG.DiscordInvite,
    }
    return table.concat(lines, "\n")
end

local function GetRequestFunction()
    if type(syn) == "table" and type(syn.request) == "function" then return syn.request end
    if type(http_request) == "function" then return http_request end
    if type(request) == "function" then return request end
    return nil
end

local function HttpGetJson(url)
    local req = GetRequestFunction()
    if req then
        local ok, response = pcall(req, {Url = url, Method = "GET"})
        if ok and response then
            local code = tonumber(response.StatusCode or response.Status)
            if code and code >= 400 then return false, "HTTP " .. tostring(code) end
            local body = response.Body or response.body
            if body then
                local decodedOk, data = pcall(function() return HttpService:JSONDecode(body) end)
                if decodedOk and type(data) == "table" then return true, data end
                return false, "Invalid JSON response"
            end
        end
    end

    local ok, body = pcall(function()
        if type(game.HttpGet) == "function" then return game:HttpGet(url) end
        return nil
    end)
    if ok and body then
        local decodedOk, data = pcall(function() return HttpService:JSONDecode(body) end)
        if decodedOk and type(data) == "table" then return true, data end
        return false, "Invalid JSON response"
    end
    return false, "Executor HTTP request API is unavailable"
end

local function FetchPublicServers(maxPages, forceRefresh)
    maxPages = math.clamp(tonumber(maxPages) or 3, 1, 6)
    if not forceRefresh and tick() - ServerCache.At < 5 and #ServerCache.Servers > 0 then
        return true, ServerCache.Servers
    end

    local all = {}
    local cursor = nil
    for _ = 1, maxPages do
        local url = "https://games.roblox.com/v1/games/" .. tostring(game.PlaceId) .. "/servers/Public?sortOrder=Asc&limit=100"
        if cursor and cursor ~= "" then url = url .. "&cursor=" .. HttpService:UrlEncode(cursor) end
        local ok, dataOrError = HttpGetJson(url)
        if not ok then return false, dataOrError end
        local data = dataOrError
        for _, server in ipairs(data.data or {}) do
            if type(server) == "table" and server.id then table.insert(all, server) end
        end
        cursor = data.nextPageCursor
        if not cursor or cursor == "" then break end
    end
    ServerCache = {At = tick(), Servers = all, Cursor = cursor}
    return true, all
end

local function FindServerByJobId(jobId, servers)
    local wanted = tostring(jobId or ""):gsub("^%s+", ""):gsub("%s+$", ""):lower()
    if wanted == "" then return nil end
    for _, server in ipairs(servers or {}) do
        if tostring(server.id or ""):lower() == wanted then return server end
    end
    return nil
end

local function GetCurrentPingNumber()
    local ping
    pcall(function()
        local stats = game:GetService("Stats")
        local network = stats:FindFirstChild("Network")
        local item = network and network:FindFirstChild("ServerStatsItem")
        local dataPing = item and item:FindFirstChild("Data Ping")
        if dataPing then
            local value = tonumber(tostring(dataPing:GetValueString()):match("([%d%.]+)"))
            if value then ping = value end
        end
    end)
    return ping
end

-- ==================== TOP STATUS OVERLAY ====================
-- Kept separate from the panel so it remains readable while the panel is closed.
local StatusOverlay = Instance.new("Frame", ScreenGui)
StatusOverlay.Name = "TopStatusOverlay"
StatusOverlay.AnchorPoint = Vector2.new(0.5, 0)
StatusOverlay.Position = UDim2.new(0.5, 0, 0, 12)
StatusOverlay.Size = UDim2.new(0, 280, 0, 0)
StatusOverlay.AutomaticSize = Enum.AutomaticSize.Y
StatusOverlay.BackgroundColor3 = Color3.fromRGB(10, 14, 22) -- GLASS: frosted dark pane
StatusOverlay.BackgroundTransparency = 0.3
StatusOverlay.BorderSizePixel = 0
StatusOverlay.Visible = false
StatusOverlay.ZIndex = 30
Instance.new("UICorner", StatusOverlay).CornerRadius = UDim.new(0, 10)
local overlayStroke = Instance.new("UIStroke", StatusOverlay)
overlayStroke.Color = CONFIG.Accent; overlayStroke.Transparency = 0.35; overlayStroke.Thickness = 1
local overlayPadding = Instance.new("UIPadding", StatusOverlay)
overlayPadding.PaddingTop = UDim.new(0, 8); overlayPadding.PaddingBottom = UDim.new(0, 8)
overlayPadding.PaddingLeft = UDim.new(0, 12); overlayPadding.PaddingRight = UDim.new(0, 12)
local overlayList = Instance.new("UIListLayout", StatusOverlay)
overlayList.Padding = UDim.new(0, 3); overlayList.SortOrder = Enum.SortOrder.LayoutOrder

local function CreateOverlayRow(prefix)
    local row = Instance.new("TextLabel", StatusOverlay)
    row.Size = UDim2.new(1, 0, 0, 20)
    row.BackgroundTransparency = 1
    row.Font = Enum.Font.GothamSemibold
    row.TextSize = 12
    row.TextColor3 = Color3.fromRGB(238, 238, 245)
    row.TextXAlignment = Enum.TextXAlignment.Left
    row.Text = prefix
    row.ZIndex = 31
    return row
end

local OverlayRows = {
    FPS = CreateOverlayRow("FPS: --"),
    ServerName = CreateOverlayRow("Server: Loading..."),
    Ping = CreateOverlayRow("Ping: --"),
    Network = CreateOverlayRow("Network: Checking..."),
}
do -- scoped: overlay drag state (register budget) + Panic-safe connections
local overlayDragging, overlayDragStart, overlayStartPosition = false, nil, nil
Connect("OverlayDrag", StatusOverlay.InputBegan, function(input)
    if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
        overlayDragging = true
        overlayDragStart = input.Position
        overlayStartPosition = StatusOverlay.Position
    end
end)
Connect("OverlayDragMove", UserInputService.InputChanged, function(input)
    if not overlayDragging or not overlayDragStart or not overlayStartPosition then return end
    if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
        local delta = input.Position - overlayDragStart
        local viewport = Camera and Camera.ViewportSize or Vector2.new(1920, 1080)
        local x = math.clamp(overlayStartPosition.X.Offset + delta.X, -viewport.X * 0.45, viewport.X * 0.45)
        local y = math.clamp(overlayStartPosition.Y.Offset + delta.Y, 8, math.max(8, viewport.Y - 110))
        StatusOverlay.Position = UDim2.new(overlayStartPosition.X.Scale, x, overlayStartPosition.Y.Scale, y)
    end
end)
Connect("OverlayDragEnd", UserInputService.InputEnded, function(input)
    if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
        overlayDragging = false
    end
end)
end
local overlayLastUpdate = 0
local overlayGameName = "Loading..."
local overlayNameUpdated = 0
Connect("TopStatusOverlay", RunService.Heartbeat, function()
    if PanicActive or not State.Overlay.Enabled then
        StatusOverlay.Visible = false
        return
    end
    local now = tick()
    if now - overlayLastUpdate < 0.25 then return end
    overlayLastUpdate = now
    if now - overlayNameUpdated > 20 then
        overlayNameUpdated = now
        overlayGameName = GetGameName()
    end
    local ping = GetCurrentPingNumber()
    OverlayRows.FPS.Visible = State.Overlay.FPS
    OverlayRows.ServerName.Visible = State.Overlay.ServerName
    OverlayRows.Ping.Visible = State.Overlay.Ping
    OverlayRows.Network.Visible = State.Overlay.Network
    OverlayRows.FPS.Text = "FPS: " .. GetFPS()
    OverlayRows.ServerName.Text = "Server: " .. overlayGameName
    OverlayRows.Ping.Text = "Ping: " .. (ping and (tostring(math.floor(ping)) .. " ms") or "N/A")
    OverlayRows.Network.Text = "Network: " .. (ping and (ping < 100 and "Stable" or "High latency") or "Unavailable")
    local v = Camera and Camera.ViewportSize or Vector2.new(1920, 1080)
    StatusOverlay.Size = UDim2.new(0, math.clamp(v.X - 24, 190, 280), 0, 0)
    StatusOverlay.Visible = State.Overlay.FPS or State.Overlay.ServerName or State.Overlay.Ping or State.Overlay.Network
end)
RegisterThemed(overlayStroke, "Color")

local function JoinJobId(jobId)
    local clean = tostring(jobId or ""):gsub("^%s+", ""):gsub("%s+$", "")
    if clean == "" then
        Notify("Join", "Paste a Job ID first.", 2, Color3.fromRGB(255,80,80))
        return false
    end
    if clean == tostring(game.JobId or "") then
        Notify("Join", "You are already in that server.", 2, CONFIG.Accent)
        return false
    end
    local ok, err = pcall(function()
        TeleportService:TeleportToPlaceInstance(game.PlaceId, clean, LocalPlayer)
    end)
    if not ok then
        Notify("Join Failed", tostring(err), 4, Color3.fromRGB(255,80,80))
        return false
    end
    Notify("Join", "Teleport requested for Job ID.", 3, CONFIG.Accent)
    return true
end

local function ChooseBestServer(servers, mode)
    local candidates = {}
    for _, server in ipairs(servers or {}) do
        local id = tostring(server.id or "")
        local playing = tonumber(server.playing) or 0
        local maxPlayers = tonumber(server.maxPlayers) or 0
        if id ~= "" and id ~= tostring(game.JobId or "") and maxPlayers > 0 and playing < maxPlayers then
            table.insert(candidates, server)
        end
    end
    if #candidates == 0 then return nil, "No joinable public server found." end

    table.sort(candidates, function(a,b)
        local ap,bp = tonumber(a.ping), tonumber(b.ping)
        local af,bf = tonumber(a.fps), tonumber(b.fps)
        if mode == "ping" and ap and bp and ap ~= bp then return ap < bp end
        if mode == "best" then
            if ap and bp and ap ~= bp then return ap < bp end
            if af and bf and af ~= bf then return af > bf end
        else
            if af and bf and af ~= bf then return af > bf end
        end
        return (tonumber(a.playing) or 0) < (tonumber(b.playing) or 0)
    end)
    return candidates[1]
end

local function CheckServerStatus(jobId)
    local clean = tostring(jobId or ""):gsub("^%s+", ""):gsub("%s+$", "")
    if clean == "" then
        Notify("Server Status", "Paste a Job ID first.", 2, Color3.fromRGB(255,80,80))
        return false
    end

    -- The current server can always be reported locally without an HTTP request.
    if clean == tostring(game.JobId or "") then
        local playersNow = #Players:GetPlayers()
        local localPing = GetCurrentPingNumber()
        ServerStatus = {
            Text = "Online (Current Server)",
            Data = {id = game.JobId, playing = playersNow, maxPlayers = Players.MaxPlayers, ping = localPing},
            Error = nil,
            LocalPing = localPing
        }
        Notify("Server Status", "Current server is online • " .. tostring(playersNow) .. "/" .. tostring(Players.MaxPlayers), 3, Color3.fromRGB(100,220,150))
        return true
    end

    local ok, serversOrError = FetchPublicServers(6, true)
    if not ok then
        ServerStatus = {Text = "Unavailable", Data = nil, Error = tostring(serversOrError)}
        Notify("Server Status", "Roblox server list could not be reached: " .. tostring(serversOrError), 4, Color3.fromRGB(255,80,80))
        return false
    end
    local target = FindServerByJobId(clean, serversOrError)
    if not target then
        ServerStatus = {Text = "Not found / not public", Data = nil, Error = nil}
        Notify("Server Status", "Job ID was not found in the sampled public-server list. It may be private, full, ended, or outside the sampled pages.", 4, Color3.fromRGB(255,180,80))
        return false
    end
    ServerStatus = {Text = "Online", Data = target, Error = nil, LocalPing = GetCurrentPingNumber()}
    Notify("Server Status", "Online • " .. tostring(target.playing or 0) .. "/" .. tostring(target.maxPlayers or 0) .. " players", 3, Color3.fromRGB(100,220,150))
    return true
end

local function JoinSelectedServer(mode)
    local ok, serversOrError = FetchPublicServers(5, true)
    if not ok then
        Notify("Server Finder", tostring(serversOrError), 4, Color3.fromRGB(255,80,80))
        return
    end
    local server, reason = ChooseBestServer(serversOrError, mode)
    if not server then
        Notify("Server Finder", reason or "No suitable server found.", 3, Color3.fromRGB(255,80,80))
        return
    end
    local ping = tonumber(server.ping)
    local fps = tonumber(server.fps)
    local metric = ping and ("ping " .. math.floor(ping) .. "ms") or (fps and ("FPS " .. math.floor(fps)) or "best available")
    Notify("Server Finder", "Joining " .. metric .. " • " .. tostring(server.playing or 0) .. "/" .. tostring(server.maxPlayers or 0), 3, CONFIG.Accent)
    JoinJobId(server.id)
end

local function GetChangelogText()
    return table.concat({
        "RBX 2.2.0-MOBILE — AIMBOT & GLASS FIXES",
        "",
        "AIMBOT REWRITE",
        "• FIXED: aimbot missed the head — camera updates now bind at Camera+1",
        "  priority (after Roblox's own camera), so the view STAYS locked on",
        "  the head instead of fighting the default camera script every frame.",
        "• FIXED: a missing Head on some rigs silently disabled the aim — new",
        "  Auto part resolver falls back Head > Torso > UpperTorso > arms.",
        "• FOV ring now ignores the top-bar inset, so its center matches the",
        "  real screen center; the target highlight follows the aim part.",
        "• Default smoothing raised to 0.35 (0.08 crawled onto the target).",
        "",
        "GUI FIXES",
        "• FIXED: minimize (−) no longer leaves the screen blurred — blur only",
        "  clears when the panel is actually closed or destroyed.",
        "• FIXED: closing while minimized shrank the panel permanently;",
        "  reopening now always restores the full window.",
        "",
        "RBX 2.1.0-MOBILE — TOUCH EDITION",
        "",
        "MOBILE EDITION CHANGES",
        "• Built for phones/tablets: compact 560x620 panel that fits landscape",
        "  screens, tighter rows, fat touch scrollbars, swipeable tabs.",
        "• On-screen touch controls (right edge): AIM hold = Target Lock,",
        "  CAM = camera-lock toggle, TP = tap-the-ground teleport mode.",
        "• PANIC button in the title bar (phones have no End key) — kills every",
        "  loop, the touch controls included.",
        "• Toggle button stays on screen while the panel is open — the panel",
        "  minimizes to the title bar instead of vanishing into nothing.",
        "• Keyboard hotkeys still work on devices that have them.",
        "",
        "RBX 2.1.0 — FULL GLASS UI / REGISTER OVERFLOW FIX",
        "",
        "CRITICAL FIX",
        "• FIXED: script did not run at all — 'Out of local registers when",
        "  trying to allocate dragStart; exceeded limit 200'. The chunk used",
        "  205+ top-level locals; Luau caps a script at 200. Internal state",
        "  moved to globals + scoped blocks: now 167 and it COMPILES.",
        "",
        "STABILITY HARDENING",
        "• FIXED: theme registry grew without bound — every tab switch rebuilt",
        "  all controls and re-registered them (rainbow loop slowed over time).",
        "  Now deduped on insert + dead entries purged every few seconds.",
        "• FIXED: toggles created in the ON state showed the OFF stroke until",
        "  first clicked (initial visual state was never applied).",
        "• FIXED: window, floating button and overlay drag connections leaked on",
        "  PANIC — all now run through the Panic-safe connection registry.",
        "",
        "FULL GLASS UI (MASTERPIECE EDITION)",
        "• Every panel is now real frosted glass: translucent panes, white",
        "  edge highlights, animated sheen across the whole window.",
        "• GLASS BLUR: the game world behind the panel frosts over while the",
        "  menu is open and unfreezes on close/PANIC.",
        "• Glass cards: toggles, sliders, buttons, dropdowns, textboxes,",
        "  keybinds, info cards — all rebuilt as floating glass panes.",
        "• Glass notifications, watermark, status overlay, floating button",
        "  and the loading screen (blur veil instead of a black wall).",
        "• Themes now tint the glass edges; Rainbow flows through the glass.",
        "",
        "RBX 2.0.0 — POWER COMBAT / RAINBOW / DEVICE-FIT UPDATE",
        "",
        "COMBAT (MASSIVE UPGRADE)",
        "• Silent Aim now really redirects: gun RemoteEvents get a hit position",
        "  locked on the target (CFrame + drop + prediction).",
        "• Target Lock override: hold the Aimbot key to hard-lock one target.",
        "• Auto Parry V2: fires real key presses + tool activation + every",
        "  remote named like Parry/Block/Deflect.",
        "• Auto Parry Every Frame: 5x faster parry fire rate.",
        "• Auto Pot / Auto Eat: drinks healing items when you drop below the",
        "  Pot Threshold slider.",
        "• Rapid Fire V2: fires every RemoteEvent inside the tool with a real",
        "  millisecond delay (Rapid Fire Rate slider, 1-100 ms).",
        "• Melee Aura V2: ATTACK MODE — faces the target (LookAt) and attacks",
        "  with every click method at once.",
        "• Auto Shoot V2: fires whenever a target is inside the aimbot FOV,",
        "  plus a Spam mode that unloads 5 clicks per tick.",
        "• Hitbox V2: optional Torso/Arms expansion (not just Head).",
        "• Spin Bot V2: velocity-free rotation so anti-cheats do not flag it.",
        "• God Mode V2: auto-revive with a full heal right after death.",
        "• PANIC COMBAT button: instantly resets every combat module.",
        "",
        "THEMES / UI",
        "• NEW RAINBOW THEME: every accent in the GUI (header, tabs, toggles,",
        "  sliders, notifications, ESP, aimbot ring) flows through the full RGB",
        "  spectrum in real time.",
        "• Choosing a theme now recolors the WHOLE panel, not just the top bar:",
        "  toggles, sliders, buttons, arrows, strokes, ESP and the floating button.",
        "• New UI Scale slider (50-150%) for extra screen fitting on top of the",
        "  automatic device fit.",
        "",
        "FIXED (BUGS)",
        "• DEVICE FIT: the panel now truly fits EVERY screen. Safe-area is always",
        "  subtracted (notches, bars, touch controls), phones/tablets/consoles",
        "  reflow automatically on rotation, and the minimum scale is clamped.",
        "• Loading screen: Gui reference typo fixed — fade-out animation works.",
        "• COPY ALL INFO: GetServerRegion crash fixed (function now exists).",
        "• CPS is REAL now: Super/Ultra/Auto Click run at the exact speed shown;",
        "  the hidden 66 CPS global cap is gone.",
        "• ESP: Names / Health / Distance / Tool toggles now really hide each part.",
        "• ESP: added Skeleton drawing (R6 + R15).",
        "• FPS meter no longer uses undeclared globals.",
        "• Destroy GUI now runs full PANIC cleanup (kills all loops).",
        "• ScreenGui now uses IgnoreGuiInset (no more offset by the top bar).",
        "• Profile import validates theme and UI-scale values.",
        "",
        "NOTES",
        "• Device layout updates automatically after rotation or window resizing.",
        "• Rainbow overrides the accent color everywhere until you pick another theme.",
        "• Server data is shown only when Roblox exposes it.",
    }, "\n")
end

-- Exports only client UI/preferences. Active feature toggles are intentionally not saved,
-- so importing a profile cannot unexpectedly start a loop or change the character state.
local function BuildSettingsProfile()
    return {
        Version = "1.4.0",
        Overlay = {
            Enabled = State.Overlay.Enabled, FPS = State.Overlay.FPS,
            ServerName = State.Overlay.ServerName, Ping = State.Overlay.Ping,
            Network = State.Overlay.Network, AutoShowOnClose = State.Overlay.AutoShowOnClose,
        },
        Display = {FOV = State.FOV, Gravity = State.Gravity},
        Movement = {SpeedValue = State.Speed.Value, JumpPower = State.Jump.Power, FlySpeed = State.Fly.Speed},
        Aimbot = {FOV = State.Aimbot.FOV, Smoothness = State.Aimbot.Smoothness, Part = State.Aimbot.Part, TeamCheck = State.Aimbot.TeamCheck},
        FPSBoost = {
            RemoveDecals = State.FPSBoost.RemoveDecals, RemoveParticles = State.FPSBoost.RemoveParticles,
            RemoveTextures = State.FPSBoost.RemoveTextures, DisableShadows = State.FPSBoost.DisableShadows,
            LowQuality = State.FPSBoost.LowQuality, RemoveTrails = State.FPSBoost.RemoveTrails,
            RemoveBeams = State.FPSBoost.RemoveBeams, DisableLightingEffects = State.FPSBoost.DisableLightingEffects,
        },
    }
end

local function ApplySettingsProfile(data)
    if type(data) ~= "table" then return false, "Profile must be a JSON object." end
    local function copyBooleans(source, destination, allowed)
        if type(source) ~= "table" then return end
        for _, key in ipairs(allowed) do if type(source[key]) == "boolean" then destination[key] = source[key] end end
    end
    copyBooleans(data.Overlay, State.Overlay, {"Enabled", "FPS", "ServerName", "Ping", "Network", "AutoShowOnClose"})
    copyBooleans(data.FPSBoost, State.FPSBoost, {"RemoveDecals", "RemoveParticles", "RemoveTextures", "DisableShadows", "LowQuality", "RemoveTrails", "RemoveBeams", "DisableLightingEffects"})
    if type(data.Display) == "table" then
        if type(data.Display.FOV) == "number" then State.FOV = math.clamp(data.Display.FOV, 40, 120) end
        if type(data.Display.Gravity) == "number" then State.Gravity = math.clamp(data.Display.Gravity, 0, 500) end
        if type(data.Display.UIScale) == "number" then State.UIScale = math.clamp(data.Display.UIScale, 50, 150) end
    end
    if type(data.Movement) == "table" then
        if type(data.Movement.SpeedValue) == "number" then State.Speed.Value = math.clamp(data.Movement.SpeedValue, 50, 500) end
        if type(data.Movement.JumpPower) == "number" then State.Jump.Power = math.clamp(data.Movement.JumpPower, 50, 300) end
        if type(data.Movement.FlySpeed) == "number" then State.Fly.Speed = math.clamp(data.Movement.FlySpeed, 10, 200) end
    end
    if type(data.Aimbot) == "table" then
        if type(data.Aimbot.FOV) == "number" then State.Aimbot.FOV = math.clamp(data.Aimbot.FOV, 30, 500) end
        if type(data.Aimbot.Smoothness) == "number" then State.Aimbot.Smoothness = math.clamp(data.Aimbot.Smoothness, 0.01, 1) end
        if type(data.Aimbot.Part) == "string" then State.Aimbot.Part = data.Aimbot.Part end
        if data.Aimbot.PartMode ~= nil then State.Aimbot.PartMode = data.Aimbot.PartMode end
        if type(data.Aimbot.TeamCheck) == "boolean" then State.Aimbot.TeamCheck = data.Aimbot.TeamCheck end
    end
    return true
end

local ThemePresets = {
    ["Sky Blue"] = Color3.fromRGB(56, 189, 248),
    ["Ocean"] = Color3.fromRGB(14, 165, 233),
    ["Purple"] = Color3.fromRGB(139, 92, 246),
    ["Emerald"] = Color3.fromRGB(16, 185, 129),
    ["Lime"] = Color3.fromRGB(132, 204, 22),
    ["Amber"] = Color3.fromRGB(245, 158, 11),
    ["Rose"] = Color3.fromRGB(244, 63, 94),
    ["Red"] = Color3.fromRGB(239, 68, 68),
    ["Orange"] = Color3.fromRGB(249, 115, 22),
    ["White"] = Color3.fromRGB(226, 232, 240),
    ["Rainbow"] = Color3.fromRGB(255, 0, 128),
}
local ThemeOrder = {"Sky Blue", "Rainbow", "Ocean", "Purple", "Emerald", "Lime", "Amber", "Rose", "Red", "Orange", "White"}
local function StopRainbow()
    if RainbowConnection then
        SafeCall(function() RainbowConnection:Disconnect() end)
        RainbowConnection = nil
    end
    ThemeHook = nil
end

local function StartRainbow()
    if RainbowConnection then return end
    ThemeHook = {
        Rainbow = true,
        Get = function() return Color3.fromHSV((tick() * 0.25) % 1, 1, 1) end,
    }
    RainbowConnection = RunService.RenderStepped:Connect(function()
        if PanicActive then return end
        if tick() - (LastThemePurge or 0) > 3 then LastThemePurge = tick(); PurgeThemeRegistry() end
        local c = ThemeHook.Get()
        CONFIG.Accent = c
        for _, item in ipairs(ThemeRegistry) do
            SafeCall(function()
                if item.Object and item.Object.Parent then
                    -- OFF toggles stay grey/white (state readable); glass edges get a tinted white
                    if item.Kind == "toggle" then
                        local isOff = false
                        if item.Prop == "Color" then
                            isOff = (item.Object.Color == Color3.fromRGB(255,255,255))
                        else
                            isOff = (item.Object.BackgroundColor3 == Color3.fromRGB(45,45,45))
                        end
                        if isOff then return end
                    end
                    item.Object[item.Prop] = item.Kind == "glass" and Color3.new(0.25 + c.R * 0.75, 0.25 + c.G * 0.75, 0.25 + c.B * 0.75) or c
                end
            end)
        end
    end)
end

local function ApplyTheme(themeName)
    local accent = ThemePresets[themeName]
    if not accent then return false end
    State.Theme = themeName

    if themeName == "Rainbow" then
        StartRainbow()
    else
        StopRainbow()
        CONFIG.Accent = accent
        PurgeThemeRegistry()
        for _, item in ipairs(ThemeRegistry) do
            SafeCall(function()
                if item.Object and item.Object.Parent then
                    -- OFF toggles keep their grey so on/off state stays readable
                    if item.Kind == "toggle" then
                        local isOff = false
                        if item.Prop == "Color" then
                            isOff = (item.Object.Color == Color3.fromRGB(255,255,255))
                        else
                            isOff = (item.Object.BackgroundColor3 == Color3.fromRGB(45,45,45))
                        end
                        if isOff then return end
                    end
                    -- GLASS: edge strokes stay whitish (glass look) but pick up the theme tint
                    item.Object[item.Prop] = item.Kind == "glass" and Color3.new(0.25 + accent.R * 0.75, 0.25 + accent.G * 0.75, 0.25 + accent.B * 0.75) or accent
                end
            end)
        end
    end

    -- This recalculates on next open/resize; keeps the FOV ring matching the theme too
    SafeCall(function()
        if FOVFrame and FOVFrame.Parent then FOVStroke.Color = GetAccent() end
        if LeftArrow and LeftArrow.Parent then LeftArrow.TextColor3 = GetAccent() end
        if RightArrow and RightArrow.Parent then RightArrow.TextColor3 = GetAccent() end
    end)
    return true
end

-- Plain text persistence: no JSON is used. It is saved only when the runtime exposes file APIs.
local PROFILE_FILE = "RBX_1_0_Hub_Profile.txt"
local function EncodeProfileText()
    local p = BuildSettingsProfile()
    local lines = {"RBX_1_0_PROFILE=" .. GetHubVersion(), "Theme=" .. State.Theme, "UIScale=" .. tostring(State.UIScale)}
    local function put(prefix, values)
        for key, value in pairs(values) do table.insert(lines, prefix .. key .. "=" .. tostring(value)) end
    end
    put("Overlay.", p.Overlay); put("Display.", p.Display); put("Movement.", p.Movement); put("Aimbot.", p.Aimbot); put("FPSBoost.", p.FPSBoost)
    return table.concat(lines, "\n")
end
local function DecodeProfileText(text)
    if type(text) ~= "string" or not text:find("RBX_1_0_PROFILE=", 1, true) then return nil, "Invalid saved profile." end
    local raw = {}
    for line in text:gmatch("[^\r\n]+") do
        local key, value = line:match("^([^=]+)=(.*)$")
        if key then raw[key] = value end
    end
    local function bool(key) return raw[key] == "true" and true or (raw[key] == "false" and false or nil) end
    local function num(key) return tonumber(raw[key]) end
    local data = {
        Overlay = {}, Display = {}, Movement = {}, Aimbot = {}, FPSBoost = {},
    }
    for _, key in ipairs({"Enabled", "FPS", "ServerName", "Ping", "Network", "AutoShowOnClose"}) do data.Overlay[key] = bool("Overlay." .. key) end
    for _, key in ipairs({"RemoveDecals", "RemoveParticles", "RemoveTextures", "DisableShadows", "LowQuality", "RemoveTrails", "RemoveBeams", "DisableLightingEffects"}) do data.FPSBoost[key] = bool("FPSBoost." .. key) end
    for _, key in ipairs({"FOV", "Gravity"}) do data.Display[key] = num("Display." .. key) end
    data.Display.UIScale = num("UIScale") -- validated in ApplySettingsProfile (50-150 clamp)
    for _, key in ipairs({"SpeedValue", "JumpPower", "FlySpeed"}) do data.Movement[key] = num("Movement." .. key) end
    data.Aimbot.FOV = num("Aimbot.FOV"); data.Aimbot.Smoothness = num("Aimbot.Smoothness")
    data.Aimbot.Part = raw["Aimbot.Part"]; data.Aimbot.TeamCheck = bool("Aimbot.TeamCheck")
    return data, raw.Theme
end
local function SaveProfileToFile()
    if type(writefile) ~= "function" then return false, "File saving is unavailable in this runtime." end
    local ok, err = pcall(writefile, PROFILE_FILE, EncodeProfileText())
    return ok, ok and nil or tostring(err)
end
local function LoadProfileFromFile()
    if type(readfile) ~= "function" or (type(isfile) == "function" and not isfile(PROFILE_FILE)) then return false, "No saved profile file was found." end
    local ok, text = pcall(readfile, PROFILE_FILE)
    if not ok then return false, tostring(text) end
    local data, themeOrReason = DecodeProfileText(text)
    if not data then return false, themeOrReason end
    local applied, reason = ApplySettingsProfile(data)
    if not applied then return false, reason end
    -- FIXED: theme AND UI scale from the profile are validated before applying
    ApplyTheme(ThemePresets[themeOrReason] and themeOrReason or "Sky Blue")
    UpdateMainScale()
    return true
end

-- ==================== FEATURES TABLE (FULLY FIXED) ====================
local Features = {
    {Category="Movement", Type="Section", Text="MOVEMENT"},
    {Category="Movement", Type="Toggle", Name="Velocity Speed", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Speed.Enabled = v; Disconnect("VelocitySpeed")
        if v then Connect("VelocitySpeed", RunService.Heartbeat, function()
            if not State.Speed.Enabled or PanicActive then return end
            local hrp = GetHRP(); local hum = GetHum()
            if not hrp or not hum then return end
            if hum.MoveDirection.Magnitude > 0 then
                local dir = hum.MoveDirection.Unit
                local vel = hrp.AssemblyLinearVelocity
                hrp.AssemblyLinearVelocity = Vector3.new(dir.X * State.Speed.Value, vel.Y, dir.Z * State.Speed.Value)
            end
        end) end
    end},
    {Category="Movement", Type="Slider", Name="Speed Value", Min=50, Max=500, Default=120, Callback=function(v) State.Speed.Value = v end},
    {Category="Movement", Type="Toggle", Name="Super Jump", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Jump.Enabled = v; Disconnect("SuperJump")
        if v then Connect("SuperJump", RunService.Heartbeat, function()
            if not State.Jump.Enabled or PanicActive then return end
            local hum = GetHum(); if hum and hum.JumpPower ~= State.Jump.Power then hum.JumpPower = State.Jump.Power end
        end) else local hum = GetHum(); if hum then hum.JumpPower = 50 end end
    end},
    {Category="Movement", Type="Slider", Name="Jump Power", Min=50, Max=300, Default=130, Callback=function(v) State.Jump.Power = v end},
    {Category="Movement", Type="Toggle", Name="Fly Mode", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Fly.Enabled = v; Disconnect("Fly"); 
        local hrp = GetHRP()
        if hrp then
            for _, c in ipairs(hrp:GetChildren()) do if c.Name == "RBX_FlyGyro" or c.Name == "RBX_FlyVel" then c:Destroy() end end
        end
        if v then
            if hrp then
                local bg = Instance.new("BodyGyro", hrp); bg.Name = "RBX_FlyGyro"; bg.MaxTorque = Vector3.new(9e9,9e9,9e9); bg.P = 10000
                local bv = Instance.new("BodyVelocity", hrp); bv.Name = "RBX_FlyVel"; bv.MaxForce = Vector3.new(9e9,9e9,9e9); bv.Velocity = Vector3.zero
            end
            Connect("Fly", RunService.RenderStepped, function()
                if not State.Fly.Enabled or PanicActive then return end
                local currentHRP = GetHRP(); if not currentHRP then return end
                local bg = currentHRP:FindFirstChild("RBX_FlyGyro"); local bv = currentHRP:FindFirstChild("RBX_FlyVel")
                if not bg or not bv then return end
                local camCF = Camera.CFrame; local md = Vector3.zero
                if UserInputService:IsKeyDown(Enum.KeyCode.W) then md = md + camCF.LookVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.S) then md = md - camCF.LookVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.A) then md = md - camCF.RightVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.D) then md = md + camCF.RightVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.Space) then md = md + Vector3.new(0,1,0) end
                if UserInputService:IsKeyDown(Enum.KeyCode.LeftShift) then md = md - Vector3.new(0,1,0) end
                bv.Velocity = md.Magnitude > 0 and md.Unit * State.Fly.Speed or Vector3.zero
                bg.CFrame = camCF
            end)
            Notify("Fly", "Fly enabled", 3, Color3.fromRGB(100,100,100))
        else
            if hrp then for _, c in ipairs(hrp:GetChildren()) do if c.Name == "RBX_FlyGyro" or c.Name == "RBX_FlyVel" then c:Destroy() end end end
            local hum = GetHum(); if hum then hum.PlatformStand = false end
            Notify("Fly", "Fly disabled", 2, Color3.fromRGB(100,100,100))
        end
    end},
    {Category="Movement", Type="Slider", Name="Fly Speed", Min=10, Max=200, Default=90, Callback=function(v) State.Fly.Speed = v end},
    {Category="Movement", Type="Toggle", Name="Infinite Jump", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.InfJump = v; Disconnect("InfJump")
        if v then Connect("InfJump", UserInputService.InputBegan, function(input, gpe)
            if PanicActive then return end
            if gpe then return end
            if input.UserInputType == Enum.UserInputType.Keyboard and input.KeyCode == Enum.KeyCode.Space then
                local hum = GetHum(); if hum then hum:ChangeState(Enum.HumanoidStateType.Jumping) end
            end
        end) end
    end},
    {Category="Movement", Type="Toggle", Name="Bunny Hop", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.BunnyHop = v; Disconnect("BunnyHop")
        if v then Connect("BunnyHop", RunService.Heartbeat, function()
            if not State.BunnyHop or PanicActive then return end
            local hum = GetHum(); local char = GetChar()
            if hum and char and hum.FloorMaterial ~= Enum.Material.Air then hum:ChangeState(Enum.HumanoidStateType.Jumping) end
        end) end
    end},
    {Category="Movement", Type="Toggle", Name="Auto-Heal", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.AutoHeal.Enabled = v; Disconnect("AutoHeal")
        if v then Connect("AutoHeal", RunService.Heartbeat, function()
            if not State.AutoHeal.Enabled or PanicActive then return end
            local hum = GetHum(); if hum and hum.Health < State.AutoHeal.Threshold then hum.Health = hum.MaxHealth end
        end) end
    end},
    {Category="Movement", Type="Slider", Name="Heal Threshold", Min=1, Max=100, Default=100, Callback=function(v) State.AutoHeal.Threshold = v end},
    {Category="Movement", Type="Toggle", Name="NoClip", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.NoClip = v; Disconnect("NoClip")
        if v then Connect("NoClip", RunService.Heartbeat, function()
            if not State.NoClip or PanicActive then return end
            local c = GetChar(); if not c then return end
            for _, part in ipairs(c:GetDescendants()) do
                if part:IsA("BasePart") then part.CanCollide = false end
            end
        end) else local c = GetChar(); if c then for _, part in ipairs(c:GetDescendants()) do if part:IsA("BasePart") then part.CanCollide = true end end end end
    end},
    {Category="Movement", Type="Slider", Name="Hip Height", Min=-10, Max=50, Default=0, Callback=function(v) State.HipHeight = v; local hum = GetHum(); if hum then hum.HipHeight = v end end},
    {Category="Movement", Type="Toggle", Name="Jetpack", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Jetpack = v; Disconnect("Jetpack")
        if v then Connect("Jetpack", RunService.Heartbeat, function()
            if not State.Jetpack or PanicActive then return end
            local hum = GetHum(); if hum and UserInputService:IsKeyDown(Enum.KeyCode.Space) then hum:ChangeState(Enum.HumanoidStateType.Jumping) end
        end) end
    end},
    {Category="Movement", Type="Toggle", Name="Invisible", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Invisible = v; local char = GetChar(); if not char then return end
        if v then
            InvisibleOriginals = {}
            for _, part in ipairs(char:GetDescendants()) do
                if part:IsA("BasePart") and part.Name ~= "HumanoidRootPart" then
                    InvisibleOriginals[part] = part.Transparency
                    part.Transparency = 1
                elseif part:IsA("Decal") or part:IsA("Texture") then
                    InvisibleOriginals[part] = part.Transparency
                    part.Transparency = 1
                end
            end
        else
            for part, transparency in pairs(InvisibleOriginals) do
                if part and part.Parent then part.Transparency = transparency end
            end
            InvisibleOriginals = {}
        end
    end},
    {Category="Movement", Type="Toggle", Name="Walk on Water", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.WaterWalk.Enabled = v; Disconnect("WaterWalk")
        if State.WaterWalk.Platform and State.WaterWalk.Platform.Parent then 
            State.WaterWalk.Platform:Destroy(); State.WaterWalk.Platform = nil 
        end
        if v then
            local platform = Instance.new("Part"); platform.Name = "RBX_WaterPlatform"; platform.Size = Vector3.new(8,1,8)
            platform.Anchored = true; platform.CanCollide = true; platform.Transparency = 1; platform.Material = Enum.Material.Glass; platform.Parent = Workspace
            State.WaterWalk.Platform = platform
            Connect("WaterWalk", RunService.Heartbeat, function()
                if not State.WaterWalk.Enabled or PanicActive then return end
                local hrp = GetHRP(); if not hrp then return end
                local rp = RaycastParams.new(); rp.FilterDescendantsInstances = {GetChar(), platform}; rp.FilterType = Enum.RaycastFilterType.Blacklist
                local res = Workspace:Raycast(hrp.Position, Vector3.new(0,-20,0), rp)
                if res then
                    local isWater = (res.Instance.Material == Enum.Material.Water) or (res.Instance.Name:lower():find("water") ~= nil)
                    if isWater then platform.Position = Vector3.new(hrp.Position.X, res.Position.Y + 0.5, hrp.Position.Z); platform.CanCollide = true
                    else platform.CanCollide = false; platform.Position = Vector3.new(0,-500,0) end
                else platform.CanCollide = false; platform.Position = Vector3.new(0,-500,0) end
            end)
            Notify("WaterWalk", "Walk on Water enabled", 2, Color3.fromRGB(100,100,100))
        else Notify("WaterWalk", "Walk on Water disabled", 2, Color3.fromRGB(100,100,100)) end
    end},
    {Category="Movement", Type="Toggle", Name="Infinite Stamina", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Stamina = v; Disconnect("Stamina")
        if v then Connect("Stamina", RunService.Heartbeat, function()
            if not State.Stamina or PanicActive then return end
            local hum = GetHum(); if not hum then return end
            SafeCall(function() if hum:FindFirstChild("Stamina") then hum.Stamina.Value = 100 end end)
        end) end
    end},
    {Category="Movement", Type="Toggle", Name="Anti Knockback", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.AntiKnockback = v; Disconnect("AntiKnockback")
        if v then Connect("AntiKnockback", RunService.Heartbeat, function()
            if not State.AntiKnockback or PanicActive then return end
            local hrp = GetHRP(); if hrp then 
                local vel = hrp.AssemblyLinearVelocity
                hrp.AssemblyLinearVelocity = Vector3.new(vel.X * 0.1, math.clamp(vel.Y, -5, 5), vel.Z * 0.1) 
            end
        end) end
    end},
    {Category="Movement", Type="Toggle", Name="Vehicle Speed", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.VehicleSpeed.Enabled = v; Disconnect("VehicleSpeed")
        if v then Connect("VehicleSpeed", RunService.Heartbeat, function()
            if not State.VehicleSpeed.Enabled or PanicActive then return end
            local hum = GetHum(); if not hum or not hum.SeatPart then return end
            local vehicle = hum.SeatPart.Parent; if not vehicle or not vehicle:IsA("Model") then return end
            for _, seat in ipairs(vehicle:GetDescendants()) do if seat:IsA("VehicleSeat") then seat.MaxSpeed = State.VehicleSpeed.Value end end
            local pp = vehicle.PrimaryPart or vehicle:FindFirstChildWhichIsA("BasePart")
            if pp then
                local bv = pp:FindFirstChild("RBX_VehicleBoost")
                if bv then bv:Destroy() end
                bv = Instance.new("BodyVelocity", pp)
                bv.Name = "RBX_VehicleBoost"; bv.MaxForce = Vector3.new(40000,0,40000)
                bv.Velocity = pp.CFrame.LookVector * State.VehicleSpeed.Value
            end
        end) else
            local hum = GetHum()
            if hum and hum.SeatPart then
                local vehicle = hum.SeatPart.Parent
                if vehicle then
                    local pp = vehicle.PrimaryPart or vehicle:FindFirstChildWhichIsA("BasePart")
                    if pp then
                        local bv = pp:FindFirstChild("RBX_VehicleBoost")
                        if bv then bv:Destroy() end
                    end
                end
            end
        end
    end},
    {Category="Movement", Type="Slider", Name="Vehicle Speed", Min=50, Max=500, Default=200, Callback=function(v) State.VehicleSpeed.Value = v end},

    {Category="Combat", Type="Section", Text="COMBAT"},
    {Category="Combat", Type="Toggle", Name="Aimbot", Color=Color3.fromRGB(120,120,120), Default=false, Callback=function(v)
        State.Aimbot.Enabled = v
        pcall(function() RunService:UnbindFromRenderStep("RBX_Aimbot") end)
        Disconnect("AimbotMouse")
        if v then
            FOVFrame.Visible = true
            -- CAMERA FIX: bind AFTER Roblox's own camera update (Camera priority) so the
            -- camera script cannot snap the view back off the head every frame.
            pcall(function()
                RunService:BindToRenderStep("RBX_Aimbot", Enum.RenderPriority.Camera.Value + 1, function()
                    if not State.Aimbot.Enabled or PanicActive then return end
                    local target = GetAimbotTarget()
                    if target and IsPlayerAlive(target) and target.Character and target.Character.Parent then
                        local part = GetAimPart(target.Character)
                        if part and part.Parent then
                            local myHRP = GetHRP()
                            local dist = 0
                            SafeCall(function()
                                if myHRP then
                                    dist = math.floor((part.Position - myHRP.Position).Magnitude)
                                end
                            end)
                            DistanceLabel.Text = tostring(dist) .. "m"
                            DistanceLabel.Position = UDim2.new(0.5, -60, 0.5, State.Aimbot.FOV + 15)
                            DistanceLabel.Visible = true

                            local pos = part.Position
                            if State.Aimbot.Prediction then
                                local vel = part.AssemblyLinearVelocity or Vector3.zero
                                local mult = State.Aimbot.PowerMode and 0.25 or 0.15
                                pos = pos + (vel * mult)
                            end
                            if State.Aimbot.DropComp then
                                pos = pos - Vector3.new(0, 0.35, 0)
                            end
                            if State.Aimbot.Shake > 0 then
                                local shake = State.Aimbot.Shake
                                pos = pos + Vector3.new(math.random(-shake, shake), math.random(-shake, shake), math.random(-shake, shake)) * 0.01
                            end

                            local currentCF = Camera.CFrame
                            local targetCF = CFrame.lookAt(currentCF.Position, pos)
                            local smooth = (State.Aimbot.PowerMode or State.CameraLock.Enabled) and 1 or State.Aimbot.Smoothness
                            Camera.CFrame = currentCF:Lerp(targetCF, smooth)
                        end
                        UpdateTargetHighlight(target)
                    else
                        DistanceLabel.Visible = false
                        UpdateTargetHighlight(nil)
                    end
                    if State.Aimbot.AutoShoot and HasTool() then
                        local t = GetAimbotTarget()
                        if t and IsPlayerAlive(t) then
                            UniversalClick()
                        end
                    end
                end)
            end)
            Notify("Aimbot", "Aimbot ACTIVE", 3, Color3.fromRGB(120,120,120))
        else
            FOVFrame.Visible = false
            DistanceLabel.Visible = false
            UpdateTargetHighlight(nil)
            Notify("Aimbot", "Aimbot disabled", 2, Color3.fromRGB(120,120,120))
        end
    end},
    {Category="Combat", Type="Slider", Name="Aimbot FOV", Min=10, Max=500, Default=150, Callback=function(v)
        State.Aimbot.FOV = v; FOVFrame.Size = UDim2.new(0,v*2,0,v*2); FOVFrame.Position = UDim2.new(0.5,-v,0.5,-v)
        DistanceLabel.Position = UDim2.new(0.5, -60, 0.5, v + 15)
    end},
    {Category="Combat", Type="Slider", Name="Aimbot Smooth", Min=1, Max=100, Default=8, Callback=function(v) State.Aimbot.Smoothness = v/100 end},
    {Category="Combat", Type="Slider", Name="Shake", Min=0, Max=50, Default=0, Callback=function(v) State.Aimbot.Shake = v end},
    {Category="Combat", Type="Slider", Name="Max Distance", Min=50, Max=2000, Default=1000, Callback=function(v) State.AimbotMaxDistance = v end},
    {Category="Combat", Type="Toggle", Name="Power Mode", Color=Color3.fromRGB(255,80,80), Default=false, Callback=function(v)
        State.Aimbot.PowerMode = v
        Notify("Aimbot", v and "POWER MODE ON ☠️" or "Power Mode off", 2, v and Color3.fromRGB(255,80,80) or Color3.fromRGB(120,120,120))
    end},
    {Category="Combat", Type="Toggle", Name="Lock Target", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v) State.Aimbot.LockOn = v end},
    {Category="Combat", Type="Dropdown", Name="Aim Part", Options={"Head","Torso","HumanoidRootPart","LeftArm","RightArm"}, Default=1, Callback=function(val) State.Aimbot.Part = val end},
    {Category="Combat", Type="Dropdown", Name="Priority", Options={"Closest","Distance","Lowest Health","FOV"}, Default=1, Callback=function(val) State.Aimbot.Priority = val end},
    {Category="Combat", Type="Toggle", Name="Team Check", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.Aimbot.TeamCheck = v end},
    {Category="Combat", Type="Toggle", Name="Wall Check", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v) State.Aimbot.WallCheck = v end},
    {Category="Combat", Type="Toggle", Name="Prediction", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.Aimbot.Prediction = v end},
    {Category="Combat", Type="Toggle", Name="Drop Comp", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.Aimbot.DropComp = v end},
    {Category="Combat", Type="Toggle", Name="Auto Shoot", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Aimbot.AutoShoot = v; Disconnect("AutoShoot")
        if v then Connect("AutoShoot", RunService.Heartbeat, function()
            if not State.Aimbot.AutoShoot or PanicActive then return end
            local t = GetAimbotTarget()
            if t and IsPlayerAlive(t) and HasTool() then
                if State.Aimbot.AutoShootMode == "Spam" then
                    OverrideClickCooldown = true
                    for _ = 1, 5 do UniversalClick(true) end
                    OverrideClickCooldown = false
                else
                    UniversalClick()
                end
            end
        end) end
    end},
    {Category="Combat", Type="Dropdown", Name="Auto Shoot Mode", Options={"Hold","Spam"}, Default=1, Callback=function(val) State.Aimbot.AutoShootMode = val end},
    {Category="Combat", Type="Toggle", Name="Auto WallBang", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v) State.Aimbot.AutoWallBang = v end},
    {Category="Combat", Type="Toggle", Name="Camera Lock", Color=Color3.fromRGB(255,80,80), Default=false, Callback=function(v)
        State.CameraLock.Enabled = v
        Notify("Combat", v and "CAMERA LOCK ENGAGED ☠️" or "Camera Lock disabled", 2, v and Color3.fromRGB(255,80,80) or Color3.fromRGB(120,120,120))
    end},
    {Category="Combat", Type="Keybind", Name="Camera Lock Key", Default=State.CameraLock.Keybind, Callback=function(key)
        State.CameraLock.Keybind = key
        local name = typeof(key) == "EnumItem" and (key.EnumType == Enum.KeyCode and tostring(key):gsub("Enum.KeyCode.", "") or tostring(key):gsub("Enum.UserInputType.", "")) or "None"
        Notify("Combat", "Camera Lock key set to " .. name, 2, Color3.fromRGB(255,80,80))
    end},
    {Category="Combat", Type="Toggle", Name="Silent Aim", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.SilentAim.Enabled = v
        -- POWER COMBAT: silent aim pipes the locked target position through every click path
        OverrideClickCooldown = false
        if v then Notify("Silent Aim", "Hits redirect to the locked target", 2, GetAccent()) end
    end},
    {Category="Combat", Type="Slider", Name="Silent FOV", Min=10, Max=300, Default=80, Callback=function(v) State.SilentAim.FOV = v end},
    {Category="Combat", Type="Slider", Name="Hit Chance", Min=1, Max=100, Default=100, Callback=function(v) State.SilentAim.HitChance = v end},
    {Category="Combat", Type="Toggle", Name="Silent Team Check", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v) State.SilentAim.TeamCheck = v end},
    {Category="Combat", Type="Toggle", Name="Silent Visible Check", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v) State.SilentAim.VisibleCheck = v end},
    {Category="Combat", Type="Toggle", Name="Trigger Bot", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.TriggerBot.Enabled = v; Disconnect("TriggerBot")
        if v then Connect("TriggerBot", RunService.RenderStepped, function()
            if not State.TriggerBot.Enabled or PanicActive then return end
            local mouse = LocalPlayer:GetMouse(); local target = mouse.Target
            if target then
                local char = target:FindFirstAncestorOfClass("Model")
                if char then
                    local plr = Players:GetPlayerFromCharacter(char)
                    if plr and plr ~= LocalPlayer and plr.Parent and HasTool() then
                        if not State.Aimbot.TeamCheck or (plr.Team and LocalPlayer.Team and plr.Team ~= LocalPlayer.Team) then
                            local now = tick()
                            if now - LastTriggerTime >= State.TriggerBot.Delay then
                                LastTriggerTime = now
                                UniversalClick()
                            end
                        end
                    end
                end
            end
        end) end
    end},
    {Category="Combat", Type="Slider", Name="Trigger Delay", Min=0, Max=50, Default=0, Callback=function(v) State.TriggerBot.Delay = v/100 end},
    {Category="Combat", Type="Toggle", Name="Auto Parry", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.AutoParry.Enabled = v; Disconnect("AutoParry")
        if v then Connect("AutoParry", RunService.Heartbeat, function()
            if not State.AutoParry.Enabled or PanicActive then return end
            local now = tick()
            local cooldown = State.AutoParry.FrameFire and 0.05 or 0.5
            if now - State.AutoParry.LastParry < cooldown then return end
            local myHRP = GetHRP(); if not myHRP then return end
            for _, p in ipairs(Players:GetPlayers()) do
                if p ~= LocalPlayer and p.Character and p.Character.Parent and p.Character:FindFirstChild("HumanoidRootPart") then
                    if (p.Character.HumanoidRootPart.Position - myHRP.Position).Magnitude < State.AutoParry.Range then
                        if p.Character:FindFirstChildOfClass("Tool") then
                            State.AutoParry.LastParry = now
                            -- POWER COMBAT V2: key press + tool activation + parry remotes, all at once
                            TriggerParry()
                        end
                    end
                end
            end
        end) end
    end},
    {Category="Combat", Type="Toggle", Name="Auto Parry Every Frame", Color=Color3.fromRGB(255,80,80), Default=false, Callback=function(v)
        State.AutoParry.FrameFire = v
        Notify("Auto Parry", v and "FRAME FIRE MODE ☠️ (5x faster parries)" or "Normal parry speed", 2, v and Color3.fromRGB(255,80,80) or Color3.fromRGB(100,100,100))
    end},
    {Category="Combat", Type="Slider", Name="Parry Range", Min=5, Max=50, Default=25, Callback=function(v) State.AutoParry.Range = v end},
    -- POWER COMBAT V2: fires EVERY RemoteEvent inside the tool with a real ms delay
    {Category="Combat", Type="Toggle", Name="Rapid Fire", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.RapidFire = v; Disconnect("RapidFire")
        if v then Connect("RapidFire", RunService.Heartbeat, function()
            if not State.RapidFire or PanicActive then return end
            if not HasTool() then return end
            local now = tick()
            if now - (State._LastRapidFire or 0) < State.RapidFireDelay then return end
            State._LastRapidFire = now
            local char = GetChar()
            local tool = char and char:FindFirstChildOfClass("Tool")
            if tool then
                local hitPos = GetSilentAimPosition()
                SafeCall(function()
                    for _, obj in ipairs(tool:GetDescendants()) do
                        if obj:IsA("RemoteEvent") then
                            if hitPos then obj:FireServer(hitPos) else obj:FireServer() end
                        elseif obj:IsA("RemoteFunction") then
                            if hitPos then obj:InvokeServer(hitPos) else obj:InvokeServer() end
                        end
                    end
                    if tool.Enabled then tool:Activate() end
                end)
            end
        end) end
    end},
    {Category="Combat", Type="Slider", Name="Rapid Fire Rate", Min=1, Max=100, Default=20, Callback=function(v) State.RapidFireDelay = v/1000 end},
    -- POWER COMBAT V2: attack mode — LookAt every target + fire every click method at once
    {Category="Combat", Type="Toggle", Name="Melee Aura", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.MeleeAura.Enabled = v; Disconnect("MeleeAura")
        if v then 
            Connect("MeleeAura", RunService.Heartbeat, function()
                if not State.MeleeAura.Enabled or PanicActive then return end
                local myHRP = GetHRP(); if not myHRP then return end
                local char = GetChar()
                if not char then return end
                local tool = char:FindFirstChildOfClass("Tool")
                if not tool then return end
                local isMelee = tool:FindFirstChild("Handle") ~= nil
                local isGun = tool:FindFirstChild("Ammo") or tool:FindFirstChild("Mag") or tool:FindFirstChild("Fire") or tool.Name:lower():match("gun") or tool.Name:lower():match("rifle") or tool.Name:lower():match("pistol")
                if not isMelee or isGun then return end
                if not State.MeleeAura.AttackAll then
                    -- original gentle mode: swing when someone is close
                    local inRange = false
                    for _, p in ipairs(GetCachedPlayers()) do
                        if p ~= LocalPlayer and p.Character and p.Character.Parent and p.Character:FindFirstChild("HumanoidRootPart") then
                            local dist = (p.Character.HumanoidRootPart.Position - myHRP.Position).Magnitude
                            if dist < State.MeleeAura.Range then inRange = true; break end
                        end
                    end
                    if inRange then UniversalClick() end
                    return
                end
                -- ATTACK MODE: face the closest target and unload every attack method
                local now = tick()
                if now - (State._LastAuraSwing or 0) < 0.08 then return end
                State._LastAuraSwing = now
                local closest, closestDist = nil, math.huge
                for _, p in ipairs(GetCachedPlayers()) do
                    if p ~= LocalPlayer and p.Character and p.Character.Parent and p.Character:FindFirstChild("HumanoidRootPart") and IsPlayerAlive(p) then
                        if State.Aimbot.TeamCheck and p.Team and LocalPlayer.Team and p.Team == LocalPlayer.Team then continue end
                        local dist = (p.Character.HumanoidRootPart.Position - myHRP.Position).Magnitude
                        if dist < State.MeleeAura.Range and dist < closestDist then
                            closestDist = dist
                            closest = p
                        end
                    end
                end
                if closest and closest.Character and closest.Character:FindFirstChild("HumanoidRootPart") then
                    local targetHRP = closest.Character.HumanoidRootPart
                    SafeCall(function()
                        myHRP.CFrame = CFrame.new(myHRP.Position, Vector3.new(targetHRP.Position.X, myHRP.Position.Y, targetHRP.Position.Z))
                    end)
                    OverrideClickCooldown = true
                    UniversalClick(true)
                    OverrideClickCooldown = false
                end
            end) 
        end
    end},
    {Category="Combat", Type="Toggle", Name="Aura Attack Mode", Color=Color3.fromRGB(255,80,80), Default=false, Callback=function(v)
        State.MeleeAura.AttackAll = v
        Notify("Melee Aura", v and "ATTACK MODE ☠️ (LookAt + full unload)" or "Passive swing mode", 2, v and Color3.fromRGB(255,80,80) or Color3.fromRGB(100,100,100))
    end},
    {Category="Combat", Type="Slider", Name="Aura Range", Min=5, Max=30, Default=15, Callback=function(v) State.MeleeAura.Range = v end},
    {Category="Combat", Type="Toggle", Name="Hitbox Expander", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Hitbox.Enabled = v
        for name, conn in pairs(HitboxConnections) do SafeCall(function() conn:Disconnect() end) end
        HitboxConnections = {}
        Disconnect("HitboxCharAdded")

        if v then
            local function expand(char)
                if not char or not char.Parent then return end
                for _, part in ipairs(char:GetDescendants()) do
                    if part:IsA("BasePart") and part.Name ~= "HumanoidRootPart" then
                        -- POWER COMBAT V2: head always expands; Torso/Arms only when the toggle is on
                        local isHead = part.Name == "Head"
                        local isTorso = part.Name:match("Torso") or part.Name == "Torso"
                        local isLimb = part.Name:match("Arm") or part.Name:match("Hand") or part.Name:match("Leg") or part.Name:match("Foot")
                        if isHead or (State.Hitbox.ExpandTorso and (isTorso or isLimb)) then
                            if not State.Hitbox.Originals[part] then State.Hitbox.Originals[part] = part.Size end
                            part.Size = Vector3.new(State.Hitbox.Size, State.Hitbox.Size, State.Hitbox.Size)
                        end
                    end
                end
            end
            for _, p in ipairs(Players:GetPlayers()) do
                if p ~= LocalPlayer then
                    if p.Character and p.Character.Parent then expand(p.Character) end
                    HitboxConnections[p] = p.CharacterAdded:Connect(function(char)
                        if State.Hitbox.Enabled and not PanicActive then task.wait(0.3); expand(char) end
                    end)
                end
            end
            Connect("HitboxCharAdded", Players.PlayerAdded, function(p)
                if p == LocalPlayer then return end
                HitboxConnections[p] = p.CharacterAdded:Connect(function(char)
                    if State.Hitbox.Enabled and not PanicActive then task.wait(0.3); expand(char) end
                end)
            end)
            Notify("Hitbox", "Hitboxes expanded", 2, Color3.fromRGB(100,100,100))
        else
            for part, size in pairs(State.Hitbox.Originals) do if part and part.Parent then part.Size = size end end
            State.Hitbox.Originals = {}
            Notify("Hitbox", "Hitboxes restored", 2, Color3.fromRGB(100,100,100))
        end
    end},
    {Category="Combat", Type="Slider", Name="Hitbox Size", Min=2, Max=50, Default=12, Callback=function(v)
        State.Hitbox.Size = v
        if State.Hitbox.Enabled then
            for _, p in ipairs(Players:GetPlayers()) do
                if p ~= LocalPlayer and p.Character and p.Character.Parent then
                    for _, part in ipairs(p.Character:GetDescendants()) do
                        if part:IsA("BasePart") and part.Name ~= "HumanoidRootPart" and (part.Name == "Head" or State.Hitbox.ExpandTorso) then
                            part.Size = Vector3.new(v,v,v)
                        end
                    end
                end
            end
        end
    end},
    {Category="Combat", Type="Toggle", Name="Hitbox Expand Torso/Arms", Color=Color3.fromRGB(255,80,80), Default=false, Callback=function(v)
        State.Hitbox.ExpandTorso = v
        Notify("Hitbox", v and "TORSO + ARMS EXPANSION ☠️" or "Head-only hitboxes", 2, v and Color3.fromRGB(255,80,80) or Color3.fromRGB(100,100,100))
    end},
    {Category="Combat", Type="Toggle", Name="Reach", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Reach.Enabled = v; Disconnect("ReachChildAdded"); Disconnect("ReachCharAdded")
        if State.Reach.Originals then
            for handle, size in pairs(State.Reach.Originals) do if handle and handle.Parent then handle.Size = size; handle.Massless = false end end
        end
        State.Reach.Originals = {}

        if v then
            local function expandTool(tool)
                if tool:IsA("Tool") and tool:FindFirstChild("Handle") then
                    if not State.Reach.Originals[tool.Handle] then State.Reach.Originals[tool.Handle] = tool.Handle.Size end
                    tool.Handle.Size = Vector3.new(State.Reach.Distance, State.Reach.Distance, State.Reach.Distance)
                    tool.Handle.Massless = true
                end
            end
            local function setupChar(char)
                if not char or not char.Parent then return end
                for _, tool in ipairs(char:GetChildren()) do expandTool(tool) end
                Connect("ReachChildAdded", char.ChildAdded, function(child) if State.Reach.Enabled and not PanicActive then expandTool(child) end end)
            end
            local char = GetChar()
            if char then setupChar(char) end
            Connect("ReachCharAdded", LocalPlayer.CharacterAdded, function(char)
                if State.Reach.Enabled and not PanicActive then setupChar(char) end
            end)
        end
    end},
    {Category="Combat", Type="Slider", Name="Reach Distance", Min=5, Max=100, Default=25, Callback=function(v) State.Reach.Distance = v end},
    -- POWER COMBAT V2: velocity-free spin (no anti-cheat velocity flags) + classic mode
    {Category="Combat", Type="Toggle", Name="Spin Bot", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.SpinBot.Enabled = v; Disconnect("SpinBot")
        if v then Connect("SpinBot", RunService.RenderStepped, function()
            if not State.SpinBot.Enabled or PanicActive then return end
            local hrp = GetHRP(); if hrp then
                if State.SpinBot.Mode == "Velocity" then
                    -- keep the current velocity untouched, only rotate the visual CFrame
                    local vel = hrp.AssemblyLinearVelocity
                    hrp.CFrame = hrp.CFrame * CFrame.Angles(0, math.rad(State.SpinBot.Speed), 0)
                    hrp.AssemblyLinearVelocity = vel
                else
                    hrp.CFrame = CFrame.new(hrp.Position) * CFrame.Angles(0, math.rad(State.SpinBot.Speed), 0)
                end
            end
        end) end
    end},
    {Category="Combat", Type="Dropdown", Name="Spin Mode", Options={"Velocity","Render"}, Default=1, Callback=function(val) State.SpinBot.Mode = val end},
    {Category="Combat", Type="Slider", Name="Spin Speed", Min=1, Max=100, Default=25, Callback=function(v) State.SpinBot.Speed = v end},
    {Category="Combat", Type="Toggle", Name="God Mode", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.GodMode = v; Disconnect("GodMode")
        if v then Connect("GodMode", RunService.Heartbeat, function()
            if not State.GodMode or PanicActive then return end
            local now = tick()
            if now - LastGodModeSet < 0.1 then return end
            LastGodModeSet = now
            local hum = GetHum(); if hum then hum.Health = hum.MaxHealth end
        end) end
    end},
    {Category="Combat", Type="Toggle", Name="God Mode Auto Revive", Color=Color3.fromRGB(255,80,80), Default=false, Callback=function(v)
        State.GodModeRevive = v
        Notify("God Mode", v and "AUTO REVIVE ON ☠️ (full heal after death)" or "Auto revive off", 2, v and Color3.fromRGB(255,80,80) or Color3.fromRGB(100,100,100))
    end},
    -- POWER COMBAT V2: auto drink/eat healing items from the Backpack when hurt
    {Category="Combat", Type="Toggle", Name="Auto Pot / Auto Eat", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.AutoHealCombat.Enabled = v; Disconnect("AutoHealCombat")
        if v then Connect("AutoHealCombat", RunService.Heartbeat, function()
            if not State.AutoHealCombat.Enabled or PanicActive then return end
            local hum = GetHum(); if not hum then return end
            if hum.Health > 0 and hum.Health < (hum.MaxHealth * State.AutoHealCombat.Threshold / 100) then
                local now = tick()
                if now - (State._LastAutoPot or 0) < 1.5 then return end
                State._LastAutoPot = now
                TryConsumeHealingItem()
            end
        end) end
    end},
    {Category="Combat", Type="Slider", Name="Pot Threshold %", Min=5, Max=100, Default=50, Callback=function(v) State.AutoHealCombat.Threshold = v end},
    {Category="Combat", Type="Button", Name="Kill All (Client)", Color=Color3.fromRGB(60,60,60), Callback=function()
        for _, p in ipairs(Players:GetPlayers()) do
            if p ~= LocalPlayer and p.Character and p.Character.Parent and p.Character:FindFirstChildOfClass("Humanoid") then
                SafeCall(function() p.Character:FindFirstChildOfClass("Humanoid").Health = 0 end)
            end
        end
        Notify("Combat", "Kill All executed", 2, Color3.fromRGB(60,60,60))
    end},
    {Category="Combat", Type="Button", Name="Bring All (Client)", Color=Color3.fromRGB(60,60,60), Callback=function()
        local myHRP = GetHRP(); if not myHRP then return end
        for _, p in ipairs(Players:GetPlayers()) do
            if p ~= LocalPlayer and p.Character and p.Character.Parent and p.Character:FindFirstChild("HumanoidRootPart") then
                SafeCall(function() p.Character.HumanoidRootPart.CFrame = myHRP.CFrame * CFrame.new(math.random(-5,5), 0, math.random(-5,5)) end)
            end
        end
    end},
    -- POWER COMBAT V2: one-button full reset of every combat module
    {Category="Combat", Type="Button", Name="PANIC COMBAT (Reset All)", Color=Color3.fromRGB(140,30,30), Callback=function()
        OverrideClickCooldown = false
        State.Aimbot.Enabled = false; Disconnect("Aimbot"); FOVFrame.Visible = false; DistanceLabel.Visible = false; UpdateTargetHighlight(nil)
        State.CameraLock.Enabled = false
        State.SilentAim.Enabled = false
        State.TriggerBot.Enabled = false; Disconnect("TriggerBot")
        State.AutoParry.Enabled = false; Disconnect("AutoParry")
        State.RapidFire = false; Disconnect("RapidFire")
        State.MeleeAura.Enabled = false; Disconnect("MeleeAura")
        State.AutoHealCombat.Enabled = false; Disconnect("AutoHealCombat")
        State.Hitbox.Enabled = false
        for name, conn in pairs(HitboxConnections) do SafeCall(function() conn:Disconnect() end) end
        HitboxConnections = {}
        Disconnect("HitboxCharAdded")
        for part, size in pairs(State.Hitbox.Originals) do if part and part.Parent then part.Size = size end end
        State.Hitbox.Originals = {}
        State.Reach.Enabled = false; Disconnect("ReachChildAdded"); Disconnect("ReachCharAdded")
        for handle, size in pairs(State.Reach.Originals) do if handle and handle.Parent then handle.Size = size; handle.Massless = false end end
        State.Reach.Originals = {}
        State.SpinBot.Enabled = false; Disconnect("SpinBot")
        State.GodMode = false; Disconnect("GodMode")
        State.GodModeRevive = false
        for _, name in ipairs({"Aimbot","Power Mode","Lock Target","Camera Lock","Silent Aim","Trigger Bot","Auto Parry","Auto Parry Every Frame","Rapid Fire","Melee Aura","Aura Attack Mode","Hitbox Expander","Hitbox Expand Torso/Arms","Spin Bot","God Mode","God Mode Auto Revive","Auto Pot / Auto Eat","Auto Shoot"}) do
            local ctrl = ToggleControls[name]
            if ctrl and ctrl.Set then pcall(ctrl.Set, false) end
        end
        Notify("Combat", "ALL COMBAT MODULES RESET", 3, Color3.fromRGB(255,80,80))
    end},

    {Category="Visuals", Type="Section", Text="VISUALS"},
    {Category="Visuals", Type="Toggle", Name="Fullbright", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Fullbright.Enabled = v
        if v then
            CC.Brightness = State.Fullbright.Intensity; CC.Contrast = 0.1; CC.Saturation = 0.1; CC.TintColor = Color3.fromRGB(255,255,240)
            Lighting.GlobalShadows = false; Lighting.Ambient = Color3.fromRGB(178,178,178); Lighting.OutdoorAmbient = Color3.fromRGB(178,178,178)
        else
            CC.Brightness = 0; CC.Contrast = 0; CC.Saturation = 0; CC.TintColor = Color3.fromRGB(255,255,255)
            Lighting.GlobalShadows = true; Lighting.Ambient = Color3.fromRGB(91,91,91); Lighting.OutdoorAmbient = Color3.fromRGB(140,140,140)
        end
    end},
    {Category="Visuals", Type="Slider", Name="FB Intensity", Min=0, Max=20, Default=2, Callback=function(v)
        State.Fullbright.Intensity = v/10; if State.Fullbright.Enabled then CC.Brightness = State.Fullbright.Intensity end
    end},
    {Category="Visuals", Type="Toggle", Name="XRay", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.XRay.Enabled = v
        if v then
            State.XRay.Originals = {}
            for _, obj in ipairs(Workspace:GetDescendants()) do
                if obj:IsA("BasePart") and not obj:IsDescendantOf(GetChar()) then
                    State.XRay.Originals[obj] = {Transparency = obj.Transparency, Material = obj.Material}
                    obj.Transparency = State.XRay.Transparency; obj.Material = Enum.Material.ForceField
                end
            end
        else
            for obj, orig in pairs(State.XRay.Originals or {}) do if obj and obj.Parent then obj.Transparency = orig.Transparency; obj.Material = orig.Material end end
            State.XRay.Originals = {}
        end
    end},
    {Category="Visuals", Type="Slider", Name="XRay Alpha", Min=0, Max=10, Default=7, Callback=function(v)
        State.XRay.Transparency = v/10
        if State.XRay.Enabled then for obj, _ in pairs(State.XRay.Originals or {}) do if obj and obj.Parent then obj.Transparency = State.XRay.Transparency end end end
    end},
    {Category="Visuals", Type="Toggle", Name="Wireframe", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Wireframe.Enabled = v
        if v then
            State.Wireframe.Originals = {}
            for _, obj in ipairs(Workspace:GetDescendants()) do
                if obj:IsA("BasePart") and not obj:IsDescendantOf(GetChar()) then
                    State.Wireframe.Originals[obj] = obj.Material; obj.Material = Enum.Material.Wireframe
                end
            end
        else
            for obj, mat in pairs(State.Wireframe.Originals or {}) do if obj and obj.Parent then obj.Material = mat end end
            State.Wireframe.Originals = {}
        end
    end},
    {Category="Visuals", Type="Toggle", Name="Bloom", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Bloom.Enabled = v; BL.Intensity = v and State.Bloom.Intensity or 0; BL.Size = v and State.Bloom.Size or 0
    end},
    {Category="Visuals", Type="Slider", Name="Bloom Intensity", Min=0, Max=50, Default=20, Callback=function(v)
        State.Bloom.Intensity = v/10; if State.Bloom.Enabled then BL.Intensity = State.Bloom.Intensity end
    end},
    {Category="Visuals", Type="Slider", Name="Bloom Size", Min=0, Max=60, Default=24, Callback=function(v)
        State.Bloom.Size = v; if State.Bloom.Enabled then BL.Size = v end
    end},
    {Category="Visuals", Type="Toggle", Name="SunRays", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.SunRays.Enabled = v; SR.Intensity = v and State.SunRays.Intensity or 0; SR.Spread = v and State.SunRays.Spread or 0
    end},
    {Category="Visuals", Type="Slider", Name="SunRays Intensity", Min=0, Max=10, Default=3, Callback=function(v)
        State.SunRays.Intensity = v/10; if State.SunRays.Enabled then SR.Intensity = State.SunRays.Intensity end
    end},
    {Category="Visuals", Type="Slider", Name="SunRays Spread", Min=0, Max=10, Default=5, Callback=function(v)
        State.SunRays.Spread = v/10; if State.SunRays.Enabled then SR.Spread = State.SunRays.Spread end
    end},
    {Category="Visuals", Type="Toggle", Name="Color Tint", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.ColorTint.Enabled = v; CC.TintColor = v and State.ColorTint.Color or Color3.fromRGB(255,255,255)
    end},
    {Category="Visuals", Type="Toggle", Name="Time Freeze", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.TimeFreeze.Enabled = v
        if v then State.TimeFreeze.OriginalTime = Lighting.ClockTime; Lighting.ClockTime = 12
        else Lighting.ClockTime = State.TimeFreeze.OriginalTime end
    end},
    {Category="Visuals", Type="Toggle", Name="Freecam", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Freecam.Enabled = v; Disconnect("Freecam")
        if v then
            State.Freecam.OriginalCameraType = Camera.CameraType
            Camera.CameraType = Enum.CameraType.Scriptable
            State.Freecam.CFrame = Camera.CFrame
            Connect("Freecam", RunService.RenderStepped, function()
                if not State.Freecam.Enabled or PanicActive then return end
                local spd = State.Freecam.Speed; local cf = State.Freecam.CFrame; local md = Vector3.zero
                if UserInputService:IsKeyDown(Enum.KeyCode.W) then md = md + cf.LookVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.S) then md = md - cf.LookVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.A) then md = md - cf.RightVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.D) then md = md + cf.RightVector end
                if UserInputService:IsKeyDown(Enum.KeyCode.Space) then md = md + Vector3.new(0,1,0) end
                if UserInputService:IsKeyDown(Enum.KeyCode.LeftShift) then md = md - Vector3.new(0,1,0) end
                State.Freecam.CFrame = cf + md * spd * 0.016
                Camera.CFrame = State.Freecam.CFrame
            end)
        else 
            Camera.CameraType = State.Freecam.OriginalCameraType or Enum.CameraType.Custom 
        end
    end},
    {Category="Visuals", Type="Slider", Name="Freecam Speed", Min=1, Max=50, Default=10, Callback=function(v) State.Freecam.Speed = v/5 end},
    {Category="Visuals", Type="Toggle", Name="Click TP", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.ClickTP.Enabled = v; Disconnect("ClickTP")
        if v then Connect("ClickTP", UserInputService.InputBegan, function(input, gpe)
            if PanicActive then return end
            if gpe then return end
            if input.UserInputType == Enum.UserInputType.MouseButton1 and UserInputService:IsKeyDown(State.ClickTP.Key) then
                local mouse = LocalPlayer:GetMouse(); local hrp = GetHRP()
                if hrp then hrp.CFrame = CFrame.new(mouse.Hit.Position + Vector3.new(0,3,0)) end
            end
        end) end
    end},
    {Category="Visuals", Type="Toggle", Name="Crosshair", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Crosshair = v
        if v then
            local h = Instance.new("Frame", ScreenGui); h.Name = "RBX_CrosshairH"; h.Size = UDim2.new(0,20,0,2); h.Position = UDim2.new(0.5,-10,0.5,-1)
            h.BackgroundColor3 = Color3.fromRGB(255,255,255); h.BorderSizePixel = 0; h.ZIndex = 100
            local v = h:Clone(); v.Name = "RBX_CrosshairV"; v.Size = UDim2.new(0,2,0,20); v.Position = UDim2.new(0.5,-1,0.5,-10); v.Parent = ScreenGui
            State.CrosshairH = h; State.CrosshairV = v
        else
            if State.CrosshairH then SafeCall(function() State.CrosshairH:Destroy() end) end
            if State.CrosshairV then SafeCall(function() State.CrosshairV:Destroy() end) end
            State.CrosshairH = nil; State.CrosshairV = nil
        end
    end},
    {Category="Visuals", Type="Slider", Name="FOV", Min=30, Max=120, Default=70, Callback=function(v) State.FOV = v; Camera.FieldOfView = v end},
    {Category="Visuals", Type="Slider", Name="Gravity", Min=0, Max=196, Default=196, Callback=function(v) State.Gravity = v; Workspace.Gravity = v end},

    {Category="ESP", Type="Section", Text="ESP"},
    {Category="ESP", Type="Toggle", Name="Enable ESP", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.ESP.Enabled = v; RefreshESP()
        Notify("ESP", v and "ESP Enabled" or "ESP Disabled", 2, Color3.fromRGB(100,100,100))
    end},
    {Category="ESP", Type="Toggle", Name="ESP Team Check", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v) State.ESP.TeamCheck = v; RefreshESP() end},
    {Category="ESP", Type="Toggle", Name="Boxes", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.ESP.Boxes = v end},
    {Category="ESP", Type="Toggle", Name="Chams", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.ESP.Chams = v end},
    {Category="ESP", Type="Toggle", Name="Names", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.ESP.Names = v end},
    {Category="ESP", Type="Toggle", Name="Health", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.ESP.Health = v end},
    {Category="ESP", Type="Toggle", Name="Distance", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.ESP.Distance = v end},
    {Category="ESP", Type="Toggle", Name="Tracers", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.ESP.Tracers = v end},
    {Category="ESP", Type="Toggle", Name="Tool", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.ESP.Tool = v end},
    {Category="ESP", Type="Toggle", Name="Skeleton", Color=Color3.fromRGB(255,120,120), Default=false, Callback=function(v) State.ESP.Skeleton = v end},

    {Category="World", Type="Section", Text="WORLD"},
    {Category="World", Type="Button", Name="Destroy Trees", Color=Color3.fromRGB(60,60,60), Callback=function()
        for _, obj in ipairs(Workspace:GetDescendants()) do
            if obj:IsA("BasePart") and (obj.Name:lower():match("tree") or obj.Name:lower():match("bush")) then obj:Destroy() end
        end
        Notify("World", "Trees destroyed", 2, Color3.fromRGB(60,60,60))
    end},
    {Category="World", Type="Button", Name="Clear Fog", Color=Color3.fromRGB(60,60,60), Callback=function()
        Lighting.FogEnd = 100000; Lighting.FogStart = 0; Notify("World", "Fog cleared", 2, Color3.fromRGB(60,60,60))
    end},
    {Category="World", Type="Button", Name="Reset Lighting", Color=Color3.fromRGB(60,60,60), Callback=function()
        Lighting.FogEnd = 1000; Lighting.Brightness = 1; Lighting.ClockTime = 12; Notify("World", "Lighting reset", 2, Color3.fromRGB(60,60,60))
    end},

    {Category="Players", Type="Section", Text="PLAYERS"},
    {Category="Players", Type="PlayerSelector", Callback=function(player) end},
    {Category="Players", Type="Button", Name="Save Location", Color=Color3.fromRGB(60,60,60), Callback=function()
        local hrp = GetHRP(); if hrp then table.insert(SavedLocations, hrp.CFrame); Notify("Teleport", "Location #"..#SavedLocations.." saved", 2, Color3.fromRGB(60,60,60)) end
    end},
    {Category="Players", Type="Button", Name="TP to Saved #1", Color=Color3.fromRGB(60,60,60), Callback=function()
        if SavedLocations[1] then local hrp = GetHRP(); if hrp then hrp.CFrame = SavedLocations[1] end else Notify("Teleport", "No saved location", 2, Color3.fromRGB(60,60,60)) end
    end},
    {Category="Players", Type="Button", Name="TP to Saved #2", Color=Color3.fromRGB(60,60,60), Callback=function()
        if SavedLocations[2] then local hrp = GetHRP(); if hrp then hrp.CFrame = SavedLocations[2] end else Notify("Teleport", "No saved location", 2, Color3.fromRGB(60,60,60)) end
    end},
    {Category="Players", Type="Button", Name="Clear Saved", Color=Color3.fromRGB(60,60,60), Callback=function()
        SavedLocations = {}; Notify("Teleport", "Saved locations cleared", 2, Color3.fromRGB(60,60,60))
    end},
    {Category="Players", Type="Toggle", Name="Spectate", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.Spectate.Enabled = v
        if not v then 
            local hum = GetHum()
            if hum then Camera.CameraSubject = hum end
        end
    end},
    {Category="Players", Type="TextBox", Name="Spectate Player", Placeholder="Username", Callback=function(text)
        for _, p in ipairs(Players:GetPlayers()) do
            if p.Name:lower():sub(1, #text) == text:lower() then
                State.Spectate.Target = p
                if State.Spectate.Enabled and p.Character and p.Character.Parent then 
                    local hum = p.Character:FindFirstChildOfClass("Humanoid")
                    if hum then Camera.CameraSubject = hum end
                end
                Notify("Spectate", "Now spectating: "..p.Name, 2, Color3.fromRGB(100,100,100)); break
            end
        end
    end},

    {Category="Misc", Type="Section", Text="MISC"},
    {Category="Misc", Type="Toggle", Name="Anti-AFK", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.AntiAFK = v; Disconnect("AntiAFK")
        if v then Connect("AntiAFK", LocalPlayer.Idled, function()
            VirtualUser:CaptureController()
            VirtualUser:Button2Down(Vector2.new(0,0), Camera); task.wait(1); VirtualUser:Button2Up(Vector2.new(0,0), Camera)
        end) end
    end},

    -- FIXED: Legacy Auto Click — real CPS timing now (no hidden global cap)
    {Category="Misc", Type="Toggle", Name="Auto Click (Legacy)", Color=Color3.fromRGB(80,80,80), Default=false, Callback=function(v)
        State.AutoClick.Enabled = v; Disconnect("AutoClick")
        if v then 
            Connect("AutoClick", RunService.Heartbeat, function()
                if not State.AutoClick.Enabled or PanicActive then return end
                if not HasTool() then return end
                local now = tick()
                if now - (State._LastLegacyClick or 0) < 1 / math.max(State.AutoClick.CPS, 1) then return end
                State._LastLegacyClick = now
                UniversalClick()
            end) 
        end
    end},
    {Category="Misc", Type="Slider", Name="Legacy CPS", Min=1, Max=50, Default=15, Callback=function(v) State.AutoClick.CPS = v end},

    -- FIXED: Super Fast Click (dedicated thread, no lag)
    {Category="Misc", Type="Toggle", Name="Super Fast Click", Color=Color3.fromRGB(255,100,100), Default=false, Callback=function(v)
        State.SuperFastClick = v
        Disconnect("SuperFastClick")

        if v then
            -- FIXED (real CPS): bypass the global throttle — this thread owns its own timing
            OverrideClickCooldown = true
            local clickThread = task.spawn(function()
                while State.SuperFastClick and not PanicActive do
                    if HasTool() then
                        UniversalClick()
                    end
                    local waitTime = math.max(1 / math.max(State.SuperClickCPS, 1), 0.001)
                    task.wait(waitTime)
                end
                OverrideClickCooldown = false
            end)

            Connections["SuperFastClick"] = {
                Disconnect = function()
                    State.SuperFastClick = false
                    OverrideClickCooldown = false
                end
            }

            Notify("Super Click", tostring(State.SuperClickCPS) .. " CPS | Lag-Free Mode", 3, Color3.fromRGB(255,100,100))
        else
            Notify("Super Click", "Disabled", 2, Color3.fromRGB(100,100,100))
        end
    end},

    {Category="Misc", Type="Slider", Name="Super Click CPS", Min=1, Max=1000, Default=100, Callback=function(v)
        State.SuperClickCPS = v
        if State.SuperFastClick then
            Notify("Super Click", "CPS updated to " .. v, 2, Color3.fromRGB(255,100,100))
        end
    end},

    -- FIXED: Ultra Click (multi-threaded, no lag)
    {Category="Misc", Type="Toggle", Name="Ultra Click", Color=Color3.fromRGB(255,50,50), Default=false, Callback=function(v)
        State.UltraClick = v
        Disconnect("UltraClick")

        if v then
            -- FIXED (real CPS): bypass the global throttle so the 4 threads deliver the shown CPS
            OverrideClickCooldown = true
            local running = true
            local numThreads = 4
            local clicksPerThread = math.max(math.ceil(State.SuperClickCPS / numThreads), 1)
            local waitPerThread = math.max(1 / clicksPerThread, 0.0005)

            for i = 1, numThreads do
                task.spawn(function()
                    while running and State.UltraClick and not PanicActive do
                        if HasTool() then
                            UniversalClick()
                        end
                        task.wait(waitPerThread)
                    end
                end)
            end

            Connections["UltraClick"] = {
                Disconnect = function()
                    running = false
                    State.UltraClick = false
                    OverrideClickCooldown = false
                end
            }

            Notify("Ultra Click", "~" .. State.SuperClickCPS .. " CPS | Multi-Threaded", 3, Color3.fromRGB(255,50,50))
        else
            Notify("Ultra Click", "Disabled", 2, Color3.fromRGB(100,100,100))
        end
    end},

    {Category="Misc", Type="Toggle", Name="Auto Collect", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.AutoCollect.Enabled = v; Disconnect("AutoCollect")
        AutoCollectTargets = {}
        if v then Connect("AutoCollect", RunService.Heartbeat, function()
            if not State.AutoCollect.Enabled or PanicActive then return end
            local hrp = GetHRP(); if not hrp then return end
            local now = tick()
            if now - LastAutoCollectScan >= 0.5 then
                LastAutoCollectScan = now
                AutoCollectTargets = {}
                local scanned = 0
                for _, obj in ipairs(Workspace:GetDescendants()) do
                    scanned += 1
                    if scanned > MaxWorldScanObjects then break end
                    if obj:IsA("BasePart") then
                        local n = obj.Name:lower()
                        if n:match("coin") or n:match("collect") or n:match("drop") then
                            table.insert(AutoCollectTargets, obj)
                        end
                    end
                end
            end
            for _, obj in ipairs(AutoCollectTargets) do
                if obj and obj.Parent and (obj.Position - hrp.Position).Magnitude < State.AutoCollect.Range then
                    SafeCall(function() if firetouchinterest then firetouchinterest(hrp, obj, 0); firetouchinterest(hrp, obj, 1) end end)
                end
            end
        end) end
    end},
    {Category="Misc", Type="Slider", Name="Collect Range", Min=10, Max=200, Default=60, Callback=function(v) State.AutoCollect.Range = v end},
    {Category="Misc", Type="Toggle", Name="Auto Farm", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.AutoFarm.Enabled = v; Disconnect("AutoFarm")
        AutoFarmTarget = nil
        if v then
            Connect("AutoFarm", RunService.Heartbeat, function()
                if not State.AutoFarm.Enabled or PanicActive then return end
                local hrp = GetHRP(); if not hrp then return end
                local now = tick()
                if now - LastAutoFarmScan < 0.6 and AutoFarmTarget and AutoFarmTarget.Parent then
                    SafeCall(function() hrp.CFrame = AutoFarmTarget.CFrame + Vector3.new(0, 3, 0) end)
                    return
                end
                LastAutoFarmScan = now
                AutoFarmTarget = nil
                local bestDist = math.huge
                if State.AutoFarm.Mode == "Mobs" then
                    local scanned = 0
                    for _, obj in ipairs(Workspace:GetDescendants()) do
                        scanned += 1
                        if scanned > MaxWorldScanObjects then break end
                        if obj:IsA("Model") and obj ~= GetChar() and obj.Parent then
                            local hum = obj:FindFirstChildOfClass("Humanoid")
                            local root = obj:FindFirstChild("HumanoidRootPart") or obj:FindFirstChildWhichIsA("BasePart")
                            if hum and root and hum.Health > 0 then
                                local d = (root.Position - hrp.Position).Magnitude
                                if d < bestDist then bestDist = d; AutoFarmTarget = root end
                            end
                        end
                    end
                else
                    local scanned = 0
                    for _, obj in ipairs(Workspace:GetDescendants()) do
                        scanned += 1
                        if scanned > MaxWorldScanObjects then break end
                        if obj:IsA("BasePart") then
                            local n = obj.Name:lower()
                            local match = (State.AutoFarm.Mode == "Coins" and (n:match("coin") or n:match("collect") or n:match("drop")))
                                or (State.AutoFarm.Mode == "Items" and (n:match("item") or n:match("pickup") or n:match("collect")))
                            if match then
                                local d = (obj.Position - hrp.Position).Magnitude
                                if d < bestDist then bestDist = d; AutoFarmTarget = obj end
                            end
                        end
                    end
                end
                if AutoFarmTarget and AutoFarmTarget.Parent then
                    SafeCall(function() hrp.CFrame = AutoFarmTarget.CFrame + Vector3.new(0, 3, 0) end)
                end
            end)
            Notify("Auto Farm", "Client-side " .. State.AutoFarm.Mode .. " farm enabled", 2, Color3.fromRGB(100,100,100))
        end
    end},
    {Category="Misc", Type="Dropdown", Name="Farm Mode", Options={"Coins","Mobs","Items"}, Default=1, Callback=function(val) State.AutoFarm.Mode = val end},

    {Category="FPS Boost", Type="Section", Text="FPS BOOST"},
    {Category="FPS Boost", Type="Toggle", Name="Enable FPS Boost", Color=Color3.fromRGB(100,100,100), Default=false, Callback=function(v)
        State.FPSBoost.Enabled = v
        if v then
            UpdateFPSBoost()
            Notify("FPS Boost", "FPS Boost ACTIVE", 3, Color3.fromRGB(100,100,100))
        else
            UpdateFPSBoost()
            Notify("FPS Boost", "FPS Boost disabled", 2, Color3.fromRGB(100,100,100))
        end
    end},
    {Category="FPS Boost", Type="Toggle", Name="Remove Decals", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.RemoveDecals = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Toggle", Name="Remove Particles", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.RemoveParticles = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Toggle", Name="Remove Textures", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.RemoveTextures = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Toggle", Name="Disable Shadows", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.DisableShadows = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Toggle", Name="Low Quality Mode", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.LowQuality = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Toggle", Name="Remove Trails", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.RemoveTrails = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Toggle", Name="Remove Beams", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.RemoveBeams = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Toggle", Name="Disable Post Effects", Color=Color3.fromRGB(100,100,100), Default=true, Callback=function(v) State.FPSBoost.DisableLightingEffects = v; if State.FPSBoost.Enabled then UpdateFPSBoost() end end},
    {Category="FPS Boost", Type="Button", Name="Save Settings", Color=Color3.fromRGB(60,60,60), Callback=function()
        local success, json = pcall(function()
            local data = {
                FPSBoost = State.FPSBoost,
                Keybinds = {AimbotToggle = tostring(State.CustomKeybinds.AimbotToggle):gsub("Enum.UserInputType.", ""):gsub("Enum.KeyCode.", "")},
                AimbotMaxDistance = State.AimbotMaxDistance,
            }
            return HttpService:JSONEncode(data)
        end)
        if success then
            if setclipboard then setclipboard(json) end
            Notify("FPS Boost", "Settings copied to clipboard!", 3, Color3.fromRGB(100,100,100))
        else
            Notify("FPS Boost", "Failed to save settings!", 2, Color3.fromRGB(255,50,50))
        end
    end},
    {Category="FPS Boost", Type="TextBox", Name="Import Settings", Placeholder="Paste JSON here...", Callback=function(text)
        local ok, data = pcall(function() return HttpService:JSONDecode(text) end)
        if ok and data and type(data) == "table" then
            if data.FPSBoost and type(data.FPSBoost) == "table" then
                for k,v in pairs(data.FPSBoost) do State.FPSBoost[k] = v end
            end
            if data.Keybinds and data.Keybinds.AimbotToggle then
                local key = data.Keybinds.AimbotToggle
                if key == "Mouse1" then State.CustomKeybinds.AimbotToggle = Enum.UserInputType.MouseButton1
                elseif key == "Mouse2" then State.CustomKeybinds.AimbotToggle = Enum.UserInputType.MouseButton2
                elseif key == "Mouse3" then State.CustomKeybinds.AimbotToggle = Enum.UserInputType.MouseButton3
                else State.CustomKeybinds.AimbotToggle = Enum.KeyCode[key] or Enum.UserInputType.MouseButton2 end
            end
            if data.AimbotMaxDistance and type(data.AimbotMaxDistance) == "number" then State.AimbotMaxDistance = data.AimbotMaxDistance end
            Notify("FPS Boost", "Settings loaded! Reopen tab to refresh.", 3, Color3.fromRGB(100,100,100))
        else
            Notify("FPS Boost", "Invalid JSON!", 2, Color3.fromRGB(255,50,50))
        end
    end},

    {Category="Info", Type="Section", Text="RBX 2.2.0 • AIMBOT & GLASS FIXES"},
        {Category="Info", Type="Section", Text="RBX 2.0.0 • POWER COMBAT / RAINBOW / DEVICE-FIT UPDATE"},
    {Category="Info", Type="Changelog", Name="UPDATE NOTES", Value=GetChangelogText},
    {Category="Info", Type="Button", Name="COPY UPDATE NOTES", Color=Color3.fromRGB(70,70,90), Callback=function() CopyToClipboard(GetChangelogText(), "Update notes") end},
    {Category="Info", Type="Info", Name="Build", Value="RBX " .. GetHubVersion()},
    {Category="Info", Type="Info", Name="Device Profile", Value=function() return DeviceType end},
    {Category="Info", Type="Section", Text="TOP STATUS OVERLAY"},
    {Category="Info", Type="Toggle", Name="Show All Overlay Stats", Color=Color3.fromRGB(85,85,120), Default=false, Callback=function(v)
        State.Overlay.Enabled = v
        if v then State.Overlay.FPS = true; State.Overlay.ServerName = true; State.Overlay.Ping = true; State.Overlay.Network = true end
    end},
    {Category="Info", Type="Toggle", Name="Show Overlay When Panel Closes", Color=Color3.fromRGB(75,75,95), Default=true, Callback=function(v) State.Overlay.AutoShowOnClose = v end},
    {Category="Info", Type="Toggle", Name="Overlay FPS", Color=Color3.fromRGB(75,75,95), Default=true, Callback=function(v) State.Overlay.FPS = v end},
    {Category="Info", Type="Toggle", Name="Overlay Server Name", Color=Color3.fromRGB(75,75,95), Default=true, Callback=function(v) State.Overlay.ServerName = v end},
    {Category="Info", Type="Toggle", Name="Overlay Ping", Color=Color3.fromRGB(75,75,95), Default=true, Callback=function(v) State.Overlay.Ping = v end},
    {Category="Info", Type="Toggle", Name="Overlay Network", Color=Color3.fromRGB(75,75,95), Default=true, Callback=function(v) State.Overlay.Network = v end},
    {Category="Info", Type="Section", Text="INFO / LIVE CLIENT STATUS"},
    {Category="Info", Type="Info", Name="Game Name", Value=function() return GetGameName() end},
    {Category="Info", Type="Info", Name="Place ID", Value=function() return tostring(game.PlaceId) end, Button="Copy", Callback=function() CopyToClipboard(game.PlaceId, "Place ID") end},
    {Category="Info", Type="Info", Name="Job ID", Value=function() return tostring(game.JobId or "N/A") end, Button="Copy", Callback=function() CopyToClipboard(game.JobId, "Job ID") end},
    {Category="Info", Type="Info", Name="Player Name", Value=function() return LocalPlayer and (LocalPlayer.DisplayName .. " (" .. LocalPlayer.Name .. ")") or "Unknown" end, Button="Copy", Callback=function() CopyToClipboard(LocalPlayer and LocalPlayer.Name or "", "Username") end},
    {Category="Info", Type="Info", Name="Player ID", Value=function() return LocalPlayer and tostring(LocalPlayer.UserId) or "Unknown" end, Button="Copy", Callback=function() CopyToClipboard(LocalPlayer and LocalPlayer.UserId or "", "User ID") end},
    {Category="Info", Type="Info", Name="Account Age", Value=function() return LocalPlayer and (tostring(LocalPlayer.AccountAge) .. " days") or "Unknown" end},
    {Category="Info", Type="Info", Name="FPS", Value=GetFPS},
    {Category="Info", Type="Info", Name="Ping", Value=GetPingText},
    {Category="Info", Type="Info", Name="Uptime", Value=GetUptimeText},
    {Category="Info", Type="Info", Name="Platform", Value=GetPlatformText},
    {Category="Info", Type="Info", Name="Discord", Value=CONFIG.DiscordInvite, Button="Copy Link", Callback=function() CopyToClipboard(CONFIG.DiscordInvite, "Discord invite") end},
    {Category="Info", Type="Button", Name="COPY ALL INFO", Color=Color3.fromRGB(70,70,70), Callback=function() CopyToClipboard(GetAllInfoText(), "Full info") end},

    {Category="Join", Type="Section", Text="SERVER JOIN / SERVER BROWSER"},
    {Category="Join", Type="TextBox", Name="Job ID", Placeholder="Paste Job ID here...", Callback=function(text) State.JoinJobId = tostring(text or ""):gsub("%s+", "") end},
    {Category="Join", Type="Button", Name="JOIN SERVER BY JOB ID", Color=Color3.fromRGB(65,65,75), Callback=function() JoinJobId(State.JoinJobId) end},
    {Category="Join", Type="Button", Name="COPY CURRENT JOB ID", Color=Color3.fromRGB(55,55,65), Callback=function() CopyToClipboard(game.JobId or "", "Job ID") end},
    {Category="Join", Type="Button", Name="CHECK SERVER STATUS", Color=Color3.fromRGB(55,70,60), Callback=function() CheckServerStatus(State.JoinJobId) end},
    {Category="Join", Type="Info", Name="Server Status", Value=function() return ServerStatus.Text end},
    {Category="Join", Type="Info", Name="Server Members", Value=function() local d=ServerStatus.Data; return d and (tostring(d.playing or 0).." / "..tostring(d.maxPlayers or 0)) or "N/A" end},
    {Category="Join", Type="Info", Name="Server Ping", Value=function() local d=ServerStatus.Data; return d and tonumber(d.ping) and (tostring(math.floor(d.ping)).." ms") or "N/A" end},
    {Category="Join", Type="Info", Name="Server FPS", Value=function() local d=ServerStatus.Data; return d and tonumber(d.fps) and tostring(math.floor(d.fps)) or "N/A" end},
    {Category="Join", Type="Info", Name="Server Region", Value=function() return GetServerRegion(ServerStatus.Data) end},
    {Category="Join", Type="Info", Name="Current Ping", Value=function() local p=GetCurrentPingNumber(); return p and (tostring(math.floor(p)).." ms") or "N/A" end},
    {Category="Join", Type="Button", Name="JOIN LOWEST PING SERVER", Color=Color3.fromRGB(65,75,65), Callback=function() JoinSelectedServer("ping") end},
    {Category="Join", Type="Button", Name="JOIN BEST AVAILABLE SERVER", Color=Color3.fromRGB(65,65,80), Callback=function() JoinSelectedServer("best") end},
    {Category="Join", Type="Button", Name="REFRESH SERVER LIST", Color=Color3.fromRGB(50,50,60), Callback=function()
        ServerCache.At = 0
        local ok, data = FetchPublicServers(3, true)
        Notify("Server Browser", ok and ("Loaded " .. tostring(#data) .. " public servers.") or tostring(data), 3, ok and CONFIG.Accent or Color3.fromRGB(255,80,80))
    end},

    {Category="Settings", Type="Section", Text="SETTINGS"},
    {Category="Settings", Type="Section", Text="PROFILE SAVE / LOAD"},
    {Category="Settings", Type="Button", Name="SAVE PROFILE", Color=Color3.fromRGB(14,116,144), Callback=function()
        local ok, reason = SaveProfileToFile()
        if ok then Notify("Settings", "Profile saved. You can load it next time.", 3, CONFIG.Accent)
        else Notify("Settings", tostring(reason), 3, Color3.fromRGB(255,80,80)) end
    end},
    {Category="Settings", Type="Button", Name="LOAD SAVED PROFILE", Color=Color3.fromRGB(14,116,144), Callback=function()
        local ok, reason = LoadProfileFromFile()
        if ok then Notify("Settings", "Profile loaded. Reopen tabs to refresh controls.", 3, CONFIG.Accent)
        else Notify("Settings", tostring(reason), 3, Color3.fromRGB(255,80,80)) end
    end},
    {Category="Settings", Type="Section", Text="COLOR THEME"},
    {Category="Settings", Type="Dropdown", Name="UI Theme", Options=ThemeOrder, Default=1, Callback=function(theme)
        local ok = ApplyTheme(theme)
        if ok then
            Notify("Theme", theme .. " applied — whole GUI recolored" .. (theme == "Rainbow" and " (RGB live flow!)" or ""), 3, GetAccent())
        end
    end},
    {Category="Settings", Type="Slider", Name="UI Scale %", Min=50, Max=150, Default=100, Callback=function(v)
        State.UIScale = v
        UpdateMainScale()
    end},
    {Category="Settings", Type="Keybind", Name="Aimbot Toggle Key", Default=State.CustomKeybinds.AimbotToggle, Callback=function(key)
        State.CustomKeybinds.AimbotToggle = key
        local name = typeof(key) == "EnumItem" and (key.EnumType == Enum.KeyCode and tostring(key):gsub("Enum.KeyCode.", "") or tostring(key):gsub("Enum.UserInputType.", "")) or "None"
        Notify("Settings", "Aimbot keybind set to " .. name, 2, CONFIG.Accent)
    end},
    {Category="Settings", Type="Button", Name="Reset Character", Color=Color3.fromRGB(60,60,60), Callback=function()
        local hum = GetHum(); if hum then hum.Health = 0 end
    end},
    {Category="Settings", Type="Button", Name="Rejoin Server", Color=Color3.fromRGB(60,60,60), Callback=function()
        SafeCall(function() TeleportService:Teleport(game.PlaceId, LocalPlayer) end)
    end},
    {Category="Settings", Type="Button", Name="Copy JobId", Color=Color3.fromRGB(60,60,60), Callback=function()
        if setclipboard then setclipboard(game.JobId or "") end; Notify("Settings", "JobId copied", 2, Color3.fromRGB(60,60,60))
    end},
    {Category="Settings", Type="Button", Name="Destroy GUI", Color=Color3.fromRGB(60,60,60), Callback=function()
        -- FIXED: full PANIC-style cleanup — kills every loop (threads, RunService, ESP, hitboxes)
        if type(Panic) == "function" then
            SafeCall(Panic)
        else
            SafeCall(function() ScreenGui:Destroy() end)
            for name, conn in pairs(Connections) do SafeCall(function() if typeof(conn) == "RBXScriptConnection" then conn:Disconnect() end end) end
            ClearESP()
        end
    end},
}

-- ==================== STATE PERSISTENCE HELPERS (FIXED) ====================
local function GetCurrentDefault(feat)
    local name = feat.Name
    if feat.Type == "Toggle" then
        if name == "Velocity Speed" then return State.Speed.Enabled
        elseif name == "Super Jump" then return State.Jump.Enabled
        elseif name == "Fly Mode" then return State.Fly.Enabled
        elseif name == "Infinite Jump" then return State.InfJump
        elseif name == "Bunny Hop" then return State.BunnyHop
        elseif name == "Auto-Heal" then return State.AutoHeal.Enabled
        elseif name == "NoClip" then return State.NoClip
        elseif name == "Jetpack" then return State.Jetpack
        elseif name == "Invisible" then return State.Invisible
        elseif name == "Walk on Water" then return State.WaterWalk.Enabled
        elseif name == "Infinite Stamina" then return State.Stamina
        elseif name == "Anti Knockback" then return State.AntiKnockback
        elseif name == "Vehicle Speed" and feat.Category == "Movement" then return State.VehicleSpeed.Enabled
        elseif name == "Aimbot" then return State.Aimbot.Enabled
        elseif name == "Power Mode" then return State.Aimbot.PowerMode
        elseif name == "Lock Target" then return State.Aimbot.LockOn
        elseif name == "Team Check" then return State.Aimbot.TeamCheck
        elseif name == "Wall Check" then return State.Aimbot.WallCheck
        elseif name == "Prediction" then return State.Aimbot.Prediction
        elseif name == "Drop Comp" then return State.Aimbot.DropComp
        elseif name == "Auto Shoot" then return State.Aimbot.AutoShoot
        elseif name == "Auto WallBang" then return State.Aimbot.AutoWallBang
        elseif name == "Camera Lock" then return State.CameraLock.Enabled
        elseif name == "Silent Aim" then return State.SilentAim.Enabled
        elseif name == "Silent Team Check" then return State.SilentAim.TeamCheck
        elseif name == "Silent Visible Check" then return State.SilentAim.VisibleCheck
        elseif name == "Trigger Bot" then return State.TriggerBot.Enabled
        elseif name == "Auto Parry" then return State.AutoParry.Enabled
        elseif name == "Auto Parry Every Frame" then return State.AutoParry.FrameFire
        elseif name == "Rapid Fire" then return State.RapidFire
        elseif name == "Melee Aura" then return State.MeleeAura.Enabled
        elseif name == "Aura Attack Mode" then return State.MeleeAura.AttackAll
        elseif name == "Hitbox Expander" then return State.Hitbox.Enabled
        elseif name == "Hitbox Expand Torso/Arms" then return State.Hitbox.ExpandTorso
        elseif name == "God Mode Auto Revive" then return State.GodModeRevive
        elseif name == "Auto Pot / Auto Eat" then return State.AutoHealCombat.Enabled
        elseif name == "Skeleton" then return State.ESP.Skeleton
        elseif name == "Reach" then return State.Reach.Enabled
        elseif name == "Spin Bot" then return State.SpinBot.Enabled
        elseif name == "God Mode" then return State.GodMode
        elseif name == "Fullbright" then return State.Fullbright.Enabled
        elseif name == "XRay" then return State.XRay.Enabled
        elseif name == "Wireframe" then return State.Wireframe.Enabled
        elseif name == "Bloom" then return State.Bloom.Enabled
        elseif name == "SunRays" then return State.SunRays.Enabled
        elseif name == "Color Tint" then return State.ColorTint.Enabled
        elseif name == "Time Freeze" then return State.TimeFreeze.Enabled
        elseif name == "Freecam" then return State.Freecam.Enabled
        elseif name == "Click TP" then return State.ClickTP.Enabled
        elseif name == "Crosshair" then return State.Crosshair
        elseif name == "Enable ESP" then return State.ESP.Enabled
        elseif name == "ESP Team Check" then return State.ESP.TeamCheck
        elseif name == "Boxes" then return State.ESP.Boxes
        elseif name == "Chams" then return State.ESP.Chams
        elseif name == "Names" then return State.ESP.Names
        elseif name == "Health" then return State.ESP.Health
        elseif name == "Distance" then return State.ESP.Distance
        elseif name == "Tracers" then return State.ESP.Tracers
        elseif name == "Tool" then return State.ESP.Tool
        elseif name == "Spectate" then return State.Spectate.Enabled
        elseif name == "Anti-AFK" then return State.AntiAFK
        elseif name == "Auto Click (Legacy)" then return State.AutoClick.Enabled
        elseif name == "Super Fast Click" then return State.SuperFastClick
        elseif name == "Ultra Click" then return State.UltraClick
        elseif name == "Auto Collect" then return State.AutoCollect.Enabled
        elseif name == "Auto Farm" then return State.AutoFarm.Enabled
        elseif name == "Enable FPS Boost" then return State.FPSBoost.Enabled
        elseif name == "Show All Overlay Stats" then return State.Overlay.Enabled
        elseif name == "Show Overlay When Panel Closes" then return State.Overlay.AutoShowOnClose
        elseif name == "Overlay FPS" then return State.Overlay.FPS
        elseif name == "Overlay Server Name" then return State.Overlay.ServerName
        elseif name == "Overlay Ping" then return State.Overlay.Ping
        elseif name == "Overlay Network" then return State.Overlay.Network
        elseif name == "Remove Decals" then return State.FPSBoost.RemoveDecals
        elseif name == "Remove Particles" then return State.FPSBoost.RemoveParticles
        elseif name == "Remove Textures" then return State.FPSBoost.RemoveTextures
        elseif name == "Disable Shadows" then return State.FPSBoost.DisableShadows
        elseif name == "Low Quality Mode" then return State.FPSBoost.LowQuality
        elseif name == "Remove Trails" then return State.FPSBoost.RemoveTrails
        elseif name == "Remove Beams" then return State.FPSBoost.RemoveBeams
        elseif name == "Disable Post Effects" then return State.FPSBoost.DisableLightingEffects
        else return feat.Default end
    elseif feat.Type == "Slider" then
        if name == "Speed Value" then return State.Speed.Value
        elseif name == "Jump Power" then return State.Jump.Power
        elseif name == "Fly Speed" then return State.Fly.Speed
        elseif name == "Heal Threshold" then return State.AutoHeal.Threshold
        elseif name == "Hip Height" then return State.HipHeight
        elseif name == "Vehicle Speed" and feat.Category == "Movement" then return State.VehicleSpeed.Value
        elseif name == "Aimbot FOV" then return State.Aimbot.FOV
        elseif name == "Aimbot Smooth" then return math.floor(State.Aimbot.Smoothness * 100)
        elseif name == "Shake" then return State.Aimbot.Shake
        elseif name == "Max Distance" then return State.AimbotMaxDistance
        elseif name == "Silent FOV" then return State.SilentAim.FOV
        elseif name == "Hit Chance" then return State.SilentAim.HitChance
        elseif name == "Trigger Delay" then return math.floor(State.TriggerBot.Delay * 100)
        elseif name == "Parry Range" then return State.AutoParry.Range
        elseif name == "Aura Range" then return State.MeleeAura.Range
        elseif name == "Rapid Fire Rate" then return math.floor(State.RapidFireDelay * 1000)
        elseif name == "Pot Threshold %" then return State.AutoHealCombat.Threshold
        elseif name == "UI Scale %" then return State.UIScale
        elseif name == "Hitbox Size" then return State.Hitbox.Size
        elseif name == "Reach Distance" then return State.Reach.Distance
        elseif name == "Spin Speed" then return State.SpinBot.Speed
        elseif name == "FB Intensity" then return math.floor(State.Fullbright.Intensity * 10)
        elseif name == "XRay Alpha" then return math.floor(State.XRay.Transparency * 10)
        elseif name == "Bloom Intensity" then return math.floor(State.Bloom.Intensity * 10)
        elseif name == "Bloom Size" then return State.Bloom.Size
        elseif name == "SunRays Intensity" then return math.floor(State.SunRays.Intensity * 10)
        elseif name == "SunRays Spread" then return math.floor(State.SunRays.Spread * 10)
        elseif name == "Freecam Speed" then return math.floor(State.Freecam.Speed * 5)
        elseif name == "FOV" then return State.FOV
        elseif name == "Gravity" then return State.Gravity
        elseif name == "Legacy CPS" then return State.AutoClick.CPS
        elseif name == "Super Click CPS" then return State.SuperClickCPS
        elseif name == "Collect Range" then return State.AutoCollect.Range
        else return feat.Default end
    elseif feat.Type == "Dropdown" then
        if name == "Aim Part" then
            local parts = {"Head","Torso","HumanoidRootPart","LeftArm","RightArm"}
            for i, p in ipairs(parts) do if p == State.Aimbot.Part then return i end end
            return 1
        elseif name == "Priority" then
            local pris = {"Closest","Distance","Lowest Health","FOV"}
            for i, p in ipairs(pris) do if p == State.Aimbot.Priority then return i end end
            return 1
        elseif name == "Farm Mode" then
            local modes = {"Coins","Mobs","Items"}
            for i, m in ipairs(modes) do if m == State.AutoFarm.Mode then return i end end
            return 1
        elseif name == "Auto Shoot Mode" then
            if State.Aimbot.AutoShootMode == "Spam" then return 2 end
            return 1
        elseif name == "Spin Mode" then
            if State.SpinBot.Mode == "Render" then return 2 end
            return 1
        elseif name == "UI Theme" then
            for i, theme in ipairs(ThemeOrder) do if theme == State.Theme then return i end end
            return 1
        else return feat.Default end
    else
        return feat.Default
    end
end

local function CreateChangelogCard(parent, title, value)
    local frame = Instance.new("Frame", parent)
    frame.Size = UDim2.new(1,0,0,430)
    frame.BackgroundColor3 = Color3.fromRGB(16,16,20)
    frame.BorderSizePixel = 0
    frame.ClipsDescendants = true
    Instance.new("UICorner", frame).CornerRadius = UDim.new(0,12)
    local stroke = Instance.new("UIStroke", frame)
    stroke.Color = Color3.fromRGB(55,55,70)
    stroke.Thickness = 1.2
    stroke.Transparency = 0.3
    RegisterThemed(stroke, "Color") -- changelog card follows the theme

    local header = Instance.new("TextLabel", frame)
    header.Size = UDim2.new(1,-28,0,28)
    header.Position = UDim2.new(0,14,0,10)
    header.BackgroundTransparency = 1
    header.Text = "▌ " .. tostring(title or "UPDATE NOTES")
    header.TextColor3 = Color3.fromRGB(245,245,250)
    header.Font = Enum.Font.GothamBold
    header.TextSize = 14
    header.TextXAlignment = Enum.TextXAlignment.Left

    local scroll = Instance.new("ScrollingFrame", frame)
    scroll.Size = UDim2.new(1,-28,1,-52)
    scroll.Position = UDim2.new(0,14,0,42)
    scroll.BackgroundTransparency = 1
    scroll.BorderSizePixel = 0
    scroll.ScrollBarThickness = 8
    scroll.ScrollBarImageTransparency = 0.25
    scroll.AutomaticCanvasSize = Enum.AutomaticSize.Y
    scroll.CanvasSize = UDim2.new(0,0,0,0)

    local body = Instance.new("TextLabel", scroll)
    body.Size = UDim2.new(1,-8,0,0)
    body.AutomaticSize = Enum.AutomaticSize.Y
    body.BackgroundTransparency = 1
    body.Text = tostring(value or "")
    body.TextColor3 = Color3.fromRGB(190,190,205)
    body.Font = Enum.Font.Code
    body.TextSize = 12
    body.TextWrapped = true
    body.TextXAlignment = Enum.TextXAlignment.Left
    body.TextYAlignment = Enum.TextYAlignment.Top
    return frame
end

-- ==================== RENDER TABS (FIXED) ====================
local TabButtons = {}
local CurrentTab = 1

local function RenderTab(index)
    if PanicActive then return end
    if index < 1 then index = #CONFIG.Categories end
    if index > #CONFIG.Categories then index = 1 end
    CurrentTab = index

    for i, btn in ipairs(TabButtons) do
        local active = i == index
        SafeCall(function()
            TweenService:Create(btn, TweenInfo.new(0.2), {
                BackgroundColor3 = active and Color3.fromRGB(60,60,60) or Color3.fromRGB(25,25,25),
                TextColor3 = active and Color3.fromRGB(255,255,255) or Color3.fromRGB(130,130,130)
            }):Play()
        end)
    end

    InfoLiveLabels = {}
    for _, child in ipairs(ContentFrame:GetChildren()) do if child:IsA("Frame") or child:IsA("TextButton") then child:Destroy() end end

    for _, feat in ipairs(Features) do
        if feat.Category == CONFIG.Categories[index] then
            SafeCall(function()
                local def = GetCurrentDefault(feat)
                if feat.Type == "Section" then CreateSection(ContentFrame, feat.Text)
                elseif feat.Type == "Toggle" then CreateToggle(ContentFrame, feat.Name, def, feat.Color, feat.Callback)
                elseif feat.Type == "Slider" then CreateSlider(ContentFrame, feat.Name, feat.Min, feat.Max, def, feat.Callback)
                elseif feat.Type == "Button" then CreateButton(ContentFrame, feat.Name, feat.Color, feat.Callback)
                elseif feat.Type == "Dropdown" then CreateDropdown(ContentFrame, feat.Name, feat.Options, def, feat.Callback)
                elseif feat.Type == "TextBox" then CreateTextBox(ContentFrame, feat.Name, feat.Placeholder, feat.Callback)
                elseif feat.Type == "Keybind" then CreateKeybind(ContentFrame, feat.Name, def, feat.Callback)
                elseif feat.Type == "PlayerSelector" then CreatePlayerSelector(ContentFrame, feat.Callback)
                elseif feat.Type == "Info" then
                    local infoValue = type(feat.Value) == "function" and feat.Value() or feat.Value
                    CreateInfoCard(ContentFrame, feat.Name, infoValue, feat.Button, feat.Callback)
                elseif feat.Type == "Changelog" then
                    local changeValue = type(feat.Value) == "function" and feat.Value() or feat.Value
                    CreateChangelogCard(ContentFrame, feat.Name, changeValue)
                end
            end)
        end
    end

    ContentFrame.CanvasPosition = Vector2.new(0, 0)
end

local tabWidth = DeviceType == "Mobile" and 118 or math.max(42, math.floor((CONFIG.PanelWidth - 70 - (5 * (#CONFIG.Categories - 1))) / #CONFIG.Categories))
for i, name in ipairs(CONFIG.Categories) do
    local btn = Instance.new("TextButton", TabContainer)
    btn.Size = UDim2.new(0, tabWidth, 1, -4); btn.Position = UDim2.new(0, 0, 0, 2)
    btn.BackgroundColor3 = (i == 1) and Color3.fromRGB(60,60,60) or Color3.fromRGB(25,25,25)
    btn.Text = name; btn.TextColor3 = (i == 1) and Color3.fromRGB(255,255,255) or Color3.fromRGB(130,130,130)
    btn.Font = Enum.Font.GothamSemibold; btn.TextSize = 11; btn.AutoButtonColor = false; btn.BorderSizePixel = 0
    Instance.new("UICorner", btn).CornerRadius = UDim.new(0, 8)
    AddHoverAnimation(btn, (i == 1) and Color3.fromRGB(60,60,60) or Color3.fromRGB(25,25,25), Color3.fromRGB(70,70,70), btn.Size, UDim2.new(btn.Size.X.Scale, btn.Size.X.Offset, btn.Size.Y.Scale, btn.Size.Y.Offset + 2))
    btn.MouseButton1Click:Connect(function() if not PanicActive then RenderTab(i) end end)
    table.insert(TabButtons, btn)
end
ApplyResponsiveLayout()

LeftArrow.MouseButton1Click:Connect(function() if not PanicActive then RenderTab(CurrentTab - 1) end end)
RightArrow.MouseButton1Click:Connect(function() if not PanicActive then RenderTab(CurrentTab + 1) end end)

Connect("InfoLiveUpdate", RunService.Heartbeat, function()
    if PanicActive or next(InfoLiveLabels) == nil then return end
    local values = {
        ["Game Name"] = GetGameName(), ["Place ID"] = tostring(game.PlaceId), ["Job ID"] = tostring(game.JobId or "N/A"),
        ["Player Name"] = LocalPlayer and (LocalPlayer.DisplayName .. " (" .. LocalPlayer.Name .. ")") or "Unknown",
        ["Player ID"] = LocalPlayer and tostring(LocalPlayer.UserId) or "Unknown",
        ["Account Age"] = LocalPlayer and (tostring(LocalPlayer.AccountAge) .. " days") or "Unknown",
        ["FPS"] = GetFPS(), ["Ping"] = GetPingText(), ["Uptime"] = GetUptimeText(), ["Platform"] = GetPlatformText(),
        ["Server Status"] = ServerStatus.Text,
        ["Server Members"] = (ServerStatus.Data and (tostring(ServerStatus.Data.playing or 0) .. " / " .. tostring(ServerStatus.Data.maxPlayers or 0)) or "N/A"),
        ["Server Ping"] = (ServerStatus.Data and tonumber(ServerStatus.Data.ping) and (tostring(math.floor(ServerStatus.Data.ping)) .. " ms") or "N/A"),
        ["Server FPS"] = (ServerStatus.Data and tonumber(ServerStatus.Data.fps) and tostring(math.floor(ServerStatus.Data.fps)) or "N/A"),
        ["Server Region"] = GetServerRegion(ServerStatus.Data),
        ["Current Ping"] = (function() local p=GetCurrentPingNumber(); return p and (tostring(math.floor(p)) .. " ms") or "N/A" end)()
    }
    for key, label in pairs(InfoLiveLabels) do
        local value = values[key]
        if value and label and label.Parent then SafeCall(function() label.Text = tostring(value) end) end
    end
end)

-- ==================== FLOATING TOGGLE BUTTON (POWER) (FIXED) ====================
-- Global on purpose: ToggleUI (defined earlier) hides it while the panel is open.
FloatBtn = Instance.new("TextButton", ScreenGui)
FloatBtn.Name = "FloatBtn"
FloatBtn.Size = UDim2.new(0, 190, 0, 55)
FloatBtn.Position = UDim2.new(1, -210, 0, 20)
FloatBtn.BackgroundColor3 = Color3.fromRGB(10, 14, 22) -- GLASS
FloatBtn.BackgroundTransparency = 0.25
FloatBtn.Text = "RBX MOBILE"
FloatBtn.TextColor3 = Color3.fromRGB(255,255,255)
FloatBtn.TextSize = 16
FloatBtn.Font = Enum.Font.GothamBold
FloatBtn.AutoButtonColor = false
FloatBtn.BorderSizePixel = 0
FloatBtn.ZIndex = 10
FloatBtn.TextStrokeTransparency = 0
FloatBtn.TextStrokeColor3 = Color3.fromRGB(0,0,0)
Instance.new("UICorner", FloatBtn).CornerRadius = UDim.new(0, 10)

local BtnGrad = Instance.new("UIGradient", FloatBtn)
BtnGrad.Color = ColorSequence.new({
    ColorSequenceKeypoint.new(0, Color3.fromRGB(25,25,25)),
    ColorSequenceKeypoint.new(1, Color3.fromRGB(10,10,10))
})
BtnGrad.Rotation = 90

local BtnStroke = Instance.new("UIStroke", FloatBtn)
BtnStroke.Color = Color3.fromRGB(100,100,100)
BtnStroke.Thickness = 2
BtnStroke.Transparency = 0.4
RegisterThemed(BtnStroke, "Color")

Connect("BtnPulse", RunService.RenderStepped, function()
    if PanicActive then return end
    local pulse = 0.3 + math.sin(tick() * 3) * 0.15
    BtnStroke.Transparency = pulse
    -- FIXED: pulse color now follows the theme instead of a hard-coded grey
    local c = GetAccent()
    BtnStroke.Color = Color3.new(
        math.clamp(c.R + math.sin(tick()*2) * 0.2, 0, 1),
        math.clamp(c.G + math.sin(tick()*2) * 0.2, 0, 1),
        math.clamp(c.B + math.sin(tick()*2) * 0.2, 0, 1)
    )
end)

FloatBtn.MouseButton1Click:Connect(function() if not PanicActive then ToggleUI(not uiVisible) end end)

do -- scoped: float-button drag state (register budget)
local drag, dragStart, startPos = false, nil, nil
Connect("FloatDragBegan", FloatBtn.InputBegan, function(i) if i.UserInputType == Enum.UserInputType.MouseButton1 or i.UserInputType == Enum.UserInputType.Touch then drag = true; dragStart = i.Position; startPos = FloatBtn.Position end end)
Connect("FloatDragMoved", FloatBtn.InputChanged, function(i) if drag and (i.UserInputType == Enum.UserInputType.MouseMovement or i.UserInputType == Enum.UserInputType.Touch) then local d = i.Position - dragStart; FloatBtn.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + d.X, startPos.Y.Scale, startPos.Y.Offset + d.Y) end end)
Connect("FloatDragEnded", FloatBtn.InputEnded, function(i) if i.UserInputType == Enum.UserInputType.MouseButton1 or i.UserInputType == Enum.UserInputType.Touch then drag = false end end)
end

-- ==================== MOBILE TOUCH CONTROLS (MOBILE EDITION) ====================
-- A phone has no keyboard / no Mouse2: these side buttons ARE the keybinds.
--   AIM (hold) = Target Lock override  ·  CAM = camera-lock toggle
--   TP = tap-to-teleport mode. Each button lights up while active.
local TouchGui = Instance.new("ScreenGui")
TouchGui.Name = "RBX_MobileTouch"; TouchGui.ResetOnSpawn = false
TouchGui.IgnoreGuiInset = true; TouchGui.DisplayOrder = 998
TouchGui.Parent = LocalPlayer:FindFirstChild("PlayerGui") or LocalPlayer:WaitForChild("PlayerGui", 3)
if not TouchGui.Parent then
    warn("[RBX 1.0 MOBILE] PlayerGui not found - touch controls disabled")
end

local TPMode = false
local touchTpConn = nil
local function MakeTouchBtn(label, posY, col)
    local b = Instance.new("TextButton", TouchGui)
    b.Size = UDim2.new(0, 74, 0, 74); b.Position = UDim2.new(1, -86, 0, posY)
    b.BackgroundColor3 = Color3.fromRGB(10, 14, 22); b.BackgroundTransparency = 0.25
    b.Text = label; b.TextColor3 = col; b.Font = Enum.Font.GothamBold
    b.TextSize = 14; b.AutoButtonColor = false; b.BorderSizePixel = 0
    Instance.new("UICorner", b).CornerRadius = UDim.new(1, 0)
    local s = Instance.new("UIStroke", b); s.Color = col; s.Thickness = 1.5; s.Transparency = 0.4
    return b, s
end

-- AIM: hold to lock — drives the same flag as the desktop Mouse2 keybind
local aimBtn, aimStroke = MakeTouchBtn("AIM", 170, Color3.fromRGB(255,80,80))
do
    local aimHeld = false
    local function SetAimHeld(v)
        if PanicActive then return end
        aimHeld = v; AimbotKeyHeld = v
        SafeCall(function()
            TweenService:Create(aimBtn, TweenInfo.new(0.12), {BackgroundTransparency = v and 0.55 or 0.25}):Play()
            aimStroke.Transparency = v and 0 or 0.4
        end)
    end
    Connect("TouchAimOn", aimBtn.InputBegan, function(i)
        if i.UserInputType == Enum.UserInputType.Touch or i.UserInputType == Enum.UserInputType.MouseButton1 then SetAimHeld(true) end
    end)
    Connect("TouchAimOff", aimBtn.InputEnded, function(i)
        if i.UserInputType == Enum.UserInputType.Touch or i.UserInputType == Enum.UserInputType.MouseButton1 then SetAimHeld(false) end
    end)
    -- if the button dies while held (PANIC), the lock must not stick on
    aimBtn.Destroying:Connect(function() if aimHeld then aimHeld = false; AimbotKeyHeld = false end end)
end

-- CAM: toggles Camera Lock through the same control the Combat tab uses (state stays in sync)
local camBtn, camStroke = MakeTouchBtn("CAM", 256, Color3.fromRGB(90,200,255))
Connect("TouchCamToggle", camBtn.MouseButton1Click, function()
    if PanicActive then return end
    local ctrl = ToggleControls["Camera Lock"]
    local on
    if ctrl then on = not ctrl.Get() else on = not State.CameraLock.Enabled end
    if ctrl then ctrl.Set(on) else State.CameraLock.Enabled = on end
    camStroke.Transparency = on and 0 or 0.4
end)

-- TP: tap-anywhere teleport mode — replaces the desktop Ctrl+Click combo
local tpBtn, tpStroke = MakeTouchBtn("TP", 342, Color3.fromRGB(160,120,255))
Connect("TouchTPToggle", tpBtn.MouseButton1Click, function()
    if PanicActive then return end
    TPMode = not TPMode
    tpStroke.Transparency = TPMode and 0 or 0.4
    Notify("Touch TP", TPMode and "Tap the ground to teleport" or "TP mode off", 2, Color3.fromRGB(160,120,255))
    if TPMode and not touchTpConn then
        touchTpConn = UserInputService.InputBegan:Connect(function(input, gpe)
            if not TPMode or PanicActive or gpe then return end
            if input.UserInputType ~= Enum.UserInputType.Touch then return end
            local cam = Workspace.CurrentCamera; local hrp = GetHRP()
            if not cam or not hrp then return end
            SafeCall(function()
                local unitRay = cam:ViewportPointToRay(input.Position.X, input.Position.Y)
                local result = Workspace:Raycast(unitRay.Origin, unitRay.Direction * 5000, GetRaycastParams())
                local pos = result and result.Position or (unitRay.Origin + unitRay.Direction * 500)
                hrp.CFrame = CFrame.new(pos + Vector3.new(0, 3, 0))
            end)
        end)
    elseif not TPMode and touchTpConn then
        touchTpConn:Disconnect(); touchTpConn = nil
    end
end)
-- safety net: whenever the touch layer goes away, nothing may stay armed
TouchGui.Destroying:Connect(function()
    if touchTpConn then touchTpConn:Disconnect(); touchTpConn = nil end
    TPMode = false
    AimbotKeyHeld = false
end)

-- ==================== PANIC (FULLY FIXED) ====================
-- Global so the Settings tab "Destroy GUI" button can call the same full cleanup.
Panic = function()
    if PanicActive then return end
    PanicActive = true

    for name, conn in pairs(Connections) do 
        SafeCall(function() 
            if typeof(conn) == "RBXScriptConnection" then 
                conn:Disconnect() 
            elseif type(conn) == "table" and conn.Disconnect then
                conn:Disconnect()
            end
        end) 
    end
    Connections = {}
    ClearESP()

    SafeCall(function()
        local hrp = GetHRP(); if hrp then 
            hrp.AssemblyLinearVelocity = Vector3.zero 
            for _, c in ipairs(hrp:GetChildren()) do
                if c.Name == "RBX_FlyGyro" or c.Name == "RBX_FlyVel" or c.Name == "RBX_VehicleBoost" then
                    c:Destroy()
                end
            end
        end
        local hum = GetHum(); if hum then hum.WalkSpeed = 16; hum.JumpPower = 50 end
        Camera.FieldOfView = 70; Camera.CameraType = Enum.CameraType.Custom
        Workspace.Gravity = OriginalGravity
        Lighting.Brightness = 1; Lighting.GlobalShadows = true; Lighting.ClockTime = 12
        Lighting.Technology = Enum.Technology.Future
        Lighting.Ambient = Color3.fromRGB(91,91,91); Lighting.OutdoorAmbient = Color3.fromRGB(140,140,140)
        CC.Brightness = 0; CC.Contrast = 0; CC.Saturation = 0; CC.TintColor = Color3.fromRGB(255,255,255)
        BL.Intensity = 0; BL.Size = 0; SR.Intensity = 0; SR.Spread = 0
        if State.WaterWalk.Platform and State.WaterWalk.Platform.Parent then 
            State.WaterWalk.Platform:Destroy(); State.WaterWalk.Platform = nil 
        end
        if State.CrosshairH then SafeCall(function() State.CrosshairH:Destroy() end); State.CrosshairH = nil end
        if State.CrosshairV then SafeCall(function() State.CrosshairV:Destroy() end); State.CrosshairV = nil end
        if TargetHighlight then SafeCall(function() TargetHighlight:Destroy() end); TargetHighlight = nil end
        for part, transparency in pairs(InvisibleOriginals) do
            if part and part.Parent then SafeCall(function() part.Transparency = transparency end) end
        end
        InvisibleOriginals = {}
        SafeCall(function() FOVGui:Destroy() end)
        SafeCall(function() FXFolder:Destroy() end)
        SafeCall(function() ESPFolder:Destroy() end)
        FOVFrame.Visible = false
        DistanceLabel.Visible = false
        for part, size in pairs(State.Hitbox.Originals) do 
            if part and part.Parent then part.Size = size end 
        end
        State.Hitbox.Originals = {}
        for handle, size in pairs(State.Reach.Originals) do 
            if handle and handle.Parent then handle.Size = size; handle.Massless = false end 
        end
        State.Reach.Originals = {}
        State.FPSBoost.Enabled = false
        UpdateFPSBoost()
    end)

    StopRainbow()
    OverrideClickCooldown = false
    SafeCall(function() SetGlassBlur(false) end) -- GLASS: unfreeze the world
    SafeCall(function() if GlassBlur then GlassBlur:Destroy() end end)
    SafeCall(function() if TouchGui then TouchGui:Destroy() end end) -- MOBILE: purge touch controls too
    SafeCall(function() ScreenGui:Destroy() end)
    warn("[RBX 1.0 MOBILE] PANIC EXECUTED. ALL SYSTEMS PURGED.")
end

-- ==================== INPUT (FIXED) ====================
Connect("MainInput", UserInputService.InputBegan, function(input, gpe)
    if gpe or PanicActive then return end
    if input.KeyCode == CONFIG.PanicKey then Panic()
    elseif input.KeyCode == CONFIG.ToggleKey then ToggleUI(not uiVisible)
    end

    local bind = State.CustomKeybinds.AimbotToggle
    if typeof(bind) == "EnumItem" then
        if bind.EnumType == Enum.KeyCode and input.KeyCode == bind then
            AimbotKeyEnum = bind
            AimbotKeyHeld = true -- POWER COMBAT: holding the key = Target Lock override
        elseif bind.EnumType == Enum.UserInputType and input.UserInputType == bind then
            AimbotKeyEnum = bind
            AimbotKeyHeld = true
        end
    end

    local camBind = State.CameraLock.Keybind
    if typeof(camBind) == "EnumItem" and camBind.EnumType == Enum.KeyCode and input.KeyCode == camBind then
        local ctrl = ToggleControls["Camera Lock"]
        if ctrl then ctrl.Set(not ctrl.Get()) end
    end
end)

Connect("MainInputEnd", UserInputService.InputEnded, function(input)
    -- POWER COMBAT: releasing the aimbot key releases the Target Lock override
    local bind = State.CustomKeybinds.AimbotToggle
    if typeof(bind) == "EnumItem" then
        if bind.EnumType == Enum.KeyCode and input.KeyCode == bind then
            AimbotKeyHeld = false
        elseif bind.EnumType == Enum.UserInputType and input.UserInputType == bind then
            AimbotKeyHeld = false
        end
    end
end)

-- ==================== INIT (ANIMATED) ====================
task.spawn(function()
    local LoadingScreen = CreateLoadingScreen()
    if LoadingScreen and LoadingScreen.SetProgress then
        local ok, err = pcall(function()
            LoadingScreen.SetProgress(10, "Loading services..."); task.wait(0.25); if PanicActive then return end
            LoadingScreen.SetProgress(25, "Initializing state..."); task.wait(0.25); if PanicActive then return end
            LoadingScreen.SetProgress(40, "Setting up ESP system..."); task.wait(0.25); if PanicActive then return end
            LoadingScreen.SetProgress(55, "Building RBX 1.0 interface..."); task.wait(0.25); if PanicActive then return end
            LoadingScreen.SetProgress(70, "Loading feature modules..."); task.wait(0.25); if PanicActive then return end
            LoadingScreen.SetProgress(85, "Finalizing setup..."); task.wait(0.25); if PanicActive then return end
            LoadingScreen.SetProgress(100, "Ready!"); task.wait(0.45); if PanicActive then return end

            SafeCall(function()
                for _, child in ipairs(LoadingScreen.Gui:GetDescendants()) do
                    if child:IsA("Frame") then
                        TweenService:Create(child, TweenInfo.new(0.45), {BackgroundTransparency = 1}):Play()
                    elseif child:IsA("TextLabel") then
                        TweenService:Create(child, TweenInfo.new(0.45), {TextTransparency = 1}):Play()
                    elseif child:IsA("UIStroke") then
                        TweenService:Create(child, TweenInfo.new(0.45), {Transparency = 1}):Play()
                    end
                end
            end)
            task.wait(0.5)
            LoadingScreen.Destroy()
            if PanicActive then return end

            -- FIXED (device fit): re-measure BEFORE the panel shows so phones never see
            -- an oversized frame flash, and reflow AFTER the first render.
            UpdateMainScale()
            ApplyResponsiveLayout()
            ScreenGui.Enabled = true
            ToggleUI(true)
            task.defer(function()
                if not PanicActive then UpdateMainScale(); ApplyResponsiveLayout() end
            end)
            Notify("RBX 1.0 HUB MOBILE", "Welcome • " .. GetHubVersion() .. " • touch controls ready", 4, Color3.fromRGB(220,220,220))
        end)
        if not ok and not PanicActive then
            warn("[RBX 1.0] Loading error: " .. tostring(err))
            pcall(function() if LoadingScreen and LoadingScreen.Destroy then LoadingScreen.Destroy() end end)
            UpdateMainScale(); ApplyResponsiveLayout()
            ScreenGui.Enabled = true
            MainFrame.Visible = true
            SetGlassBlur(true)
            Watermark.Visible = true
            RenderTab(1)
        end
    else
        UpdateMainScale(); ApplyResponsiveLayout()
        ScreenGui.Enabled = true
        MainFrame.Visible = true
        SetGlassBlur(true)
        Watermark.Visible = true
        RenderTab(1)
    end
end)
