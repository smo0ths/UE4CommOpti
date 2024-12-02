## updated 12/2/2024 ✂ 📋 :ramen: v1.200.23

### for UE4 and UE5* games for reference/customization/optimization/learning

#### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

#### my config is trying to be quality and perform well for any UE4/5 game, it might not be perfectly optimal for a specific game

#### [Installing and optimizing nvidia drivers here](https://github.com/smo0ths/Installing-and-optimizing-new-nvidia-drivers-on-windows-11-gaming-PC)

#### 2560x1440 (~2k) use 58%(balance) 67%(quality) 70%(custom/TAAU) scaling for PERFORMANCE (higher if cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR/NIS/IS)

#### 3328x1872 (3.25K) use 50%(performance/TAAU) scaling for PERFORMANCE (higher if cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR/NIS/IS)

#### 3840x2160 (~4K UHD) use 33%(ultra performance) 50%(performance/TAAU) scaling for PERFORMANCE (higher if cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR/NIS/IS)

#### negative LOD bias -1/-0.6 or 0 for PERFORMANCE (0 is best on proper mipmaps/textures) (set by nvidiaProfileInspector)

---

## Open Engine.ini and copy pasta %localappdata%

#### or UnrealPak method (Engine\Config\Windows\WindowsEngine.ini)

#### check 🟢 options for more fps

#### High config (works with UE5*)

