## updated 12/6/2024 ✂ 📋 🌀 :ramen: v0.201.50

### for UE4 and UE5* games for reference/customization/optimization/learning

#### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

#### my config is trying to be quality and perform well for any UE4/5 game, it might not be perfectly optimal for a specific game

#### [Installing and optimizing nvidia drivers here](https://github.com/smo0ths/Installing-and-optimizing-new-nvidia-drivers-on-windows-11-gaming-PC)

#### check 🔴 options for more fps (left to right, performance to quality)

#### 2560x1440 use 🔴 58%,67%,70% for PERFORMANCE (higher when cpu bound) (DLSS/TAAU/TSR/CAS/FSR/XeSS/PSSR/NIS/IS)

#### 3328x1872 use 🔴 50%,58%,67% for PERFORMANCE (higher when cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR/NIS/IS)

#### 3840x2160 use 🔴 33%,50%,67% for PERFORMANCE (higher when cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR/NIS/IS)

#### negative LOD bias 0,-0.6,-1 for PERFORMANCE (0 is best on proper mipmaps/textures) (set by nvidiaProfileInspector)

## Open Engine.ini and copy pasta %localappdata%

#### or Repak.bat method (zzz_ENGINE_INI\Engine\Config\Windows\WindowsEngine.ini)

#### High config (works with UE5*)

