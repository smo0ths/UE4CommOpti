#### updated 12/30/2023 ✂️ 📋 :ramen:

##### for UE4 games for reference/customization/optimization/learning

##### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

##### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

##### ⚫️DEF is reference to high scalablity group

##### 2k scaling (DLSS123/TAAU/CAS/FSR123/XeSS) (58% scaling -1/0 NegativeMipMapLODbias, best for PERFORMANCE) (67% scaling -0.5/0 NegativeMipMapLODbias) (70% scaling 0 NegativeMipMapLODbias, best for cheap scalers like TAAU)

##### 4k scaling (DLSS123/TAAU/CAS/FSR123/XeSS) (33% scaling -2/0 NegativeMipMapLODbias, best for PERFORMANCE) (50% scaling -1.5/0 NegativeMipMapLODbias, best for cheap scalers like TAAU)

##### NegativeMipMapLODbias costs PERFORMANCE but helps upscaling quality*

##### make sure your scaling % is set correctly! and match PIP(scope) resolution scaling in games (manually in graphic settings) for PERFORMANCE

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
MaxChannels=32;----------⚫️DEF ❓ 🔵
CommonAudioPoolSize=0;----------⚫️DEF 0 🔵

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=50;----------⚫️DEF 70 🟢texturepool cache ⚪️EDITED 🔵

[ConsoleVariables]
sg.ResolutionQuality=50;----------🟡set correctly
sg.ViewDistanceQuality=2;
sg.AntiAliasingQuality=2;
sg.ShadowQuality=2;
sg.PostProcessQuality=2;
sg.TextureQuality=2;
sg.EffectsQuality=2;
sg.FoliageQuality=2;
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0
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
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0

[ViewDistanceQuality@2]
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0

[ShadowQuality@2]
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0

[PostProcessQuality@2]
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0

[TextureQuality@2]
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0

[EffectsQuality@2]
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0

