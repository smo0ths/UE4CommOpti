#### updated 12/23/2023 :ramen: :ramen: :ramen:

##### for UE4 games for reference/customization/optimization/learning

##### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

##### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

##### def is reference to high scalablity group

##### 2k scaling (DLSS123/TAAU/CAS/FSR123/XeSS) 58%/67% or 70% resolution scale (balance/quality) -1/-0.5 (0/1 for PERFORMANCE) (recommended negative LOD bias)

##### 4k scaling (DLSS123/TAAU/CAS/FSR123/XeSS) 33%/50% resolution scale (ultra performance/performance) -2/-1.5 (-1/0 for PERFORMANCE) (recommended negative LOD bias)

##### make sure your scaling % is set correctly! and match PIP(scope) resolution scaling in games (manually in graphic settings) for best fps

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
MaxChannels=128;
CommonAudioPoolSize=0;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=70;----------⚫️DEF 70 🟢texturepool cache

[ConsoleVariables]
sg.ResolutionQuality=50;----------🟡set correctly
sg.ViewDistanceQuality=2;
sg.AntiAliasingQuality=2;
sg.ShadowQuality=2;
sg.PostProcessQuality=2;
sg.TextureQuality=2;
sg.EffectsQuality=2;
sg.FoliageQuality=2;
sg.ShadingQuality=2;
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
```

---

<details><summary>Now the fun part open up Scalability.ini and add the config to the scalability groups eg [EffectsQuality@2] i'm not going threw all the commands and putting them perfectly into place this is the brute force method :D</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Scalability.ini
</p>
</details>

```python
[AntiAliasingQuality@2]
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1

[ViewDistanceQuality@2]
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1

[ShadowQuality@2]
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1

[PostProcessQuality@2]
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1

[TextureQuality@2]
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1

[EffectsQuality@2]
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1

[FoliageQuality@2]
ShowFlag.Grain=0;----------🔵
ShowFlag.Tessellation=0;----------🔵
ShowFlag.Vignette=0;----------🔵
r.SupportAnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=0;----------⚫️DEF ❓
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
p.BatchPhysXTasksSize=3;----------⚫️DEF 3 🔵
p.AnimDynamics=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.SkipSkeletalRepOptimization=1;----------⚫️DEF 1
p.SkipUpdateOverlapsOptimEnabled=1;----------⚫️DEF 1
p.RigidBodyNode=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5;----------⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1;----------⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0;----------⚫️DEF 0
t.ApplicationFPSCap=0;----------⚫️DEF ❓
t.MaxFPS=0;----------⚫️DEF ❓
fx.FXAllowParticleMeshLODs=0;----------⚫️DEF 0
fx.MaxCPUParticlesPerEmitter=10;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=10486;----------⚫️DEF 1048576 ⚪️EDITED 🔵
fx.ParticleManagerAsyncBatchSize=8;----------⚫️DEF 8
fx.ParticleSystemPool.Enable=1;----------⚫️DEF 1
fx.QualityLevelSpawnRateScaleReferenceLevel=2;----------⚫️DEF 2 🔵
au.RenderThreadPriority=0;----------⚫️DEF 3 🔵
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.DBuffer=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0;----------⚫️DEF 4 ⚪️EDITED
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EarlyZPass=2;----------⚫️DEF ❓
r.EarlyZPassMovable=1;----------⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.HZBOcclusion=0;----------⚫️DEF ❓ 🔵
r.MinTimeBetweenTicks=8;----------⚫️DEF 8 or 16 ⚪️EDITED 🔵
r.SceneColorFormat=3;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.VSync=0;----------⚫️DEF 0
r.RenderTargetPoolMin=200;----------⚫️DEF ❓ 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.ScreenPercentage=50;----------🟡set correctly
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.05;----------⚫️DEF 0.05
r.TemporalAASamples=8;----------⚫️DEF 8
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.ParticleLightQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.Filter.SizeScale=0.8;----------⚫️DEF 0.8
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🔵
r.MaxAnisotropy=8;----------⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=0;----------⚫️DEF 0
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5;----------⚫️DEF 5 🟢0 for PERFORMANCE
r.DistanceFields.ForceMaxAtlasSize=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.DistanceFields.RuntimeDownsamplingFactor=0.5;----------⚫️DEF 0 ⚪️EDITED 🔵
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;------def 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.DistanceScale=0.85;----------⚫️DEF 0.85
r.Shadow.CSM.MaxCascades=3;----------⚫️DEF 3 🟢2 for PERFORMANCE
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024;----------⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.08;----------⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=0;----------⚫️DEF 0 🔵
r.SSR.MaxRoughness=0.6;----------⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1;----------⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Burley.Quality=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=0;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.04;----------⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.NormalMapsForStaticLighting=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0;----------⚫️DEF 0
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionLevels=1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusion.Compute=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=2;----------⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1;----------⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;----------⚫️DEF 0 🔵
r.Streaming.PoolSize=1600;----------⚫️DEF 2000 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0
r.Streaming.MaxHiddenPrimitiveViewBoost=1.5;----------⚫️DEF 1.5 🔵
r.Streaming.MaxReferenceChecksBeforeStreamOut=2;----------⚫️DEF 2 🔵
r.Streaming.MaxTempMemoryAllowed=50;----------⚫️DEF 50 🔵
r.Streaming.MaxTextureUVDensity=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF 100 🔵
r.Streaming.MinMipForSplitRequest=10;----------⚫️DEF 10 🔵
r.Streaming.MipCalculationEnablePerLevelList=1;----------⚫️DEF 1 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.UITextureLODBias=0;----------⚫️DEF 0
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;----------⚫️DEF 1
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
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
bDepthOfField=?;
bMotionBlur=?;
bBounceLightEnabled=?;
bFlashlightShadowsEnabled=?;
AmbientOcclusion=(Value=?);
AntiAliasingMode=(Value=?);
AudioQualityLevel=?;
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
FoliageMinLOD=(Value=?);
FullscreenMode=?;
Gamma=?;
GlobalSensitivity=?;
GraphicsQuality=?;
GraphicsPresetIndex=?;
HDRDisplayOutputNits=?;
HZBOcclusion=(Value=?);
MaxAnisotropy=(Value=?);
MaxAnisotropy=?;
bFrameLimitEnabled=?;
FrameRateLimit=?;
MaxFPS=?;
MenuFrameRateLimit=?;
OceanQuality=(Value=?);
OverrideOptions=(("r.command",(Value=?,bModified=True)),("r.command",(Value=?,bModified=True)));
PostFX_Saturation=?;
PostFX_Sharpness=?;
ResolutionScaleModifier=?;
ScreenPercentage=(Value=?);
SkeletalMeshLODBias=(Value=?);
Tessellation=(Value=?);
TessellationMode=(Value=?);
TextureStreamPoolSizeStorage=(Value=?);
TAASampleStorage=?;
WakeSim=(Value=?)
LastSavedAAQuality=?;
LastSavedAASamples=?;
ScreenPercentage=(Value=50);----------🟡set correctly
TemporalAASamples=(Value=2);----------🔵force 2 or any value you want
DoubleKeyPressTime=0.01;

