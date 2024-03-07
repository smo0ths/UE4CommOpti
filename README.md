#### updated 3/7/2024 ✂️ 📋 :ramen: v1.100.08

##### for UE4 games for reference/customization/optimization/learning

##### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

##### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

##### make sure your scaling % is set correctly! and match PIP(scope) resolution scaling in games (manually in graphic settings) for PERFORMANCE

##### 2560x1440 use 58%(balance) 67%(quality) 70%(custom/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/TSR/CAS/FSR123/XeSS)

##### 3200x1800 use 33%(ultra performance) 50%(performance/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/TSR/CAS/FSR123/XeSS)

##### 3840x2160 use 33%(ultra performance) 50%(performance/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/TSR/CAS/FSR123/XeSS)

---

<details><summary>Open Engine.ini and copy paste under lines in the file</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Engine.ini
</p>
</details>

```python
[Core.Log]
Global=off;

[Audio]
UseAudioThread=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=50;---------------🔵 EDITED 🟣 texturepool cache

[ConsoleVariables]
sg.ResolutionQuality=50;---------------🟡 set correctly
r.ScreenPercentage=50;---------------🟡 set correctly
r.TemporalAA.Upsampling=1;---------------🔵 EDITED 🟣 TAAU
r.TemporalAACurrentFrameWeight=0.03;
r.TemporalAASamples=8;
r.TemporalAA.Algorithm=0;---------------🟢 0 for PERFORMANCE 🟣 gen5 TAAU
r.TemporalAAFilterSize=0.1;---------------🔵 EDITED 🟣 req gen5 TAAU
r.SecondaryScreenPercentage.GameViewport=0;---------------🟢 83.33 for PERFORMANCE
r.DynamicRes.OperationMode=0;
r.MSAACount=0;---------------🔵 EDITED
r.GTSyncType=0;
r.VSync=0;
rhi.SyncInterval=0;
rhi.SyncSlackMS=0;
r.D3D11.UseAllowTearing=1;---------------🟣 dxgi flip mode
r.D3D12.UseAllowTearing=1;---------------🟣 dxgi flip mode
r.FidelityFX.FSR2.QualityMode=4;---------------🔵 EDITED 🟣 4,3,2,1 ultra perf,perf,balanced,quality 🟡 set correctly
r.NGX.DLSS.Quality=-2;---------------🔵 EDITED 🟣 -2,-1,0,1 ultra perf,perf,balanced,quality 🟡 set correctly
r.NGX.DLSS.Quality.Auto=0;---------------🟢 0 for PERFORMANCE
r.NGX.DLSS.PreferNISSharpen=0;---------------🔵 EDITED
r.NGX.DLSS.Sharpness=0;
r.NGX.DLSS.AutoExposure=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.NGX.DLSS.DilateMotionVectors=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.NGX.DLAA.Enable=0;---------------🟢 0 for PERFORMANCE
r.NGX.DLSS.Reflections.TemporalAA=0;
r.NGX.DLSS.WaterReflections.TemporalAA=0;
t.Streamline.Reflex.Enable=1;---------------🟣 nvidia reflex
t.Streamline.Reflex.Mode=2;---------------🟣 reflex on with boost
r.CompileShadersForDevelopment=1;---------------🟢 1 for PERFORMANCE
r.FinishCurrentFrame=0;
r.HZBOcclusion=0;
r.OneFrameThreadLag=1;---------------🟢 1 for PERFORMANCE
p.AnimDynamics=0;---------------🟢 0 for PERFORMANCE
p.AnimDynamicsWind=0;---------------🟢 0 for PERFORMANCE
p.RigidBodyNode=0;---------------🟢 0 for PERFORMANCE
p.ClothPhysics=1;
r.EyeAdaptationQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.EyeAdaptation.Basic.Compute=1;---------------🟢 1 for PERFORMANCE
r.Tonemapper.MergeWithUpscale.Mode=1;
r.Tonemapper.Quality=3;---------------🔵 EDITED
r.ToneMapper.Sharpen=0;
r.Tonemapper.GrainQuantization=0;
r.FilmGrain=0;
r.SceneColorFringeQuality=0;---------------🔵 EDITED
r.DefaultFeature.MotionBlur=0;---------------🔵 EDITED
r.MotionBlurQuality=0;---------------🔵 EDITED
r.BloomQuality=4;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.Bloom.Cross=0.4;---------------🔵 EDITED
r.Filter.SizeScale=0.7;---------------🔵 EDITED
r.Upscale.Quality=1;---------------🔵 EDITED
r.LensFlareQuality=1;---------------🟢 0,1 for PERFORMANCE
r.Filter.LoopMode=0;---------------🟢 0 for PERFORMANCE
r.DepthOfFieldQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.DOF.Gather.AccumulatorQuality=0;
r.DOF.Gather.PostfilterMethod=1;---------------🔵 EDITED
r.DOF.Gather.EnableBokehSettings=0;
r.DOF.Gather.RingCount=3;---------------🔵 EDITED
r.DOF.Scatter.ForegroundCompositing=0;---------------🔵 EDITED
r.DOF.Scatter.BackgroundCompositing=0;---------------🔵 EDITED
r.DOF.Scatter.EnableBokehSettings=0;
r.DOF.Scatter.MaxSpriteRatio=0.04;
r.DOF.Recombine.Quality=0;
r.DOF.TemporalAAQuality=0;
r.DOF.Kernel.MaxForegroundRadius=0.006;---------------🔵 EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;---------------🔵 EDITED
foliage.DensityScale=0.6;---------------🟢 0.6 for PERFORMANCE 🔵 EDITED
foliage.LODDistanceScale=0.8;
foliage.MinimumScreenSize=0.0001;
foliage.DitheredLOD=1;---------------🟢 1 for PERFORMANCE
grass.DensityScale=0.6;---------------🟢 0.6 for PERFORMANCE 🔵 EDITED
grass.CullDistanceScale=1;
grass.DisableDynamicShadows=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.MipMapLODBias=0;---------------🟢 1 for PERFORMANCE
r.ParticleLODBias=0;
r.LandscapeLODBias=0;---------------🟢 1 for PERFORMANCE
r.SkeletalMeshLODBias=0;---------------🟢 1 for PERFORMANCE
r.ViewDistanceScale=1;---------------🟢 0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;---------------🟢 0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1;
r.SkeletalMeshLODRadiusScale=0.75;---------------🟢 0.5,0.75 for PERFORMANCE 🔵 EDITED
r.DetailMode=1;---------------🟢 0,1 for PERFORMANCE
r.RefractionQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.MaterialQualityLevel=1;---------------🟢 0,2 for PERFORMANCE
r.SupportMaterialLayers=1;---------------🟢 0 for PERFORMANCE
r.SupportAnisotropicMaterials=1;---------------🟢 0 for PERFORMANCE
r.AnisotropicMaterials=1;---------------🟢 0 for PERFORMANCE
r.MaxAnisotropy=8;---------------🟢 0 for PERFORMANCE
r.VT.MaxAnisotropy=8;
r.AllowSimpleLights=1;---------------🟢 0 for PERFORMANCE
r.ParticleLightQuality=1;---------------🟢 0,1 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;---------------🟢 0.125,0.25 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=16;
r.SubsurfaceScattering=1;---------------🟢 0 for PERFORMANCE
r.SSS.Quality=0;
r.SSS.SampleSet=0;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.SSS.Checkerboard=1;---------------🟢 1 for PERFORMANCE
r.SSS.HalfRes=1;
r.SSS.Scale=1;
r.SSGI.Enable=0;---------------🟢 0 for PERFORMANCE
r.SSGI.Quality=0;---------------🟢 0,2 for PERFORMANCE 🔵 EDITED 🟣 req ssgi enable
r.SSGI.HalfRes=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.SSGI.LeakFreeReprojection=1;
r.ClearCoatNormal=1;---------------🟢 0 for PERFORMANCE
r.IrisNormal=1;---------------🟢 0 for PERFORMANCE
r.HairStrands.Enable=0;---------------🟢 0 for PERFORMANCE
r.TiledDeferredShading=1;---------------🟢 0 for PERFORMANCE 🔵 gpu lights
r.SceneColorFormat=3;---------------🟢 2,3 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=999999;---------------🟢 999999 for PERFORMANCE 🔵 EDITED
r.LightFunctionQuality=1;---------------🟢 0,1 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;---------------🟢 0.6 for PERFORMANCE
r.LightShaftQuality=1;---------------🟢 0 for PERFORMANCE
r.MinScreenRadiusForLights=0.03;---------------🟢 0.04,0.06 for PERFORMANCE 🔵 EDITED
r.AllowGlobalClipPlane=0;---------------🟢 0 for PERFORMANCE
r.chaos.ReflectionCaptureStaticSceneOnly=1;
r.SkyLight.RealTimeReflectionCapture=1;---------------🟢 0 for PERFORMANCE
r.HighQualityLightMaps=1;
r.MinRoughnessOverride=0;
r.SSR.MaxRoughness=-1;
r.SSR.HalfResSceneColor=1;---------------🟢 1 for PERFORMANCE
r.SSR.Quality=2;---------------🟢 0 for PERFORMANCE
r.SSR.Temporal=0;
r.Water.EnableShallowWaterSimulation=0;---------------🟢 0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.ShadersSupportDistanceFieldShadow=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.UnderwaterFog=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.UnderwaterFogWhenCameraIsAboveWater=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayerWater.SupportCloudShadow=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.RefractionDownsampleFactor=2;
r.Water.SingleLayer.SSR=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.SSRTAA=0;---------------🟢 0 for PERFORMANCE
r.Water.WaterMesh.LODScaleBias=-0.5;---------------🟢 -0.5 for PERFORMANCE 🔵 EDITED
r.Water.WaterMesh.LODCountBias=0;
r.Water.WaterMesh.LODMorphEnabled=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.Water.WaterMesh.TessFactorBias=-1;---------------🟢 -1 for PERFORMANCE 🔵 EDITED
r.Water.SingleLayer.TiledComposite=1;
r.Water.SingleLayer.DepthPrepass=0;
r.VolumetricFog=1;---------------🟢 0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=16;---------------🔵 EDITED
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.Jitter=1;
r.VolumetricFog.TemporalReprojection=1;
r.VolumetricFog.HistoryWeight=0.95;---------------🔵 EDITED
r.VolumetricFog.HistoryMissSupersampleCount=1;---------------🔵 EDITED
r.VolumetricFog.InverseSquaredLightDistanceBiasScale=1;
r.VolumetricCloud.DisableCompute=0;
r.VolumetricCloud.EnableAerialPerspectiveSampling=1;
r.VolumetricCloud.EnableAtmosphericLightsSampling=1;
r.VolumetricCloud.EnableDistantSkyLightSampling=1;
r.VolumetricCloud.EnableLocalLightsSampling=0;
r.VolumetricCloud.HighQualityAerialPerspective=0;
r.VolumetricCloud.Shadow.SampleAtmosphericLightShadowmap=0;
r.VolumetricCloud.ShadowMap=0;
r.VolumetricCloud.SkyAO=0;
r.SkyAtmosphere.SampleLightShadowmap=0;
r.SkyAtmosphere.DistantSkyLightLUT=1;
r.SkyAtmosphere.FastSkyLUT=1;
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1;
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0;
r.DistanceFields.MaxPerMeshResolution=128;
r.DistanceFields.ParallelAtlasUpdate=1;
r.DistanceFields.ForceMaxAtlasSize=1;---------------🔵 EDITED
r.DistanceFields.AtlasSizeZ=1024;
r.DistanceFields.AtlasSizeXY=512;
r.GenerateLandscapeGIData=0;---------------🟢 0 for PERFORMANCE 🟣 req generatemeshdistancefields
r.GenerateMeshDistanceFields=1;---------------🟢 0 for PERFORMANCE 🟣 dfs and dfao mesh
r.DistanceFieldShadowing=1;---------------🟢 0 for PERFORMANCE 🟣 req generatemeshdistancefields
r.DFShadowQuality=1;---------------🟢 0,1,2 for PERFORMANCE 🔵 EDITED 🟣 req distancefieldshadowing
r.DFFullResolution=0;---------------🟢 0 for PERFORMANCE
r.DFShadowScatterTileCulling=1;---------------🟢 1 for PERFORMANCE
r.CapsuleShadows=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.CapsuleDirectShadows=0;
r.CapsuleIndirectShadows=0;
r.CapsuleShadowsFullResolution=0;
r.ContactShadows=0;---------------🟢 0 for PERFORMANCE
r.ContactShadows.NonShadowCastingIntensity=0;
r.AllowLandscapeShadows=1;---------------🟢 0 for PERFORMANCE
r.Shadow.FilterMethod=0;---------------🟢 0 for PERFORMANCE 🟣 PCSS shadows
r.ShadowQuality=3;---------------🟢 3 for PERFORMANCE 🔵 EDITED
r.Shadow.DistanceScale=1;
r.Shadow.MaxCSMResolution=2048;---------------🟢 512,1024 for PERFORMANCE 🔵 EDITED
r.Shadow.MaxResolution=1024;---------------🟢 512,1024 for PERFORMANCE
r.Shadow.CSM.MaxCascades=2;---------------🟢 1,2 for PERFORMANCE 🔵 EDITED
r.Shadow.MaxNumFarShadowCascades=2;---------------🔵 EDITED
r.Shadow.CSM.TransitionScale=1;
r.Shadow.PreShadowResolutionFactor=0.5;
r.Shadow.RadiusThreshold=0.04;
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;---------------🟢 0 for PERFORMANCE 🟣 movable light shadows
r.Shadow.CacheWholeSceneShadows=1;
r.Shadow.CacheWPOPrimitives=0;
r.Shadow.ForceSingleSampleShadowingFromStationary=1;
r.Shadow.FarShadowDistanceOverride=0;
r.Shadow.FarShadowStaticMeshLODBias=1;
r.ParallelShadow=1;---------------🟢 0 for PERFORMANCE
r.ParallelShadowsNonWholeScene=0;---------------🟢 0 for PERFORMANCE
r.ParallelTranslucency=1;
r.TranslucencyLightingVolumeDim=32;---------------🟢 32 for PERFORMANCE 🔵 EDITED
r.TranslucencyVolumeBlur=1;---------------🟢 0 for PERFORMANCE
r.HLOD.DistanceScale=0.6;---------------🟢 0.6 for PERFORMANCE 🔵 EDITED
r.HLOD.ForceDisableCastDynamicShadow=0;---------------🟢 1 for PERFORMANCE
r.HeightFieldShadowing=0;---------------🟢 0 for PERFORMANCE
r.HFShadowQuality=0;---------------🟢 0,1 for PERFORMANCE 🟣 req heightfieldshadowing
r.HeightfieldGlobalIllumination=0;---------------🟢 0 for PERFORMANCE
r.DistanceFieldAO=1;---------------🟢 0 for PERFORMANCE 🟣 req generatemeshdistancefields
r.AOQuality=1;---------------🟢 0,1 for PERFORMANCE 🟣 req distancefieldao
r.AOGlobalDistanceField=0;---------------🟢 0 for PERFORMANCE 🟣 adaptive method
r.AOApplyToStaticIndirect=0;
r.AOMaxViewDistance=10000;
r.AmbientOcclusionMipLevelFactor=1;---------------🔵 EDITED
r.AmbientOcclusionMaxQuality=0;---------------🔵 EDITED
r.AmbientOcclusionLevels=2;---------------🟢 0,1 for PERFORMANCE
r.AmbientOcclusionRadiusScale=0.5;---------------🔵 EDITED
r.AmbientOcclusionStaticFraction=-1;---------------🟢 0 for PERFORMANCE
r.AmbientOcclusion.Method=0;
r.Streaming.MipBias=0;---------------🟢 1 for PERFORMANCE
r.Streaming.AmortizeCPUToGPUCopy=0;
r.Streaming.MaxNumTexturesToStreamPerFrame=0;
r.Streaming.FramesForFullUpdate=15;---------------🔵 EDITED
r.Streaming.HiddenPrimitiveScale=1;---------------🟢 0.5 for PERFORMANCE
r.Streaming.EnableOptionalMips=0;
r.Streaming.Boost=1;
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;
r.Streaming.LimitPoolSizeToVRAM=0;
r.Streaming.UseFixedPoolSize=0;
r.Streaming.PoolSize.Minimum=-1;
r.Streaming.PoolSize.MinimumFreeMemory=-1;
r.Streaming.PoolSize=800;---------------🔵 EDITED
r.Streaming.PoolSizeForMeshes=-1;
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.UseNewMetrics=1;
r.Streaming.UseMaterialData=1;
r.DiffuseIndirect.Denoiser=1;---------------🟢 1 for PERFORMANCE 🟣 denoiser
r.AmbientOcclusion.Denoiser=1;---------------🟢 1 for PERFORMANCE 🟣 denoiser
r.Shadow.Denoiser=0;---------------🟢 0 for PERFORMANCE 🟣 denoiser
r.Reflections.Denoiser.TemporalAccumulation=0;---------------🟣 denoiser
r.Reflections.Denoiser=0;---------------🔵 EDITED 🟣 denoiser
r.SSR.ExperimentalDenoiser=0;---------------🟣 denoiser
r.D3D12.GPUCrashDebuggingMode=0;---------------🟣 debug
r.gpucrash.collectionenable=0;---------------🟣 debug
r.GPUCrashDebugging=0;---------------🟣 debug
r.ShaderDevelopmentMode=0;---------------🟣 debug
r.UniformBufferPooling=1;---------------🟣 debug
r.NGX.LogLevel=0;---------------🟣 debug
fx.Niagara.QualityLevel=1;---------------🟣 wip
r.Lumen.DiffuseIndirect.Allow=0;---------------🟣 wip
r.Nanite=0;---------------🟣 wip
r.RayTracing=0;---------------🟣 wip
r.DynamicGlobalIlluminationMethod=0;----------------🟣 wip
r.ReflectionMethod=0;---------------🟣 wip
```
---

