#### updated 7/31/2024 ✂️ 📋 :ramen: v1.100.19.2

##### for UE4 games for reference/customization/optimization/learning

##### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

##### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

##### 2560x1440 (~2k) use 58%(balance) 67%(quality) 70%(custom/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/TSR/CAS/FSR123/XeSS)

##### 3328x1872 (3.25K) use 50%(performance/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/TSR/CAS/FSR123/XeSS)

##### 3840x2160 (~4K UHD) use 33%(ultra performance) 50%(performance/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/TSR/CAS/FSR123/XeSS)

##### Recommended negative LOD bias -1/-0.6 or 0 for PERFORMANCE (set by nvidiaProfileInspector)

##### 77%(ultra quality) 87%(ultra plus) are good options for small performance boosts

##### [Installing and optimizing nvidia drivers here](https://github.com/smo0ths/Installing-and-optimizing-new-nvidia-drivers-on-windows-11-gaming-PC)

##### check 🟡 and set correctly according to recommendations

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

[/Script/Engine.Engine]
bPauseOnLossOfFocus=0;
bSmoothFrameRate=0;
bUseFixedFrameRate=0;

[TextureStreaming]
PoolSizeVRAMPercentage=50;---------------🔵 EDITED 🟣 texturepool cache

[ConsoleVariables]
sg.EffectsQuality=2;
sg.FoliageQuality=2;
sg.PostProcessQuality=2;
sg.ResolutionQuality=50;---------------🟡 set correctly
sg.ShadingQuality=2;---------------🟣 Shading
sg.ShadowQuality=2;
sg.TextureQuality=2;
sg.ViewDistanceQuality=2;
foliage.DensityScale=1;---------------🟢 0.6 for PERFORMANCE
foliage.DitheredLOD=1;---------------🟢 1 for PERFORMANCE
foliage.LODDistanceScale=1;
foliage.MinimumScreenSize=0.0001;---------------🔵 EDITED
grass.CullDistanceScale=1;
grass.DensityScale=0.6;---------------🟢 0.6 for PERFORMANCE 🔵 EDITED
grass.DisableDynamicShadows=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
grass.MaxAsyncTasks=4;
grass.MaxCreatePerFrame=1;
grass.MaxUpdateFrequency=1;---------------🔵 EDITED
grass.TickInterval=10;---------------🔵 EDITED
p.AnimDynamics=0;---------------🟢 0 for PERFORMANCE
p.AnimDynamicsWind=0;---------------🟢 0 for PERFORMANCE
p.ClothPhysics=1;
p.RigidBodyNode=0;---------------🟢 0 for PERFORMANCE
r.AllowGlobalClipPlane=0;---------------🟢 0 for PERFORMANCE
r.AllowLandscapeShadows=1;---------------🟢 0 for PERFORMANCE
r.AllowSimpleLights=1;---------------🟢 0 for PERFORMANCE
r.AmbientOcclusion.Method=0;---------------🟣 SSAO,GTAO
r.AmbientOcclusionLevels=2;---------------🟢 0,1 for PERFORMANCE
r.AmbientOcclusionMaxQuality=0;---------------🔵 EDITED
r.AmbientOcclusionMipLevelFactor=1;---------------🔵 EDITED
r.AmbientOcclusionRadiusScale=0.5;---------------🔵 EDITED
r.AmbientOcclusionStaticFraction=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.AnisotropicMaterials=1;---------------🟢 0 for PERFORMANCE
r.AOApplyToStaticIndirect=0;
r.AOGlobalDistanceField=0;---------------🟢 0 for PERFORMANCE 🟣 adaptive method
r.AOMaxViewDistance=10000;---------------🔵 EDITED
r.AOQuality=0;---------------🟢 0,1 for PERFORMANCE 🟣 req distancefieldao
r.Bloom.Cross=0.4;---------------🔵 EDITED
r.BloomQuality=4;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.CapsuleDirectShadows=0;
r.CapsuleIndirectShadows=0;
r.CapsuleShadows=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.CapsuleShadowsFullResolution=0;
r.chaos.ReflectionCaptureStaticSceneOnly=1;
r.ClearCoatNormal=1;---------------🟢 0 for PERFORMANCE
r.CompileShadersForDevelopment=1;---------------🟢 1 for PERFORMANCE
r.ContactShadows.NonShadowCastingIntensity=0;
r.ContactShadows=0;---------------🟢 0 for PERFORMANCE
r.D3D11.UseAllowTearing=1;---------------🟣 dxgi flip mode
r.D3D12.GPUCrashDebuggingMode=0;---------------🟣 debug
r.D3D12.UseAllowTearing=1;---------------🟣 dxgi flip mode
r.DefaultFeature.AmbientOcclusionStaticFraction=0;
r.DefaultFeature.AutoExposure.Method=1;---------------🟣 EyeAdaptation/AutoExposure
r.DefaultFeature.AutoExposure=1;---------------🟣 EyeAdaptation/AutoExposure 🟡 set correctly
r.DefaultFeature.MotionBlur=0;---------------🔵 EDITED
r.DepthOfFieldQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.DetailMode=1;---------------🟢 0,1 for PERFORMANCE
r.DFFullResolution=0;---------------🟢 0 for PERFORMANCE
r.DFShadowQuality=1;---------------🟢 0,1,2 for PERFORMANCE 🔵 EDITED 🟣 req distancefieldshadowing
r.DFShadowScatterTileCulling=1;---------------🟢 1 for PERFORMANCE
r.DistanceFieldAO=0;---------------🟢 0 for PERFORMANCE 🟣 req generatemeshdistancefields
r.DistanceFields.AtlasSizeXY=512;
r.DistanceFields.AtlasSizeZ=1024;
r.DistanceFields.ForceMaxAtlasSize=1;---------------🔵 EDITED
r.DistanceFields.MaxPerMeshResolution=128;
r.DistanceFields.ParallelAtlasUpdate=1;
r.DistanceFieldShadowing=1;---------------🟢 0 for PERFORMANCE 🟣 req generatemeshdistancefields
r.DOF.Gather.AccumulatorQuality=0;
r.DOF.Gather.EnableBokehSettings=0;
r.DOF.Gather.PostfilterMethod=1;---------------🔵 EDITED
r.DOF.Gather.RingCount=3;---------------🔵 EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;---------------🔵 EDITED
r.DOF.Kernel.MaxForegroundRadius=0.006;---------------🔵 EDITED
r.DOF.Recombine.Quality=0;
r.DOF.Scatter.BackgroundCompositing=0;---------------🔵 EDITED
r.DOF.Scatter.EnableBokehSettings=0;
r.DOF.Scatter.ForegroundCompositing=0;---------------🔵 EDITED
r.DOF.Scatter.MaxSpriteRatio=0.04;
r.DOF.TemporalAAQuality=0;
r.DynamicRes.OperationMode=0;
r.EmitterSpawnRateScale=0.5;---------------🟢 0.125,0.25 for PERFORMANCE
r.EnableCameraAndMeshMotionBlur=0;
r.EnableCameraAndMeshMotionBlur=0;
r.EyeAdaptation.Basic.Compute=1;---------------🟣 EyeAdaptation/AutoExposure
r.EyeAdaptation.MethodOverride=-1;---------------🟣 EyeAdaptation/AutoExposure
r.EyeAdaptation.PreExposureOverride=0;---------------🟣 EyeAdaptation/AutoExposure
r.EyeAdaptationQuality=1;---------------🟢 1 for PERFORMANCE 🟣 EyeAdaptation/AutoExposure
r.FilmGrain=0;
r.Filter.SizeScale=0.7;---------------🔵 EDITED
r.FinishCurrentFrame=0;
r.GenerateLandscapeGIData=0;---------------🟢 0 for PERFORMANCE 🟣 req generatemeshdistancefields
r.GenerateMeshDistanceFields=1;---------------🟢 0 for PERFORMANCE 🟣 dfs and dfao mesh
r.gpucrash.collectionenable=0;---------------🟣 debug
r.GPUCrashDebugging=0;---------------🟣 debug
r.GTSyncType=0;---------------🟣 Sync
r.HairStrands.Enable=0;---------------🟢 0 for PERFORMANCE
r.HeightfieldGlobalIllumination=0;---------------🟢 0 for PERFORMANCE
r.HeightFieldShadowing=0;---------------🟢 0 for PERFORMANCE
r.HFShadowQuality=0;---------------🟢 0,1 for PERFORMANCE 🟣 req heightfieldshadowing
r.HLOD.DistanceScale=0.8;
r.HLOD.ForceDisableCastDynamicShadow=0;---------------🟢 1 for PERFORMANCE
r.HZBOcclusion=0;
r.IrisNormal=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.LandscapeLODBias=0;---------------🟢 1 for PERFORMANCE
r.LensFlareQuality=0;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.LightFunctionQuality=1;---------------🟢 0,1 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;---------------🟢 0.6 for PERFORMANCE
r.LightShaftBlurPasses=2;---------------🔵 EDITED
r.LightShaftDownSampleFactor=2;
r.LightShaftFirstPassDistance=0.08;---------------🔵 EDITED
r.LightShaftQuality=1;---------------🟢 0 for PERFORMANCE
r.MaterialQualityLevel=1;---------------🟢 0,2 for PERFORMANCE
r.MaxAnisotropy=8;---------------🟢 0 for PERFORMANCE
r.MinRoughnessOverride=0;
r.MinScreenRadiusForLights=0.03;---------------🟢 0.04,0.06 for PERFORMANCE 🔵 EDITED
r.MipMapLODBias=0;
r.MotionBlurQuality=0;---------------🔵 EDITED
r.MSAACount=0;---------------🔵 EDITED
r.NGX.DLAA.Enable=0;---------------🟢 0 for PERFORMANCE
r.NGX.DLSS.AutoExposure=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED 🟣 EyeAdaptation/AutoExposure 🟡 set correctly
r.NGX.DLSS.DilateMotionVectors=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.NGX.DLSS.PreferNISSharpen=0;---------------🔵 EDITED
r.NGX.DLSS.Quality.Auto=0;---------------🟢 0 for PERFORMANCE
r.NGX.DLSS.Quality=-1;---------------🔵 EDITED 🟣 -2,-1,0,1,2 ultra perf,perf,balanced,quality,ultra quality 🟡 set correctly
r.NGX.DLSS.Reflections.TemporalAA=0;
r.NGX.DLSS.Sharpness=0;
r.NGX.DLSS.WaterReflections.TemporalAA=0;
r.NGX.LogLevel=0;---------------🟣 debug
r.OneFrameThreadLag=1;---------------🟢 1 for PERFORMANCE
r.ParallelShadow=1;---------------🟢 0 for PERFORMANCE
r.ParallelShadowsNonWholeScene=0;---------------🟢 0 for PERFORMANCE
r.ParallelTranslucency=1;
r.ParticleLightQuality=1;---------------🟢 0,1 for PERFORMANCE
r.ParticleLODBias=0;
r.ParticleMinTimeBetweenTicks=16;
r.PostProcessAAQuality=4;---------------🔵 EDITED 🟣 0 off 1,2 FXAA 3,4,5,6 TAA 🟡 set correctly
r.RefractionQuality=1;---------------🟢 0,1 for PERFORMANCE
r.RenderTargetPoolMin=300;---------------🟢 300 for PERFORMANCE 🔵 EDITED
r.SceneColorFormat=3;---------------🟢 2,3 for PERFORMANCE
r.SceneColorFringe.Max=0;---------------🔵 EDITED
r.SceneColorFringeQuality=1;
r.ScreenPercentage=50;---------------🟡 set correctly
r.SecondaryScreenPercentage.GameViewport=0;---------------🟢 83.33 for PERFORMANCE
r.ShaderDevelopmentMode=0;---------------🟣 debug
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;---------------🟢 0 for PERFORMANCE 🟣 movable light shadows
r.Shadow.CacheWholeSceneShadows=1;
r.Shadow.CacheWPOPrimitives=0;
r.Shadow.CSM.MaxCascades=2;---------------🟢 1,2 for PERFORMANCE 🔵 EDITED
r.Shadow.CSM.TransitionScale=1;
r.Shadow.DistanceScale=1;
r.Shadow.FarShadowDistanceOverride=0;
r.Shadow.FarShadowStaticMeshLODBias=0;
r.Shadow.FilterMethod=0;---------------🟢 0 for PERFORMANCE 🟣 PCSS shadows
r.Shadow.ForceSingleSampleShadowingFromStationary=1;
r.Shadow.MaxCSMResolution=2048;---------------🟢 512,1024 for PERFORMANCE 🔵 EDITED
r.Shadow.MaxNumFarShadowCascades=1;---------------🔵 EDITED
r.Shadow.MaxResolution=1024;---------------🟢 512,1024 for PERFORMANCE
r.Shadow.PreShadowResolutionFactor=0.5;
r.Shadow.RadiusThreshold=0.04;
r.ShadowQuality=3;---------------🟢 3 for PERFORMANCE 🔵 EDITED
r.SkeletalMeshLODBias=0;---------------🟢 1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=0.75;---------------🟢 0.5,0.75 for PERFORMANCE 🔵 EDITED
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1;
r.SkyAtmosphere.DistantSkyLightLUT=1;
r.SkyAtmosphere.FastSkyLUT=1;
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0;
r.SkyAtmosphere.SampleLightShadowmap=0;
r.SkyLight.RealTimeReflectionCapture=1;---------------🟢 0 for PERFORMANCE
r.SSGI.Enable=0;---------------🟢 0 for PERFORMANCE
r.SSGI.HalfRes=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.SSGI.LeakFreeReprojection=1;
r.SSGI.Quality=0;---------------🟢 0,2 for PERFORMANCE 🔵 EDITED 🟣 req ssgi enable
r.SSR.HalfResSceneColor=1;---------------🟢 1 for PERFORMANCE
r.SSR.MaxRoughness=-1;
r.SSR.Quality=2;---------------🟢 0 for PERFORMANCE
r.SSR.Temporal=0;---------------🔵 EDITED
r.SSS.Checkerboard=1;---------------🟢 1 for PERFORMANCE
r.SSS.HalfRes=1;
r.SSS.Quality=0;
r.SSS.SampleSet=0;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.SSS.Scale=1;
r.StaticMeshLODDistanceScale=1;---------------🟢 1 for PERFORMANCE
r.Streaming.AmortizeCPUToGPUCopy=0;
r.Streaming.Boost=1;
r.Streaming.EnableOptionalMips=0;
r.Streaming.FramesForFullUpdate=15;---------------🔵 EDITED
r.Streaming.HiddenPrimitiveScale=1;---------------🟢 0.5 for PERFORMANCE
r.Streaming.LimitPoolSizeToVRAM=0;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.MaxNumTexturesToStreamPerFrame=0;
r.Streaming.MipBias=0;---------------🟢 1 for PERFORMANCE
r.Streaming.PoolSize.Minimum=-1;
r.Streaming.PoolSize.MinimumFreeMemory=-1;
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.PoolSize=800;---------------🔵 EDITED
r.Streaming.PoolSizeForMeshes=-1;
r.Streaming.UseFixedPoolSize=0;
r.Streaming.UseMaterialData=1;
r.Streaming.UseNewMetrics=1;
r.SubsurfaceScattering=1;---------------🟢 0 for PERFORMANCE
r.SupportAnisotropicMaterials=1;---------------🟢 0 for PERFORMANCE
r.SupportMaterialLayers=1;---------------🟢 0 for PERFORMANCE
r.TemporalAA.Algorithm=0;---------------🟢 0 for PERFORMANCE 🟣 gen5 TAAU
r.TemporalAA.Upsampling=1;---------------🟣 TAAU 🟡 set correctly
r.TemporalAACurrentFrameWeight=0.03;
r.TemporalAAFilterSize=0.1;---------------🔵 EDITED 🟣 req gen5 TAAU
r.TemporalAASamples=8;
r.TessellationAdaptivePixelsPerTriangle=999999;---------------🟢 999999 for PERFORMANCE 🔵 EDITED
r.TiledDeferredShading=1;---------------🟢 0 for PERFORMANCE 🔵 gpu lights
r.Tonemapper.GrainQuantization=1;
r.Tonemapper.MergeWithUpscale.Mode=1;
r.Tonemapper.Quality=2;
r.ToneMapper.Sharpen=0;---------------🟡 set correctly
r.TranslucencyLightingVolumeDim=32;---------------🟢 32 for PERFORMANCE 🔵 EDITED
r.TranslucencyVolumeBlur=1;---------------🟢 0 for PERFORMANCE
r.UniformBufferPooling=1;---------------🟣 debug
r.Upscale.Quality=1;---------------🔵 EDITED
r.UsePreExposure=1;---------------🟣 EyeAdaptation/AutoExposure
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;---------------🟢 0 for PERFORMANCE
r.ViewDistanceScale=1;---------------🟢 0.8 for PERFORMANCE
r.VolumetricCloud.DisableCompute=0;
r.VolumetricCloud.EnableAerialPerspectiveSampling=1;
r.VolumetricCloud.EnableAtmosphericLightsSampling=1;
r.VolumetricCloud.EnableDistantSkyLightSampling=1;
r.VolumetricCloud.EnableLocalLightsSampling=0;
r.VolumetricCloud.HighQualityAerialPerspective=0;
r.VolumetricCloud.Shadow.SampleAtmosphericLightShadowmap=0;
r.VolumetricCloud.ShadowMap=0;
r.VolumetricCloud.SkyAO=0;
r.VolumetricFog.GridPixelSize=16;---------------🔵 EDITED
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.HistoryMissSupersampleCount=1;---------------🔵 EDITED
r.VolumetricFog.HistoryWeight=0.95;---------------🔵 EDITED
r.VolumetricFog.InverseSquaredLightDistanceBiasScale=1;
r.VolumetricFog.Jitter=1;
r.VolumetricFog.TemporalReprojection=1;
r.VolumetricFog=0;---------------🟢 0 for PERFORMANCE
r.VSync=0;---------------🟣 Sync
r.VT.MaxAnisotropy=4;
r.Water.EnableShallowWaterSimulation=0;---------------🟢 0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.DepthPrepass=0;
r.Water.SingleLayer.Reflection=1;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.RefractionDownsampleFactor=2;
r.Water.SingleLayer.ShadersSupportDistanceFieldShadow=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.SSRTAA=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.TiledComposite=1;
r.Water.SingleLayer.UnderwaterFog=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.UnderwaterFogWhenCameraIsAboveWater=0;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayerWater.SupportCloudShadow=0;---------------🟢 0 for PERFORMANCE
r.Water.WaterMesh.LODCountBias=0;
r.Water.WaterMesh.LODMorphEnabled=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.Water.WaterMesh.LODScaleBias=-0.5;---------------🟢 -0.5 for PERFORMANCE 🔵 EDITED
r.Water.WaterMesh.TessFactorBias=-1;---------------🟢 -1 for PERFORMANCE 🔵 EDITED
rhi.SyncInterval=0;---------------🟣 Sync
rhi.SyncSlackMS=0;---------------🟣 Sync
t.OverrideFPS=0;
t.Streamline.Reflex.Enable=1;---------------🟣 nvidia reflex
t.Streamline.Reflex.Mode=2;---------------🟣 reflex on with boost
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
bEnableMouseSmoothing=0;
bF11TogglesFullscreen=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.1;---------------🔵 EDITED
ButtonRepeatDelay=0.1;
DoubleClickTime=0.01;---------------🔵 EDITED
```

---

#### Ultra config

```python
Use these when game is using DLSS
r.DefaultFeature.AutoExposure=0;---------------🔵 EDITED 🟣 EyeAdaptation/AutoExposure 🟡 set correctly
r.NGX.DLSS.AutoExposure=1;---------------🟢 0 for PERFORMANCE 🟣 EyeAdaptation/AutoExposure 🟡 set correctly