use these so my settings are actually being used:
[ScalabilityGroups]
sg.ResolutionQuality=50;----------🟡set correctly
sg.ViewDistanceQuality=2;
sg.AntiAliasingQuality=2;
sg.ShadowQuality=2;
sg.PostProcessQuality=2;
sg.TextureQuality=2;
sg.EffectsQuality=2;
sg.FoliageQuality=2;
sg.ShadingQuality=2;

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
InitialButtonRepeatDelay=0.2;----------⚫️DEF 0.2
ButtonRepeatDelay=0.1;----------⚫️DEF 0.1
DoubleClickTime=0.01;----------⚫️DEF 0.25 ⚪️EDITED
```

---

<details><summary>Open DeviceProfiles.ini for textures lods, should lower gpu utilization, most MaxLODSize in games are 4096. Feel free to just skip this and use devs defaults</summary>
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
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Cinematic,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=128,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=128,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=256,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_NoMipmaps,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=512,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_MobileFlattened,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_Face,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_LightMap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=512,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ColorLookupTable,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Bokeh,MinLODSize=1,MaxLODSize=1024,MaxLODSize=256,LODBias=0,MinMagFilter=linear,MipFilter=linear,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_IESLightProfile,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=point,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_HierarchicalLOD,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Impostor,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ImpostorNormalDepth,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_8BitData,LODBias=0,MinMagFilter=point,MipFilter=linear,MipGenSettings=TMGS_NoMipmaps)
TextureLODGroups=(Group=TEXTUREGROUP_16BitData,LODBias=0,MinMagFilter=point,MipFilter=linear,MipGenSettings=TMGS_NoMipmaps)
TextureLODGroups=(Group=TEXTUREGROUP_Project01,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project02,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project03,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project04,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project05,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project06,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project07,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project08,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project09,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project10,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project11,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project12,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project13,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project14,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project15,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_MAX,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
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

###### win + r type cmd then press control+shift+enter (starts as admin) then add key. NVcleaninstall gives you more MSIs options. Newest drivers auto do this on 40 series cards, i wonder if its default or set to high.

```python
reg add "HKLM\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties" /v MSISupported /t REG_DWORD /d 1 /f
```

###### restart

###### in device manager/view/resources by connection/GPU name should have a negative number in parentheses if MSIs is enabled

#### Disable HPET (High Precision event timer) in device manager/system devices and/or in your bios to get lower latency and more fps