[FoliageQuality@2]
r.SupportAnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.SupportAtmosphericFog=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SupportSkyAtmosphere=1;----------⚫️DEF ❓
r.SupportSkyAtmosphereAffectsHeightFog=1;----------⚫️DEF 1
r.SupportPointLightWholeSceneShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
p.AnimDynamics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.RigidBodyNode=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
p.ClothPhysics=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1;----------⚫️DEF 0 🟢1 for PERFORMANCE 🔵
r.IndirectLightingCache=0;----------⚫️DEF ❓
r.DoInitViewsLightingAfterPrepass=0;----------⚫️DEF 0 🔵experimental
r.DoLazyStaticMeshUpdate=0;----------⚫️DEF 0 🔵experimental
r.CompileShadersForDevelopment=0;----------⚫️DEF 1 ⚪️EDITED
r.D3D12.GPUCrashDebuggingMode=0;----------⚫️DEF ❓
r.AllowOcclusionQueries=1;----------⚫️DEF ❓
r.NumBufferedOcclusionQueries=2;----------⚫️DEF ❓ 🔵
r.UseCachedLODSceneTreeVisibilityStates=1;----------⚫️DEF ❓
r.UseParallelLightVisibilityUpdates=1;----------⚫️DEF ❓ 🔵
r.UniformBufferPooling=0;----------⚫️DEF ❓
r.ShaderPipelineCache.Enabled=1;----------⚫️DEF ❓
r.FinishCurrentFrame=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.CreateShadersOnLoad=1;----------⚫️DEF ❓ 🔵
r.GPUCrashDebugging=0;----------⚫️DEF ❓
r.gpucrash.collectionenable=0;----------⚫️DEF 1 ⚪️EDITED
r.GBufferFormat=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.ClearSceneMethod=1;----------⚫️DEF 1
r.UseClusteredDeferredShading=0;----------⚫️DEF 0
r.TiledDeferredShading=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.TiledDeferredShading.MinimumCount=1;----------⚫️DEF 80 ⚪️EDITED 🔵
r.HZBOcclusion=1;----------⚫️DEF ❓ 🔵
r.DBuffer=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.DefaultBackBufferPixelFormat=4;----------⚫️DEF 4 🟢0 for PERFORMANCE 🔵
r.SceneColorFormat=4;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.VSync=0;----------⚫️DEF 0
rhi.SyncInterval=0;----------⚫️DEF 1 ⚪️EDITED
r.GTSyncType=0;----------⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethodForceOverride=0;----------⚫️DEF 0 🔵
r.SceneRenderTargetResizeMethod=0;----------⚫️DEF 0 🔵
r.DynamicRes.OperationMode=0;----------⚫️DEF 0
r.DynamicRes.MaxScreenPercentage=67;----------⚫️DEF ❓ 🔵req DynamicRes
r.DynamicRes.FrameTimeBudget=10;----------⚫️DEF ❓ 🔵req DynamicRes
r.SecondaryScreenPercentage.GameViewport=0;----------⚫️DEF 0
r.ScreenPercentage=50;----------🟡set correctly
r.Upscale.Quality=1;----------⚫️DEF ❓ 🟢0 or 1 for PERFORMANCE 🔵
r.Tonemapper.MergeWithUpscale.Mode=1;----------⚫️DEF 1 🔵
r.PostProcessAAQuality=5;----------🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.TemporalAA.Algorithm=0;----------⚫️DEF 0 🟢0 for PERFORMANCE 🔵gen5 TAA
r.TemporalAAFilterSize=0.1;----------⚫️DEF 1 ⚪️EDITED 🔵only works for gen5 TAA
r.TemporalAA.Upsampling=1;----------⚫️DEF 0 🔵for ScreenPercentage ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03;----------⚫️DEF 0.03 ⚪️EDITED 🔵
r.TemporalAASamples=2;----------⚫️DEF 8 ⚪️EDITED 🔵
foliage.DensityScale=0.6;----------⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1;----------⚫️DEF 1
foliage.LODDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
foliage.MinLOD=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinimumScreenSize=5e-5;----------⚫️DEF 1e-4 🟢1e-3 or 5e-5 for PERFORMANCE ⚪️EDITED 🔵
foliage.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
grass.DensityScale=0.6;----------⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10;----------⚫️DEF 30 🟢10 for PERFORMANCE ⚪️EDITED
grass.TickInterval=10;----------⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.Water.EnableShallowWaterSimulation=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableUnderwaterPostProcess=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale=1;----------⚫️DEF 1 🟢0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.AllowSimpleLights=1;----------⚫️DEF 1
r.ParticleLightQuality=2;----------⚫️DEF 1 🟢0 or 1 for PERFORMANCE ⚪️EDITED 🔵
r.EmitterSpawnRateScale=1;----------⚫️DEF 1 🟢0.125 or 0.5 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;----------⚫️DEF 1000 ⚪️EDITED 🔵
fx.MaxGPUParticlesSpawnedPerFrame=1000;----------⚫️DEF 1048576 ⚪️EDITED 🔵
r.ParticleMinTimeBetweenTicks=16;----------⚫️DEF ❓
r.MinTimeBetweenTicks=16;----------⚫️DEF ❓
r.AnisotropicMaterials=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.Filter.SizeScale=0.7;----------⚫️DEF 0.8 ⚪️EDITED
r.Bloom.Cross=0;----------⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4;----------⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0;----------⚫️DEF 3 ⚪️EDITED
r.DetailMode=2;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE 🔵
r.RefractionQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0;----------⚫️DEF 1 ⚪️EDITED
r.LensFlareQuality=1;----------⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.MaxAnisotropy=16;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999;----------⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MaterialQualityLevel=1;----------⚫️DEF 1 🟢0 or 2 for PERFORMANCE 🔵
r.ClearCoatNormal=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.NormalMapsForStaticLighting=0;----------⚫️DEF ❓ 🔵
Compat.UseDXT5NormalMaps=0;----------⚫️DEF 0
r.Tonemapper.Quality=1;----------⚫️DEF 5 ⚪️EDITED
r.TonemapperFilm=0;----------⚫️DEF 0
r.TonemapperGamma=2.2;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Tonemapper.Sharpen=0;----------⚫️DEF 2 ⚪️EDITED 🔵
r.Tonemapper.GrainQuantization=1;----------⚫️DEF 1
r.SubsurfaceScattering=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Quality=0;----------⚫️DEF 0
r.SSS.SampleSet=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=2;----------⚫️DEF 2 🟢1 for PERFORMANCE
r.SSS.HalfRes=1;----------⚫️DEF 1
r.SSS.Scale=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SSR.MaxRoughness=-1;----------⚫️DEF -1 🔵
r.SSR.Quality=2;----------⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0;----------⚫️DEF 0
r.HairStrands.Interpolation.UseSingleGuide=1;----------⚫️DEF 1
r.HairStrands.SkyAO.SampleCount=4;----------⚫️DEF 4
r.HairStrands.SkyLighting.IntegrationType=2;----------⚫️DEF 2
r.HairStrands.SkyLighting=1;----------⚫️DEF 1
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.MethodOverride=-2;----------⚫️DEF -1 ⚪️EDITED 🔵
r.EyeAdaptationQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.EyeAdaptation.Basic.Compute=1;----------⚫️DEF 1
r.UsePreExposure=1;----------⚫️DEF 1
r.EyeAdaptation.PreExposureOverride=0;----------⚫️DEF 0
r.DefaultFeature.AutoExposure.Bias=1;----------⚫️DEF 1
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1;----------⚫️DEF ❓ 🔵
r.DefaultFeature.AutoExposure.Method=1;----------⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🔵Basic AutoExposure
r.DepthOfFieldQuality=1;----------⚫️DEF 2 🟢0 or 1 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Gather.AccumulatorQuality=0;----------⚫️DEF 0
r.DOF.Gather.PostfilterMethod=2;----------⚫️DEF 2
r.DOF.Gather.EnableBokehSettings=0;----------⚫️DEF 0
r.DOF.Gather.RingCount=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.ForegroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Scatter.BackgroundCompositing=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.Recombine.Quality=0;----------⚫️DEF 0
r.DOF.Kernel.MaxForegroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;----------⚫️DEF 0.012 🟢0.006 for PERFORMANCE ⚪️EDITED
r.GenerateMeshDistanceFields=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req for DF things
r.DistanceFieldShadowing=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DFShadowQuality=2;----------⚫️DEF 3 🟢1 or 2 for PERFORMANCE 🔵req DistanceFieldShadowing
r.DFDistanceScale=0.4;----------⚫️DEF 1 ⚪️EDITED
r.DFFullResolution=0;----------⚫️DEF 0
r.DFTwoSidedMeshDistanceBias=10;----------⚫️DEF 5 ⚪️EDITED
r.HeightfieldGlobalIllumination=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HeightFieldShadowing=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.HFShadowQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req HeightFieldShadowing
r.CapsuleShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows.NonShadowCastingIntensity=0;----------⚫️DEF 0
r.AllowLandscapeShadows=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵
r.ShadowQuality=3;----------⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.FilterMethod=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵PCSS shadows
r.Shadow.DistanceScale=0.7;----------⚫️DEF 0.85 ⚪️EDITED
r.Shadow.CSM.MaxCascades=4;----------⚫️DEF 3 🟢2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSMSlopeScaleDepthBias=1;----------⚫️DEF 3 ⚪️EDITED
r.Shadow.CSM.TransitionScale=2;----------⚫️DEF 0.8 ⚪️EDITED
r.Shadow.MaxCSMResolution=2048;----------⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;----------⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03;----------⚫️DEF 0.04 🟢0.06 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req some light shadows ⚪️EDITED
r.Shadow.CacheWholeSceneShadows=1;----------⚫️DEF 1
r.Shadow.WholeSceneShadowCacheMb=750;----------⚫️DEF ❓ 🔵
r.Shadow.FadeExponent=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.Shadow.UnbuiltPreviewInGame=0;----------⚫️DEF ❓
r.VolumetricFog=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;----------⚫️DEF 16 🟢16 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridSizeZ=64;----------⚫️DEF 64
r.VolumetricFog.HistoryMissSupersampleCount=1;----------⚫️DEF 4 🟢1 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.VolumetricFog.TemporalReprojection=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricCloud=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0;----------⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucentLightingVolume=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;----------⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowDownsampledStandardTranslucency=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.SeparateTranslucency=1;----------⚫️DEF 1 🔵
r.LightFunctionQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;----------⚫️DEF 1 🟢0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.02;----------⚫️DEF 0.03 🟢0.04 or 0.06 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftNumSamples=12;----------⚫️DEF ❓
r.LightShaftFirstPassDistance=0.1;----------⚫️DEF 0.1
r.LightShaftDownSampleFactor=2;----------⚫️DEF 2
r.LightShaftBlurPasses=3;----------⚫️DEF ❓
r.LightShaftAllowTAA=1;----------⚫️DEF 1
r.HighQualityLightMaps=1;----------⚫️DEF ❓
r.DoTiledReflections=1;----------⚫️DEF 1 🟢0 for PERFORMANCE 🔵
r.SkyLight.RealTimeReflectionCapture=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1;----------⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;----------⚫️DEF 1
r.GenerateLandscapeGIData=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE 🔵req GenerateMeshDistanceFields
r.DistanceFieldGI=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.SSGI.Enable=0;----------⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=0;----------⚫️DEF 2 ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1;----------⚫️DEF 0.6 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=-25;----------⚫️DEF 100 ⚪️EDITED
r.AmbientOcclusionLevels=-1;----------⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=1;----------⚫️DEF 1
r.AmbientOcclusionStaticFraction=-1;----------⚫️DEF -1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;----------⚫️DEF 0 🔵WIP
r.DistanceFieldAO=0;----------⚫️DEF ❓ 🟢0 for PERFORMANCE
r.AOQuality=2;----------⚫️DEF 2 🟢1 for PERFORMANCE 🔵req DistanceFieldAO
r.AOHeightfieldOcclusion=0;----------⚫️DEF ❓
D3D12.AdjustTexturePoolSizeBasedOnBudget=1;----------⚫️DEF ❓ 🔵
D3D12.DynamicTexturePoolSize=0;----------⚫️DEF ❓
D3D12.TexturePoolOnlyAccountStreamableTexture=1;----------⚫️DEF ❓
D3D12.UseUpdateTexture3DComputeShader=0;----------⚫️DEF 0
D3D12.ZeroBufferSizeInMB=4;----------⚫️DEF 4
r.MeshStreaming=1;----------⚫️DEF ❓ 🔵experimental
r.TextureStreaming=1;----------⚫️DEF 1
r.Streaming.Boost=1;----------⚫️DEF 1
r.Streaming.LimitPoolSizeToVRAM=0;----------⚫️DEF 1 ⚪️EDITED 🔵
r.Streaming.HiddenPrimitiveScale=1;----------⚫️DEF ❓
r.Streaming.FramesForFullUpdate=10;----------⚫️DEF ❓
r.Streaming.PrioritizeMeshLODRetention=1;----------⚫️DEF ❓
r.Streaming.MipBias=0;----------⚫️DEF 0
r.Streaming.PoolSize=3000;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.PoolSizeForMeshes=-1;----------⚫️DEF -1 ⚪️EDITED 🔵
r.Streaming.AmortizeCPUToGPUCopy=1;----------⚫️DEF 0 ⚪️EDITED 🔵
r.Streaming.MaxNumTexturesToStreamPerFrame=1;----------⚫️DEF 0 ⚪️EDITED 🔵req AmortizeCPUToGPUCopy
r.Streaming.FullyLoadUsedTextures=0;----------⚫️DEF 0
r.Streaming.DefragDynamicBounds=1;----------⚫️DEF ❓ 🔵
r.Streaming.MaxEffectiveScreenSize=0;----------⚫️DEF 0 🔵
r.Streaming.MinLevelRenderAssetScreenSize=100;----------⚫️DEF ❓ 🔵
r.Streaming.MaxTempMemoryAllowed=1500;----------⚫️DEF ❓ 🔵
r.RenderTargetPoolMin=750;----------⚫️DEF ❓ 🔵
r.DisableLODFade=0;----------⚫️DEF 0
r.LODFadeTime=1;----------⚫️DEF 0.25 ⚪️EDITED 🔵
r.SkeletalMeshLODRadiusScale=0.25;----------⚫️DEF 1 🟢1 for PERFORMANCE ⚪️EDITED 🔵
r.StaticMeshLODDistanceScale=1;----------⚫️DEF 1
r.LandscapeLODDistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLOD0DistributionScale=1;----------⚫️DEF 1 🔵
r.LandscapeLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.MipMapLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0;----------⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0;----------⚫️DEF 0
r.UITextureLODBias=0;----------⚫️DEF 0
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
TextureLODGroups=(Group=TEXTUREGROUP_World,                 MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,        MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,         MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Character,             MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,    MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,     MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,                MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,       MinLODSize=128,  MaxLODSize=512,  OptionalMaxLODSize=256,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,        MinLODSize=128,  MaxLODSize=512,  OptionalMaxLODSize=256,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,               MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=5);
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,      MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,       MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Cinematic,             MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Effects,               MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=linear, MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,    MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,                MinLODSize=1024, MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=2);
TextureLODGroups=(Group=TEXTUREGROUP_UI,                    MinLODSize=2048, MaxLODSize=2048,                          LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps);
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,              MinLODSize=32,   MaxLODSize=32,                            LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps);
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,             MinLODSize=32,   MaxLODSize=32,                            LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps);
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,          MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_MobileFlattened,       MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_Face,     MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_LightMap, MinLODSize=32,   MaxLODSize=32,                            LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps);
TextureLODGroups=(Group=TEXTUREGROUP_ColorLookupTable,      MinLODSize=2048, MaxLODSize=2048,                          LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps);
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,     MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,     MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Bokeh,                 MinLODSize=256,  MaxLODSize=256,                           LODBias=0,  MinMagFilter=linear, MipFilter=linear, MipGenSettings=TMGS_NoMipmaps);
TextureLODGroups=(Group=TEXTUREGROUP_IESLightProfile,       MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=512,  LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,              MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_HierarchicalLOD,       MinLODSize=512,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0,  MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage,  NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_8BitData,                                                                         LODBias=0,  MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps);
TextureLODGroups=(Group=TEXTUREGROUP_16BitData,                                                                        LODBias=0,  MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps);
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