```python
[Core.Log]
Global=off;

[/Script/Engine.Engine]
bPauseOnLossOfFocus=0;
bSmoothFrameRate=0;
bUseFixedFrameRate=0;

[TextureStreaming]
PoolSizeVRAMPercentage=70; 🔴 50 to lower vram usage 🔵 texturepool cache

[ConsoleVariables]
D3D12.InsertOuterOcclusionQuery=0; 🔴 1 for PERFORMANCE
D3D12.MaximumFrameLatency=1; 🔵 frame latency
demo.LoadCheckpointGarbageCollect=0;
foliage.DensityScale=0.8; 🔴 0.6,0.8 for PERFORMANCE
foliage.MinimumScreenSize=0.0001;
fx.EnableCircularAnimTrailDump=0;
fx.Niagara.Collision.CPUEnabled=0; 🔴 0 for PERFORMANCE
fx.Niagara.QualityLevel=2; 🔴 0,1,2 for PERFORMANCE
fx.ParticlePerfStats.Enabled=0;
grass.DensityScale=0.8; 🔴 0.6,0.8 for PERFORMANCE
grass.DisableDynamicShadows=0; 🔴 1 for PERFORMANCE
memory.logGenericPlatformMemoryStats=0;
p.AnimDynamics=1; 🔴 0 for PERFORMANCE
p.AnimDynamicsWind=1; 🔴 0 for PERFORMANCE
p.RigidBodyNode=1; 🔴 0 for PERFORMANCE
r.AllowLandscapeShadows=1; 🔴 0 for PERFORMANCE
r.AllowSimpleLights=1; 🔴 0 for PERFORMANCE
r.AnisotropicMaterials=1; 🔴 0 for PERFORMANCE
r.AutoExposure.IgnoreMaterials=0; 🔵 experimental
r.Bloom.ScreenPercentage=50;
r.BloomQuality=4; 🔴 0 for PERFORMANCE
r.BlurGBuffer=0;
r.CapsuleShadows=0; 🔴 0 for PERFORMANCE
r.ContactShadows=1; 🔴 0 for PERFORMANCE
r.DefaultFeature.MotionBlur=0;
r.DepthOfFieldQuality=1; 🔴 0,1 for PERFORMANCE
r.DetailMode=2; 🔴 0,1,2 for PERFORMANCE
r.DFShadowQuality=1; 🔴 1,2 for PERFORMANCE
r.DistanceFields.MaxPerMeshResolution=256; 🔴 128 for PERFORMANCE
r.DOF.Gather.AccumulatorQuality=0;
r.DOF.Gather.EnableBokehSettings=0;
r.DOF.Gather.PostfilterMethod=0;
r.DOF.Gather.RingCount=3;
r.DOF.Kernel.MaxBackgroundRadius=0.012;
r.DOF.Kernel.MaxForegroundRadius=0.012;
r.DOF.Recombine.Quality=0;
r.DOF.Scatter.BackgroundCompositing=1;
r.DOF.Scatter.EnableBokehSettings=0;
r.DOF.Scatter.ForegroundCompositing=1;
r.DOF.Scatter.MaxSpriteRatio=0.04;
r.DynamicRes.FrameTimeBudget=33.3;
r.DynamicRes.MinScreenPercentage=50;
r.DynamicRes.OperationMode=0;
r.DynamicRes.TargetedGPUHeadRoomPercentage=10;
r.EmitterSpawnRateScale=1; 🔴 0.125,0.25,0.5 for PERFORMANCE
r.EnableDebugSpam_GetObjectPositionAndScale=0; 🔵 debug
r.EyeAdaptationQuality=2; 🔴 1 for PERFORMANCE 🔵 eye adaptation
r.FilmGrain=0;
r.Filter.SizeScale=1;
r.Fog=1; 🔵 render fog
r.GBufferDiffuseSampleOcclusion=1; 🔵 bent normal maps
r.gpucrash.collectionenable=0; 🔵 debug
r.HairStrands.Enable=1; 🔴 0 for PERFORMANCE
r.HairStrands.MinLOD=1; 🔴 2 for PERFORMANCE
r.HairStrands.SkyAO=0; 🔴 0 for PERFORMANCE
r.HairStrands.UseCardsInsteadOfStrands=1; 🔴 1 for PERFORMANCE
r.HairStrands.Visibility.MSAA.SamplePerPixel=2; 🔴 2 for PERFORMANCE
r.HairStrands.Voxelization=0; 🔴 0 for PERFORMANCE 🔵 voxelization
r.HeightFieldShadowing=0; 🔵 height field shadowing
r.LandscapeLODBias=0; 🔴 1 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; 🔴 0.5,0.6 for PERFORMANCE
r.LightShaftBlurPasses=2;
r.LightShaftFirstPassDistance=0.08;
r.LightShaftQuality=1; 🔴 0 for PERFORMANCE
r.Lumen.DiffuseIndirect.Allow=1; 🔴 0 for PERFORMANCE 🔵 lumen global illumination
r.Lumen.DiffuseIndirect.SSAO=0;
r.Lumen.HardwareRayTracing=0; 🔴 0 for PERFORMANCE
r.Lumen.Reflections.Allow=1; 🔴 0 for PERFORMANCE 🔵 lumen reflections
r.Lumen.Reflections.DownsampleFactor=1; 🔴 2 for PERFORMANCE
r.Lumen.ScreenProbeGather.MaterialAO=1;
r.Lumen.ScreenProbeGather.ScreenSpaceBentNormal=1; 🔵 bent normal maps
r.Lumen.ScreenProbeGather.ShortRangeAO=1;
r.Lumen.TranslucencyReflections.FrontLayer.Allow=1; 🔴 0 for PERFORMANCE
r.Lumen.TranslucencyReflections.FrontLayer.Enable=1; 🔴 0 for PERFORMANCE
r.Lumen.TranslucencyReflections.FrontLayer.EnableForProject=1; 🔴 0 for PERFORMANCE
r.MaterialQualityLevel=1; 🔴 0,2 for PERFORMANCE
r.MaxAnisotropy=8; 🔴 0,4 for PERFORMANCE
r.MeshStreaming=0; 🔵 experimental
r.MinScreenRadiusForLights=0.03; 🔴 0.06,0.04 for PERFORMANCE
r.MipMapLODBias=0;
r.MotionBlurQuality=0;
r.NGX.DLSS.DilateMotionVectors=1; 🔴 0 for PERFORMANCE
r.NGX.DLSS.PreferNISSharpen=0;
r.NGX.DLSS.Quality.Auto=0;
r.NGX.LogLevel=0; 🔵 debug
r.ParallelShadows=1; 🔴 0 for PERFORMANCE
r.ParticleLightQuality=1; 🔴 0,1 for PERFORMANCE
r.PathTracing=0;
r.RayTracing=0;
r.ReflectionCaptureResolution=128;
r.RefractionQuality=1; 🔴 0,1 for PERFORMANCE
r.RenderTargetPoolMin=400;
r.SceneColorFormat=3; 🔴 2,3 for PERFORMANCE
r.SceneColorFringe.Max=0;
r.SecondaryScreenPercentage.GameViewport=0; 🔴 83.33 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=1; 🔴 0 for PERFORMANCE 🔵 movable light shadows
r.Shadow.CSM.MaxCascades=2; 🔴 1,2,4 for PERFORMANCE
r.Shadow.CSMShadowDistanceFadeoutMultiplier=1;
r.Shadow.DistanceScale=1; 🔴 0.7 for PERFORMANCE
r.Shadow.FilterMethod=0; 🔴 0 for PERFORMANCE 🔵 PCSS
r.Shadow.ForceSingleSampleShadowingFromStationary=0; 🔴 1 for PERFORMANCE
r.Shadow.MaxCSMResolution=2048; 🔴 512,1024 for PERFORMANCE
r.Shadow.MaxResolution=512; 🔴 512,1024 for PERFORMANCE
r.Shadow.Nanite=1; 🔴 0 for PERFORMANCE
r.Shadow.NaniteLODBias=1; 🔴 1 for PERFORMANCE
r.Shadow.PreShadowResolutionFactor=0.5;
r.Shadow.RadiusThreshold=0.04; 🔴 0.06,0.05,0.04,0.03 for PERFORMANCE
r.Shadow.Virtual.Cache.StaticSeparate=0;
r.Shadow.Virtual.Clipmap.FirstLevel=6;
r.Shadow.Virtual.Enable=1; 🔴 0 for PERFORMANCE
r.Shadow.Virtual.ForceOnlyVirtualShadowMaps=1; 🔴 1 for PERFORMANCE
r.Shadow.Virtual.MaxPhysicalPages=4096; 🔴 512,2048 to lower vram usage
r.Shadow.Virtual.OnePassProjection.MaxLightsPerPixel=8; 🔴 8 for PERFORMANCE
r.Shadow.Virtual.OnePassProjection=1; 🔴 1 for PERFORMANCE
r.Shadow.Virtual.ResolutionLodBiasDirectional=0; 🔴 0,-0.5,-1 for PERFORMANCE
r.Shadow.Virtual.ResolutionLodBiasDirectionalMoving=0; 🔴 0,-0.5,-1 for PERFORMANCE
r.Shadow.Virtual.ResolutionLodBiasLocal=1; 🔴 1 for PERFORMANCE
r.Shadow.Virtual.SMRT.MaxRayAngleFromLight=0.03;
r.Shadow.Virtual.SMRT.RayCountDirectional=4; 🔴 0,4 for PERFORMANCE
r.Shadow.Virtual.SMRT.RayCountLocal=4; 🔴 0,4 for PERFORMANCE
r.Shadow.Virtual.SMRT.RayLengthScaleDirectional=1;
r.Shadow.Virtual.SMRT.SamplesPerRayDirectional=2; 🔴 2 for PERFORMANCE
r.Shadow.Virtual.SMRT.SamplesPerRayLocal=2; 🔴 2 for PERFORMANCE
r.Shadow.Virtual.SMRT.TexelDitherScaleDirectional=2;
r.Shadow.Virtual.TranslucentQuality=0; 🔴 0 for PERFORMANCE
r.ShadowQuality=5; 🔴 3,4 for PERFORMANCE
r.SkeletalMeshLODBias=0; 🔴 2,1 for PERFORMANCE 🔵 skeletal mesh bias if supported
r.SkyAtmosphere.AerialPerspectiveLUT.DepthResolution=8; 🔴 8 for PERFORMANCE
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; 🔴 1 for PERFORMANCE
r.SkyAtmosphere.AerialPerspectiveLUT.SampleCountMaxPerSlice=2; 🔴 2 for PERFORMANCE
r.SkyAtmosphere.FastSkyLUT.SampleCountMax=32; 🔴 16,32,64 for PERFORMANCE
r.SkyAtmosphere.FastSkyLUT.SampleCountMin=4; 🔴 1 for PERFORMANCE
r.SkyAtmosphere.LUT32=0; 🔴 0 for PERFORMANCE
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; 🔴 0 for PERFORMANCE
r.SkyAtmosphere.SampleCountMax=32; 🔴 16,32,64 for PERFORMANCE
r.SkyAtmosphere.SampleCountMin=4; 🔴 1 for PERFORMANCE
r.SkyAtmosphere.SampleLightShadowmap=1; 🔴 0 for PERFORMANCE 🔵 volumetric shadows
r.SkyAtmosphere.TransmittanceLUT.SampleCount=10;
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=0; 🔴 1 for PERFORMANCE
r.SkyLight.RealTimeReflectionCapture.TimeSlice.SkyCloudCubeFacePerFrame=6;
r.SSGI.Enable=0; 🔴 0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; 🔴 1 for PERFORMANCE
r.SSR.Quality=3; 🔴 0,2 for PERFORMANCE
r.SSS.Burley.Quality=0; 🔴 0 for PERFORMANCE
r.SSS.Checkerboard=1; 🔴 1 for PERFORMANCE
r.SSS.HalfRes=1; 🔴 1 for PERFORMANCE
r.Streaming.AmortizeCPUToGPUCopy=0;
r.Streaming.Boost=1;
r.Streaming.DropMips=0; 🔵 debug
r.Streaming.FramesForFullUpdate=5;
r.Streaming.HiddenPrimitiveScale=0.5; 🔴 0.5 for PERFORMANCE
r.Streaming.LimitPoolSizeToVRAM=1;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.MaxNumTexturesToStreamPerFrame=0;
r.Streaming.MipBias=0; 🔴 1 for PERFORMANCE
r.Streaming.NumStaticComponentsProcessedPerFrame=50;
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.PoolSize=3000; 🔴 1000 to lower vram usage 🔵 texturepool size
r.Streaming.UseFixedPoolSize=0; 🔵 change poolsize at runtime
r.SubsurfaceScattering=1; 🔴 0 for PERFORMANCE
r.SupportMaterialLayers=1; 🔴 0 for PERFORMANCE
r.TemporalAA.Quality=2; 🔴 1 for PERFORMANCE
r.TemporalAA.Upsampling=1; 🔴 0 for PERFORMANCE 🔵 TAAU
r.TessellationAdaptivePixelsPerTriangle=999999; 🔴 999999 for PERFORMANCE
r.Tonemapper.Quality=2;
r.Tonemapper.Sharpen=-1;
r.Translucency.DynamicRes.TimeBudget=0;
r.TranslucencyLightingVolumeDim=48; 🔴 32,48 for PERFORMANCE
r.TranslucencyVolumeBlur=1; 🔴 0 for PERFORMANCE
r.Upscale.Quality=3; 🔴 1,2 for PERFORMANCE
r.ViewDistanceScale=1; 🔴 0.8 for PERFORMANCE
r.VolumetricCloud.DistanceToSampleMaxCount=15;
r.VolumetricCloud.EnableAtmosphericLightsSampling=1;
r.VolumetricCloud.EnableDistantSkyLightSampling=1;
r.VolumetricCloud.EnableLocalLightsSampling=0; 🔴 0 for PERFORMANCE 🔵 experimental
r.VolumetricCloud.ReflectionRaySampleMaxCount=80;
r.VolumetricCloud.SampleMinCount=2;2
r.VolumetricCloud.Shadow.ReflectionRaySampleMaxCount=24;
r.VolumetricCloud.Shadow.SampleAtmosphericLightShadowmap=1; 🔴 0 for PERFORMANCE
r.VolumetricCloud.Shadow.ViewRaySampleMaxCount=80;
r.VolumetricCloud.ShadowMap.MaxResolution=2048;
r.VolumetricCloud.ShadowMap.SpatialFiltering=1;
r.VolumetricCloud.ShadowMap=1; 🔴 0 for PERFORMANCE 🔵 cloud shadows
r.VolumetricCloud.SkyAO.MaxResolution=2048;
r.VolumetricCloud.SkyAO=1; 🔴 0 for PERFORMANCE
r.VolumetricCloud.ViewRaySampleMaxCount=768;
r.VolumetricCloud=1; 🔴 0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8; 🔴 16 for PERFORMANCE
r.VolumetricFog.GridSizeZ=128; 🔴 64 for PERFORMANCE
r.VolumetricFog=1; 🔴 0 for PERFORMANCE
r.VolumetricRenderTarget.Mode=2;
r.VolumetricRenderTarget.ReprojectionBoxConstraint=1;
r.VolumetricRenderTarget.UpsamplingMode=2;
r.VT.MaxAnisotropy=8; 🔴 0,4 for PERFORMANCE
r.VT.MaxTilesProducedPerFrame=30;
r.VT.MaxUploadsPerFrame=8;
r.Water.EnableShallowWaterSimulation=0; 🔴 0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=0; 🔴 0 for PERFORMANCE
r.Water.SingleLayer.SSR=0; 🔴 0 for PERFORMANCE
r.Water.WaterMesh.TessFactorBias=0; 🔴 -1 for PERFORMANCE
RHI.MaximumFrameLatency=1; 🔵 frame latency
t.Streamline.Reflex.Auto=0;
```

---

#### Open Input.ini and copy pasta %localappdata%

#### or Repak.bat method (zzz_ENGINE_INI\Engine\Config\Windows\WindowsInput.ini)

```python
[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bEnableMouseSmoothing=0;
bF11TogglesFullscreen=0;
ButtonRepeatDelay=0.1;
bViewAccelerationEnabled=0;
DoubleClickTime=0.01; def 0.1
InitialButtonRepeatDelay=0.1; def 0.2
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