```python
[Core.Log]
Global=off;

[/Script/Engine.Engine]
bPauseOnLossOfFocus=0;
bSmoothFrameRate=0;
bUseFixedFrameRate=0;

[TextureStreaming]
PoolSizeVRAMPercentage=70; 🟢 50 to lower vram usage 🟡 def 70 🔵 texturepool cache

[ConsoleVariables]
D3D12.InsertOuterOcclusionQuery=0; 🟢 1 for PERFORMANCE 🟡 def 0
demo.LoadCheckpointGarbageCollect=0; ⚪ EDITED 🟡 def 1
foliage.DensityScale=1; 🟢 0.6 for PERFORMANCE 🟡 def 1
foliage.MinimumScreenSize=0.0001; ⚪ EDITED 🟡 def 0.000005
fx.EnableCircularAnimTrailDump=0; ⚪ EDITED 🟡 def 2
fx.Niagara.QualityLevel=2; 🟢 0 for PERFORMANCE 🟡 def 3 🔵 0,1,2,3,4 low,med,high,ultra,cine
fx.ParticlePerfStats.Enabled=0; ⚪ EDITED 🟡 def 1
grass.DensityScale=0.8; 🟢 0.6 for PERFORMANCE ⚪ EDITED 🟡 def 1
grass.DisableDynamicShadows=0; 🟢 1 for PERFORMANCE 🟡 def 0
memory.logGenericPlatformMemoryStats=0; ⚪ EDITED 🟡 def 1
p.AnimDynamics=1; 🟢 0 for PERFORMANCE 🟡 def 1
p.AnimDynamicsWind=1; 🟢 0 for PERFORMANCE 🟡 def 1
p.RigidBodyNode=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.AllowLandscapeShadows=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.AllowSimpleLights=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.AmbientOcclusionLevels=-1; 🟢 0,1 for PERFORMANCE 🟡 def -1
r.AmbientOcclusionStaticFraction=-1; 🟢 0 for PERFORMANCE 🟡 def -1
r.AnisotropicMaterials=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.AOGlobalDistanceField.MipFactor=4; 🟢 8 for PERFORMANCE 🟡 def 4
r.AOQuality=2; 🟢 0,1 for PERFORMANCE 🟡 def 2
r.BloomQuality=4; 🟢 0 for PERFORMANCE ⚪ EDITED 🟡 def 5
r.BlurGBuffer=0; ⚪ EDITED 🟡 def -1
r.CapsuleShadows=0; 🟢 0 for PERFORMANCE ⚪ EDITED 🟡 def 1
r.ContactShadows=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.DefaultFeature.MotionBlur=0; ⚪ EDITED 🟡 def 1
r.DepthOfFieldQuality=1; 🟢 0,1 for PERFORMANCE ⚪ EDITED 🟡 def 2
r.DetailMode=2; 🟢 0,1 for PERFORMANCE ⚪ EDITED 🟡 def 3 🔵 0,1,2,3 low,med,high,epic
r.DFShadowQuality=2; 🟢 0,1,2 for PERFORMANCE ⚪ EDITED 🟡 def 3
r.DistanceFields.MaxPerMeshResolution=128; 🟢 128 for PERFORMANCE ⚪ EDITED 🟡 def 256
r.DOF.Gather.AccumulatorQuality=0; ⚪ EDITED 🟡 def 1
r.DOF.Gather.EnableBokehSettings=0; ⚪ EDITED 🟡 def 1
r.DOF.Gather.PostfilterMethod=0; ⚪ EDITED 🟡 def 1
r.DOF.Gather.RingCount=3; ⚪ EDITED 🟡 def 5
r.DOF.Kernel.MaxBackgroundRadius=0.012; ⚪ EDITED 🟡 def 0.025
r.DOF.Kernel.MaxForegroundRadius=0.012; ⚪ EDITED 🟡 def 0.025
r.DOF.Recombine.Quality=0; ⚪ EDITED 🟡 def 2
r.DOF.Scatter.BackgroundCompositing=1; ⚪ EDITED 🟡 def 2
r.DOF.Scatter.EnableBokehSettings=0; ⚪ EDITED 🟡 def 1
r.DOF.Scatter.ForegroundCompositing=1; 🟡 def 1
r.DOF.Scatter.MaxSpriteRatio=0.04; 🟡 def 0.1
r.EmitterSpawnRateScale=1; 🟢 0.125,0.25,0.5 for PERFORMANCE 🟡 def 1
r.EnableDebugSpam_GetObjectPositionAndScale=0; ⚪ EDITED 🟡 def 1 🔵 debug
r.EyeAdaptationQuality=2; 🟢 1 for PERFORMANCE 🟡 def 2 🔵 eyeadaptation,autoexposure
r.FilmGrain=0; ⚪ EDITED 🟡 def 1
r.gpucrash.collectionenable=0; ⚪ EDITED 🟡 def 1 🔵 debug
r.HairStrands.Enable=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.HairStrands.MinLOD=2; 🟢 2 for PERFORMANCE ⚪ EDITED 🟡 def 1
r.HairStrands.SkyAO=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.HairStrands.UseCardsInsteadOfStrands=1; 🟢 1 for PERFORMANCE ⚪ EDITED 🟡 def 0
r.HairStrands.Visibility.MSAA.SamplePerPixel=2; 🟢 2 for PERFORMANCE ⚪ EDITED 🟡 def 4
r.HFShadowQuality=2; 🟢 0,1 for PERFORMANCE 🟡 def 2
r.LandscapeLODBias=0; 🟢 1 for PERFORMANCE 🟡 def 0
r.LensFlareQuality=2; 🟢 0,1 for PERFORMANCE 🟡 def 2
r.LightMaxDrawDistanceScale=1; 🟢 0.5,0.6 for PERFORMANCE 🟡 def 1
r.LightShaftBlurPasses=2; ⚪ EDITED 🟡 def 3
r.LightShaftFirstPassDistance=0.08; ⚪ EDITED 🟡 def 0.1
r.LightShaftQuality=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Lumen.Reflections.DownsampleFactor=1; 🟢 2 for PERFORMANCE 🟡 def 1
r.Lumen.Reflections.ScreenSpaceReconstruction=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Lumen.Reflections.ScreenTraces=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Lumen.TranslucencyReflections.FrontLayer.Allow=0; 🟢 0 for PERFORMANCE 🟡 def 1
r.Lumen.TranslucencyReflections.FrontLayer.Enable=0; 🟢 0 for PERFORMANCE 🟡 def 0
r.Lumen.TranslucencyReflections.FrontLayer.EnableForProject=0; 🟢 0 for PERFORMANCE 🟡 def 0
r.LumenScene.SurfaceCache.NaniteMultiView=0; ⚪ EDITED 🟡 def 1
r.MaterialQualityLevel=1; 🟢 0,2 for PERFORMANCE 🟡 def 1 🔵 0,1,2,3 low,high,med,epic
r.MaxAnisotropy=16; 🟢 0,4,8 for PERFORMANCE ⚪ EDITED 🟡 def 8
r.MinScreenRadiusForLights=0.03; 🟢 0.04,0.06 for PERFORMANCE 🟡 def 0.03
r.MotionBlurQuality=0; ⚪ EDITED 🟡 def 4
r.Nanite.Streaming.MaxPageInstallsPerFrame=64; 🟢 64 for PERFORMANCE ⚪ EDITED 🟡 def 128
r.NGX.DLSS.DilateMotionVectors=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.NGX.DLSS.PreferNISSharpen=0; ⚪ EDITED 🟡 def 1
r.NGX.DLSS.Quality.Auto=0; ⚪ EDITED 🟡 def 1
r.NGX.DLSS.Quality=1; ⚪ EDITED 🟡 def -1 🔵 -2,-1,0,1,2 ultra perf,perf,balanced,quality,ultra
r.NGX.LogLevel=0; ⚪ EDITED 🟡 def 1 🔵 debug
r.ParallelShadows=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.ParticleLightQuality=1; 🟢 0,1 for PERFORMANCE 🟡 def 2
r.RefractionQuality=1; 🟢 0,1 for PERFORMANCE ⚪ EDITED 🟡 def 2
r.SceneColorFormat=3; 🟢 2,3 for PERFORMANCE ⚪ EDITED 🟡 def 4
r.SceneColorFringe.Max=0; ⚪ EDITED 🟡 def -1
r.Shadow.CachedShadowsCastFromMovablePrimitives=1; 🟢 0 for PERFORMANCE 🟡 def 1 🔵 movable light shadows
r.Shadow.CSM.MaxCascades=2; 🟢 1,2 for PERFORMANCE ⚪ EDITED 🟡 def 10
r.Shadow.DistanceScale=1; 🟢 0.7 for PERFORMANCE 🟡 def 1
r.Shadow.FilterMethod=0; 🟢 0 for PERFORMANCE 🟡 def 0 🔵 pcss shadows
r.Shadow.ForceSingleSampleShadowingFromStationary=0; 🟢 1 for PERFORMANCE 🟡 def 0
r.Shadow.MaxCSMResolution=2048; 🟢 512,1024 for PERFORMANCE 🟡 def 2048
r.Shadow.MaxResolution=512; 🟢 512,1024 for PERFORMANCE ⚪ EDITED 🟡 def 2048
r.Shadow.Nanite=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Shadow.NaniteLODBias=1; 🟢 1 for PERFORMANCE 🟡 def 1
r.Shadow.RadiusThreshold=0.04; 🟢 0.03,0.04,0.05,0.06 for PERFORMANCE ⚪ EDITED 🟡 def 0.01
r.ShadowQuality=5; 🟢 3,4 for PERFORMANCE 🟡 def 5
r.SkeletalMeshLODBias=0; 🟢 1 for PERFORMANCE 🟡 def 0 🔵 0,1,2 high,med,low
r.SkyAtmosphere.AerialPerspectiveLUT.DepthResolution=8; 🟢 8 for PERFORMANCE ⚪ EDITED 🟡 def 16
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; 🟢 1 for PERFORMANCE 🟡 def 1
r.SkyAtmosphere.AerialPerspectiveLUT.SampleCountMaxPerSlice=2; 🟢 2 for PERFORMANCE ⚪ EDITED 🟡 def 4
r.SkyAtmosphere.FastSkyLUT.SampleCountMax=32; 🟢 16,32,64 for PERFORMANCE ⚪ EDITED 🟡 def 128
r.SkyAtmosphere.FastSkyLUT.SampleCountMin=4; 🟢 1 for PERFORMANCE 🟡 def 4
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; 🟢 0 for PERFORMANCE 🟡 def 0
r.SkyAtmosphere.SampleCountMax=32; 🟢 16,32,64 for PERFORMANCE ⚪ EDITED 🟡 def 128
r.SkyAtmosphere.SampleCountMin=4; 🟢 1 for PERFORMANCE 🟡 def 4
r.SkyAtmosphere.SampleLightShadowmap=0; 🟢 0 for PERFORMANCE ⚪ EDITED 🟡 def 1 🔵 volumetric shadows
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=0; 🟢 1 for PERFORMANCE 🟡 def 0
r.SSGI.Enable=0; 🟢 0 for PERFORMANCE 🟡 def 0
r.SSR.HalfResSceneColor=1; 🟢 1 for PERFORMANCE ⚪ EDITED 🟡 def 0
r.SSR.Quality=3; 🟢 0,2 for PERFORMANCE 🟡 def 3
r.SSS.Burley.Quality=0; 🟢 0 for PERFORMANCE ⚪ EDITED 🟡 def 1
r.SSS.Checkerboard=1; 🟢 1 for PERFORMANCE ⚪ EDITED 🟡 def 2
r.SSS.HalfRes=1; 🟢 1 for PERFORMANCE ⚪ EDITED 🟡 def 0
r.Streaming.HiddenPrimitiveScale=0.5; 🟢 0.5 for PERFORMANCE 🟡 def 0.5
r.Streaming.MipBias=0; 🟢 1 for PERFORMANCE 🟡 def 0
r.SubsurfaceScattering=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.TemporalAA.Upsampling=1; 🟢 0 for PERFORMANCE 🟡 def 1 🔵 TAAU
r.TessellationAdaptivePixelsPerTriangle=999999; 🟢 999999 for PERFORMANCE ⚪ EDITED 🟡 def 48
r.Tonemapper.Quality=2; ⚪ EDITED 🟡 def 5
r.TranslucencyLightingVolumeDim=48; 🟢 32,48 for PERFORMANCE ⚪ EDITED 🟡 def 64
r.TranslucencyVolumeBlur=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.ViewDistanceScale=1; 🟢 0.8 for PERFORMANCE 🟡 def 1
r.VolumetricCloud.EnableAtmosphericLightsSampling=1; 🟡 def 1
r.VolumetricCloud.EnableDistantSkyLightSampling=1; 🟡 def 1
r.VolumetricCloud.EnableLocalLightsSampling=0; 🟢 0 for PERFORMANCE 🟡 def 0 🔵 experimental
r.VolumetricCloud.Shadow.SampleAtmosphericLightShadowmap=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.VolumetricCloud.ShadowMap.MaxResolution=2048; 🟢 1024 for PERFORMANCE 🟡 def 2048
r.VolumetricCloud.ShadowMap.SpatialFiltering=1; 🟡 def 1
r.VolumetricCloud.ShadowMap.TemporalFiltering.NewFrameWeight=1; 🟡 def 1 🔵 experimental
r.VolumetricCloud.ShadowMap=1; 🟢 0 for PERFORMANCE 🟡 def 1 🔵 cloud shadows
r.VolumetricCloud.SkyAO=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.VolumetricCloud=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.VolumetricFog.HistoryWeight=0.95; ⚪ EDITED 🟡 def 0.9
r.VolumetricFog=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Water.EnableShallowWaterSimulation=0; 🟢 0 for PERFORMANCE ⚪ EDITED 🟡 def 1
r.Water.EnableUnderwaterPostProcess=0; 🟢 0 for PERFORMANCE ⚪ EDITED 🟡 def 1
r.Water.SingleLayer.SSR=0; 🟢 0 for PERFORMANCE ⚪ EDITED 🟡 def 1
r.Water.WaterMesh.TessFactorBias=0; 🟢 -1 for PERFORMANCE 🟡 def 0
t.Streamline.Reflex.Auto=0; ⚪ EDITED 🟡 def 1
t.Streamline.Reflex.Enable=1; ⚪ EDITED 🟡 def 0 🔵 nvidia reflex
t.Streamline.Reflex.Mode=2; ⚪ EDITED 🟡 def 1 🔵 1,2 reflex,reflex with boost
```