<details><summary>Open GameUserSettings.ini these commands will overwrite your config so make sure they are correct check for new stuff after updates, good luck</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/GameUserSettings.ini
</p>
</details>

```python
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

<details><summary>Open Input.ini and edit input commands or add them</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Input.ini
</p>
</details>

```python
[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.1;---------------🔵 EDITED
ButtonRepeatDelay=0.1;
DoubleClickTime=0.15;---------------🔵 EDITED
```

---

<details><summary>Open DeviceProfiles.ini for textures lods, mess around or just skip this, could be more optimized</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
</p>
</details>

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

#### Open NVIDIA Control Panel

##### 1. 3D settings -> adjust image settings with preview -> use my preference emphasizing performance apply.

##### 2. click on use the advanced 3D image settings and apply then click "take me there"

##### 3. Anisotropic filtering:  set Application-controlled (you can force the setting in here if you can't notice it working in certain games)

##### 4. Low latency mode (Only works with dx11 and lower api):

###### Off and ~85% gpu usage for multiple frame buffers sacrificing latency (cap fps til gpu usage is ~85%) (for visual fluidity of frames)

###### On forces 1 frame buffer (for lower latency than off) (for visual fluidity of frames and less latency)

###### Ultra and high gpu usage for lowest latency

###### Nvidia relfex is in-game and dx12 only and you should use it just like Ultra low latency mode with high gpu usage

##### 5. Power management mode:  prefer max performance  (this is the "+ boost" in reflex + boost)

##### 6. Preferred refresh rate:  Highest available

##### 7. Texture filtering - anisotropic sample optimization:  on  (off will look better if this even works in your game)

##### 8. Texture filtering - negative LOD bias:  allow (allows a negative bias) clamp (0 mipmap bias) test yourself devs usually set slight negative clamps, also negative with DLSS/FSR2 upscaling

##### 9. Texture filtering quality:  high performance

##### 10. Texture filtering - trilinear optimization:  on

##### 11. Vertical sync:  Off

##### 12. Display -> Adjust desktop size and position -> set Perform scaling on: Display

#### Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method)

###### NVCleanstall enabling it in advanced settings before installing or

#### Manually enable Message-signaled interrupts (MSIs)

###### win + r type cmd then press control+shift+enter (starts as admin) then add key. NVcleaninstall gives you more MSIs options. Newest drivers auto do this on 40 series cards.

```python
reg add "HKLM\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties" /v MSISupported /t REG_DWORD /d 1 /f
```

###### restart

###### in device manager/view/resources by connection/GPU name should have a negative number in parentheses if MSIs is enabled

#### Disable HPET (High Precision event timer) in device manager/system devices and/or in your bios to get lower latency and more fps