turn this off when using other sharpening methods
r.ToneMapper.Sharpen=1;---------------🔵 EDITED 🟡 set correctly
```

```python
[Core.Log]
Global=off;

[/Script/Engine.Engine]
bPauseOnLossOfFocus=0;
bSmoothFrameRate=0;
bUseFixedFrameRate=0;

[ConsoleVariables]
sg.EffectsQuality=3;
sg.FoliageQuality=3;
sg.PostProcessQuality=3;
sg.ResolutionQuality=100;---------------🟡 set correctly
sg.ShadingQuality=3;---------------🟣 Shading
sg.ShadowQuality=3;
sg.TextureQuality=3;
sg.ViewDistanceQuality=3;
r.AmbientOcclusion.Method=0;---------------🟣 SSAO,GTAO
r.AmbientOcclusionLevels=2;---------------🟢 0,1 for PERFORMANCE
r.AmbientOcclusionMaxQuality=100;---------------🔵 EDITED
r.AmbientOcclusionMipLevelFactor=0;---------------🔵 EDITED
r.AmbientOcclusionRadiusScale=1;---------------🔵 EDITED
r.AmbientOcclusionStaticFraction=1;---------------🟢 0 for PERFORMANCE
r.AOQuality=2;---------------🟢 0,1 for PERFORMANCE 🟣 req distancefieldao
r.CompileShadersForDevelopment=1;---------------🟢 1 for PERFORMANCE
r.D3D11.UseAllowTearing=1;---------------🟣 dxgi flip mode
r.D3D12.GPUCrashDebuggingMode=0;---------------🟣 debug
r.D3D12.UseAllowTearing=1;---------------🟣 dxgi flip mode
r.DefaultFeature.AmbientOcclusionStaticFraction=1;
r.DefaultFeature.AutoExposure=1;---------------🟣 EyeAdaptation/AutoExposure 🟡 set correctly
r.DefaultFeature.MotionBlur=0;---------------🔵 EDITED
r.DepthOfFieldQuality=0;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.DistanceFieldAO=1;---------------🟢 0 for PERFORMANCE 🟣 req generatemeshdistancefields
r.DynamicRes.OperationMode=0;
r.EnableCameraAndMeshMotionBlur=0;
r.FilmGrain=0;
r.FinishCurrentFrame=0;
r.gpucrash.collectionenable=0;---------------🟣 debug
r.GPUCrashDebugging=0;---------------🟣 debug
r.GTSyncType=0;---------------🟣 Sync
r.HZBOcclusion=0;
r.IrisNormal=1;---------------🟢 0 for PERFORMANCE
r.LensFlareQuality=3;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.MinRoughnessOverride=0;
r.MotionBlurQuality=0;---------------🔵 EDITED
r.MSAACount=0;---------------🔵 EDITED
r.NGX.DLAA.Enable=0;---------------🟢 0 for PERFORMANCE
r.NGX.DLSS.AutoExposure=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED 🟣 EyeAdaptation/AutoExposure 🟡 set correctly
r.NGX.DLSS.DilateMotionVectors=1;---------------🟢 0 for PERFORMANCE
r.NGX.DLSS.PreferNISSharpen=0;---------------🔵 EDITED
r.NGX.DLSS.Quality.Auto=0;---------------🟢 0 for PERFORMANCE
r.NGX.DLSS.Quality=1;---------------🔵 EDITED 🟣 -2,-1,0,1,2 ultra perf,perf,balanced,quality,ultra quality 🟡 set correctly
r.NGX.DLSS.Reflections.TemporalAA=0;
r.NGX.DLSS.Sharpness=0;
r.NGX.DLSS.WaterReflections.TemporalAA=0;
r.NGX.LogLevel=0;---------------🟣 debug
r.OneFrameThreadLag=1;---------------🟢 1 for PERFORMANCE
r.PostProcessAAQuality=6;---------------🔵 EDITED 🟣 0 off 1,2 FXAA 3,4,5,6 TAA 🟡 set correctly
r.RenderTargetPoolMin=1000;---------------🟢 300 for PERFORMANCE 🔵 EDITED
r.SceneColorFringe.Max=0;---------------🔵 EDITED
r.SceneColorFringeQuality=1;
r.ScreenPercentage=100;---------------🟡 set correctly
r.SecondaryScreenPercentage.GameViewport=0;---------------🟢 83.33 for PERFORMANCE
r.ShaderDevelopmentMode=0;---------------🟣 debug
r.Shadow.CSM.MaxCascades=4;---------------🟢 1,2 for PERFORMANCE 🔵 EDITED
r.Shadow.MaxCSMResolution=2048;---------------🟢 512,1024 for PERFORMANCE 🔵 EDITED
r.Shadow.MaxResolution=2048;---------------🟢 512,1024 for PERFORMANCE 🔵 EDITED
r.SSR.HalfResSceneColor=0;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.SSR.MaxRoughness=-1;
r.SSR.Quality=3;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.SSR.Temporal=1;
r.Streaming.PoolSize=6000;---------------🔵 EDITED
r.TemporalAA.Algorithm=0;---------------🟢 0 for PERFORMANCE 🟣 gen5 TAAU
r.TemporalAA.Upsampling=0;---------------🟣 TAAU 🟡 set correctly
r.TemporalAACurrentFrameWeight=0.03;
r.TemporalAAFilterSize=0.1;---------------🔵 EDITED 🟣 req gen5 TAAU
r.TemporalAASamples=8;
r.Tonemapper.MergeWithUpscale.Mode=1;
r.Tonemapper.Quality=2;
r.ToneMapper.Sharpen=1;---------------🔵 EDITED 🟡 set correctly
r.UniformBufferPooling=1;---------------🟣 debug
r.Upscale.Quality=3;---------------🔵 EDITED
r.VSync=0;---------------🟣 Sync
rhi.SyncInterval=0;---------------🟣 Sync
rhi.SyncSlackMS=0;---------------🟣 Sync
t.OverrideFPS=0;
t.Streamline.Reflex.Enable=1;---------------🟣 nvidia reflex
t.Streamline.Reflex.Mode=2;---------------🟣 reflex on with boost
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