---

#### Open Input.ini and copy pasta %localappdata%

#### or UnrealPak method (Engine\Config\Windows\WindowsInput.ini)

```python
[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bEnableMouseSmoothing=0;
bF11TogglesFullscreen=0;
ButtonRepeatDelay=0.1;
bViewAccelerationEnabled=0;
DoubleClickTime=0.01; ⚪ EDITED 🟡 def 0.1
InitialButtonRepeatDelay=0.1; ⚪ EDITED 🟡 def 0.2
```

---

#### Open GameUserSettings.ini these commands can overwrite your config if they are here %localappdata%

#### you can turn down used scalability groups here or in game if they are being used

```python
[ScalabilityGroups]
sg.HairQuality=?;
sg.ResolutionQuality=?;

AmbientOcclusion=(Value=?);
AntiAliasingMode=(Value=?);
AudioQualityLevel=?;
bBounceLightEnabled=?;
bConsoleEnabled=?;
bDepthOfField=?;
bFlashlightShadowsEnabled=?;
bFrameLimitEnabled=?;
bMotionBlur=?;
bRTXAmbientOcclusionEnabled=?;
bRTXEnabled=?;
bRTXReflectionsEnabled=?;
bRTXShadowsEnabled=?;
bTelemetryEnabled=?;
bUseDynamicResolution=?;
bUseVSync=?;
ContactShadows=(Value=?);
ContactShadows=?;
DetailMode=(Value=?);
DFAO=?;
DistanceFieldShadows=?;
DlssQualitySetting=?;
DoubleKeyPressTime=?;
FoliageMinLOD=(Value=?);
FrameRateLimit=?;
FullscreenMode=?;
Gamma=?;
GlobalSensitivity=?;
GraphicsPresetIndex=?;
GraphicsQuality=?;
HDRDisplayOutputNits=?;
HZBOcclusion=(Value=?);
LastSavedAAQuality=?;
LastSavedAASamples=?;
MaterialQuality=(Value=?);
MaxAnisotropy=(Value=?);
MaxAnisotropy=?;
MaxFPS=?;
MenuFrameRateLimit=?;
OceanQuality=(Value=?);
OverrideOptions=(("r.command",(Value=?,bModified=True)),("r.command",(Value=?,bModified=True)));
PostFX_Saturation=?;
PostFX_Sharpness=?;
ResolutionScaleModifier=?;
ScreenPercentage=(Value=?);
SkeletalMeshLODBias=(Value=?);
TAASampleStorage=?;
TemporalAASamples=(Value=?);
Tessellation=(Value=?);
TessellationMode=(Value=?);
TextureStreamPoolSizeStorage=(Value=?);
WakeSim=(Value=?)
```

---

#### Open DeviceProfiles.ini for textures lods, mess around or just skip %localappdata%

```python
[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,                 MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,        MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,         MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Character,             MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,    MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,     MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,                MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,       MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,        MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,               MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,      MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,       MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Cinematic,             MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Effects,               MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=linear, MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,    MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,                MinLODSize=2048, MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_UI,                    MinLODSize=2048, MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,              MinLODSize=32,   MaxLODSize=32,                            LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,             MinLODSize=32,   MaxLODSize=32,                            LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,          MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_MobileFlattened,       MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_Face,     MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_LightMap, MinLODSize=32,   MaxLODSize=32,                            LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_ColorLookupTable,      MinLODSize=2048, MaxLODSize=2048,                          LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,     MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,     MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Bokeh,                 MinLODSize=256,  MaxLODSize=256,                           LODBias=0, MinMagFilter=linear, MipFilter=linear, MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_IESLightProfile,       MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,              MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_HierarchicalLOD,       MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_8BitData,                                                                         LODBias=0, MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_16BitData,                                                                        LODBias=0, MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
```

---
