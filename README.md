#### updated 1/5/2023 ✂️ 📋 :ramen: v0.9.7.2 release

##### for UE4 games for reference/customization/optimization/learning

##### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

##### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

##### make sure your scaling % is set correctly! and match PIP(scope) resolution scaling in games (manually in graphic settings) for PERFORMANCE

##### 2k use 58%(balance) 67%(quality) 70%(custom/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/CAS/FSR123/XeSS)

##### 4k use 33%(ultra performance) 50%(performance/TAAU) scaling for PERFORMANCE (DLSS123/TAAU/CAS/FSR123/XeSS)

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
PoolSizeVRAMPercentage=50;---------------⚫️DEF 70 🔵 EDITED 🔵 texturepool cache

[ConsoleVariables]
sg.ResolutionQuality=50;---------------🟡 set correctly
sg.ViewDistanceQuality=2;
sg.AntiAliasingQuality=2;
sg.ShadowQuality=2;
sg.PostProcessQuality=2;
sg.TextureQuality=2;
sg.EffectsQuality=2;
sg.FoliageQuality=2;
r.ScreenPercentage=50;---------------🟡 set correctly
r.SecondaryScreenPercentage.GameViewport=0;---------------🟢 83.33 for PERFORMANCE
r.Upscale.Quality=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.Tonemapper.MergeWithUpscale.Mode=1;---------------🟢 1 for PERFORMANCE
r.GTSyncType=0;---------------🔵 EDITED
r.VSync=0;
rhi.SyncInterval=0;---------------🔵 EDITED
r.MSAACount=0;
r.DynamicRes.OperationMode=0;
r.DynamicRes.MaxScreenPercentage=70;---------------🔵 req DynamicRes.OperationMode
r.DynamicRes.FrameTimeBudget=10;---------------🔵 req DynamicRes.OperationMode
r.SceneRenderTargetResizeMethodForceOverride=0;
r.SceneRenderTargetResizeMethod=0;
r.PostProcessAAQuality=5;---------------🔵 EDITED 🔵 0 for off 1,2 for FXAA 3,4,5,6 for TAA
r.TemporalAA.Algorithm=0;---------------🟢 0 for PERFORMANCE 🔵 1 for Gen5 TAAU
r.TemporalAAFilterSize=0.1;---------------🔵 EDITED 🔵 req Gen5 TAAU
r.TemporalAA.Upsampling=1;---------------🔵 EDITED 🔵 TAAU
r.TemporalAACurrentFrameWeight=0.03;
r.TemporalAASamples=8;
foliage.DensityScale=0.6;---------------🟢 0.6 for PERFORMANCE 🔵 EDITED
foliage.DitheredLOD=1;
foliage.LODDistanceScale=1;
foliage.MinLOD=0;---------------🟢 1 for PERFORMANCE
foliage.MinInstancesPerOcclusionQuery=256;
foliage.MinimumScreenSize=0.0005f;---------------🟢 0.001f,0.0005f for PERFORMANCE 🔵 EDITED
foliage.DiscardDataOnLoad=0;
r.AllowSimpleLights=1;---------------🟢 0 for PERFORMANCE
r.ParticleLightQuality=2;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.EmitterSpawnRateScale=1;---------------🟢 0.125,0.5 for PERFORMANCE
fx.Niagara.QualityLevel=2;---------------🟢 0,1 for PERFORMANCE
fx.MaxCPUParticlesPerEmitter=25;---------------🟢 25 for PERFORMANCE 🔵 EDITED
fx.MaxGPUParticlesSpawnedPerFrame=1000;---------------🟢 1000 for PERFORMANCE 🔵 EDITED
fx.GPUSimulationTextureSizeX=1024;
fx.GPUSimulationTextureSizeY=1024;
r.ParticleMinTimeBetweenTicks=16;
grass.DensityScale=0.6;---------------🟢 0.6 for PERFORMANCE 🔵 EDITED
grass.DisableDynamicShadows=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
grass.MaxAsyncTasks=4;
grass.MaxCreatePerFrame=1;
grass.MaxUpdateFrequency=30;
grass.TickInterval=16;---------------🟢 16 for PERFORMANCE 🔵 EDITED
grass.DiscardDataOnLoad=0;
a.URO.Enable=1;
a.URO.ForceAnimRate=0;
a.URO.ForceInterpolation=1;
p.AnimDynamics=1;---------------🟢 0 for PERFORMANCE
p.RigidBodyNode=1;---------------🟢 0 for PERFORMANCE
p.ClothPhysics=1;---------------🟢 0 for PERFORMANCE
r.Tonemapper.Quality=1;---------------🔵 EDITED
r.Tonemapper.GrainQuantization=0;---------------🔵 EDITED
r.TonemapperGamma=2.2;---------------🔵 EDITED
r.Tonemapper.Sharpen=0;---------------🔵 EDITED
r.MotionBlurQuality=0;---------------🔵 EDITED
r.SceneColorFringeQuality=0;---------------🔵 EDITED
r.EyeAdaptation.MethodOverride=-1;
r.EyeAdaptationQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.EyeAdaptation.Basic.Compute=1;---------------🟢 1 for PERFORMANCE
r.DefaultFeature.AutoExposure.Method=1;---------------🟢 1 for PERFORMANCE 🔵 1 for BasicAutoExposure
r.LensFlarequality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.DepthOfFieldQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.DOF.TemporalAAQuality=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.DOF.Gather.RingCount=3;---------------🟢 3 for PERFORMANCE 🔵 EDITED
r.DOF.Scatter.ForegroundCompositing=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.DOF.Scatter.BackgroundCompositing=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.DOF.Kernel.MaxForegroundRadius=0.006;---------------🟢 0.006 for PERFORMANCE 🔵 EDITED
r.DOF.Kernel.MaxBackgroundRadius=0.006;---------------🟢 0.006 for PERFORMANCE 🔵 EDITED
r.BloomQuality=4;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.Bloom.Cross=0.7777;---------------🔵 EDITED 🔵 0.7777 for anamorphic bloom
r.Filter.SizeScale=0.7;---------------🔵 EDITED
r.LightShaftQuality=1;---------------🟢 0 for PERFORMANCE
r.LightShaftFirstPassDistance=0.1;
r.LightShaftDownSampleFactor=2;
r.LightShaftBlurPasses=3;
r.LightShaftAllowTAA=1;
r.ViewDistanceScale=1;---------------🟢 0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;---------------🟢 0 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1;
r.StaticMeshLODDistanceScale=1;
r.DetailMode=2;---------------🟢 0,1 for PERFORMANCE
r.RefractionQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.SupportAnisotropicMaterials=1;---------------🟢 0 for PERFORMANCE
r.AnisotropicMaterials=1;---------------🟢 0 for PERFORMANCE
r.MaxAnisotropy=16;---------------🟢 0 for PERFORMANCE
r.MaterialQualityLevel=1;---------------🟢 0,2 for PERFORMANCE
r.SupportMaterialLayers=1;---------------🟢 0 for PERFORMANCE
r.SubsurfaceScattering=1;---------------🟢 0 for PERFORMANCE
r.SSS.Quality=0;
r.SSS.SampleSet=0;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.SSS.Checkerboard=1;
r.SSS.HalfRes=1;
r.SSS.Scale=1;---------------🟢 0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=999999;---------------🟢 999999 for PERFORMANCE
r.SupportSkyAtmosphere=1;
r.SupportSkyAtmosphereAffectsHeightFog=1;
r.SkyAtmosphere.FastSkyLUT=1;
r.SkyAtmosphere.FastSkyLUT.SampleCountMax=32;---------------🟢 32 for PERFORMANCE 🔵 EDITED
r.SkyAtmosphere.SampleCountMax=32;---------------🟢 32 for PERFORMANCE 🔵 EDITED
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0;---------------🟢 0 for PERFORMANCE
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=1;---------------🟢 1 for PERFORMANCE
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1;
r.SkyAtmosphere.AerialPerspectiveLUT.SampleCountMaxPerSlice=1;---------------🔵 EDITED
r.Water.EnableShallowWaterSimulation=1;---------------🟢 0 for PERFORMANCE
r.Water.ShallowWaterRenderTargetSize=1024;
r.Water.EnableUnderwaterPostProcess=1;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.TiledComposite=1;
r.Water.UseSplineKeyOptimization=1;
r.Water.WaterSplineResampleMaxDistance=50;
r.Water.WaterMesh.LODScaleBias=-0.5;---------------🟢 -0.5 for PERFORMANCE 🔵 EDITED
r.Water.WaterMesh.LODMorphEnabled=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.Water.WaterMesh.TessFactorBias=-1;---------------🟢 -1 for PERFORMANCE 🔵 EDITED
r.Water.SingleLayer.Reflection=1;---------------🟢 0 for PERFORMANCE
r.Water.SingleLayer.RefractionDownsampleFactor=2;
r.Water.SingleLayer.SSR=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.Water.SingleLayer.SSRTAA=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.SkyLight.RealTimeReflectionCapture=1;---------------🟢 0 for PERFORMANCE
r.SkyLight.RealTimeReflectionCapture.DepthBuffer=1;
r.DoTiledReflections=1;---------------🟢 0 for PERFORMANCE
r.ReflectionEnvironment=1;---------------🟢 0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixing=1;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;
r.AllowGlobalClipPlane=1;---------------🟢 0 for PERFORMANCE 🔵 EDITED 🔵 1 for planar reflections
r.MinRoughnessOverride=0.04;---------------🔵 EDITED
r.SSR.MaxRoughness=0.4;---------------🔵 EDITED
r.SSR.HalfResSceneColor=0;
r.SSR.Quality=2;---------------🟢 0 for PERFORMANCE
r.SSR.Temporal=0;
r.LightFunctionQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED
r.LightMaxDrawDistanceScale=1;---------------🟢 0.6 for PERFORMANCE
r.MinScreenRadiusForLights=0.03;---------------🟢 0.04,0.06 for PERFORMANCE 🔵 EDITED
r.HairStrands.Interpolation.UseSingleGuide=1;
r.HairStrands.SkyAO.SampleCount=4;
r.HairStrands.SkyLighting.IntegrationType=2;
r.HairStrands.SkyLighting=1;
r.HairStrands.Visibility.MSAA.SamplePerPixel=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.VolumetricFog=1;---------------🟢 0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=8;---------------🟢 16 for PERFORMANCE 🔵 EDITED
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.HistoryMissSupersampleCount=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=1;
r.VolumetricFog.TemporalReprojection=1;---------------🟢 0 for PERFORMANCE
r.VolumetricFog.LightFunction=1;
r.VolumetricFog.LightFunction.DirectionalLightSupersampleScale=1;---------------🔵 EDITED
r.VolumetricFog.LightFunction.Resolution=128;
r.VolumetricFog.Jitter=0;
r.VolumetricRenderTarget=1;
r.VolumetricRenderTarget.Mode=0;
r.VolumetricCloud=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.VolumetricCloud.ShadowMap=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.VolumetricCloud.SkyAO=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.VolumetricCloud.DisableCompute=0;
r.DistanceFields.MaxPerMeshResolution=128;
r.DistanceFields.ParallelAtlasUpdate=1;
r.DistanceFields.ForceMaxAtlasSize=1;
r.DistanceFields.AtlasSizeZ=1024;
r.DistanceFields.AtlasSizeXY=512;
r.GenerateMeshDistanceFields=1;---------------🟢 0 for PERFORMANCE 🔵 1 builds DFS and DFAO mesh
r.DistanceFieldShadowing=1;---------------🟢 0 for PERFORMANCE 🔵 req GenerateMeshDistanceFields
r.DFShadowQuality=2;---------------🟢 0,1,2 for PERFORMANCE 🔵 EDITED 🔵 req DistanceFieldShadowing
r.DFDistanceScale=1;
r.DFFullResolution=0;
r.DFTwoSidedMeshDistanceBias=10;---------------🔵 EDITED
r.DFFarTransitionScale=1;
r.HeightfieldGlobalIllumination=0;---------------🟢 0 for PERFORMANCE
r.HeightFieldShadowing=0;---------------🟢 0 for PERFORMANCE
r.HFShadowQuality=0;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED 🔵 req HeightFieldShadowing
r.CapsuleShadows=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.CapsuleShadowsFullResolution=0;
r.CapsuleDirectShadows=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.CapsuleIndirectShadows=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.ContactShadows=0;---------------🟢 0 for PERFORMANCE 🔵 EDITED
r.ContactShadows.NonShadowCastingIntensity=0;
r.AllowPointLightCubemapShadows=1;---------------🟢 0 for PERFORMANCE
r.AllowLandscapeShadows=1;---------------🟢 0 for PERFORMANCE
r.ShadowQuality=3;---------------🟢 3 for PERFORMANCE 🔵 EDITED
r.Shadow.FilterMethod=0;---------------🟢 0 for PERFORMANCE 🔵 1 for PCSS shadows
r.Shadow.DistanceScale=1;---------------🔵 EDITED
r.Shadow.CSM.MaxCascades=4;---------------🟢 1,2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1;---------------🔵 EDITED
r.Shadow.CSMShadowDistanceFadeoutMultiplier=1;
r.Shadow.CachePreshadow=1;
r.Shadow.PreShadowResolutionFactor=0.5;
r.Shadow.MaxCSMResolution=2048;---------------🟢 1024 for PERFORMANCE
r.Shadow.MaxResolution=1024;---------------🟢 512,1024 for PERFORMANCE 🔵 EDITED
r.Shadow.RadiusThreshold=0.04;
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;---------------🟢 0 for PERFORMANCE 🔵 1 for light cast a shadow
r.Shadow.CacheWholeSceneShadows=1;
r.Shadow.MaxNumPointShadowCacheUpdatesPerFrame=1;---------------🔵 EDITED
r.Shadow.MaxNumSpotShadowCacheUpdatesPerFrame=1;---------------🔵 EDITED
r.Shadow.FadeExponent=1;---------------🔵 EDITED
r.Shadow.UnbuiltPreviewInGame=0;
r.Shadow.WholeSceneShadowCacheMb=150;
r.Shadow.CSMDepthBias=10;
r.Shadow.CSMSlopeScaleDepthBias=3;
r.Shadow.CSMReceiverBias=0.9;
r.Shadow.PointReceiverBias=0.5;
r.Shadow.RectReceiverBias=0.5;
r.Shadow.SpotReceiverBias=0.5;
r.Shadow.Denoiser=0;
r.ParallelShadow=1;---------------🟢 0 for PERFORMANCE
r.ParallelShadowsNonWholeScene=0;---------------🟢 0 for PERFORMANCE
r.ParallelTranslucency=1;
r.ParallelGeometryCollectionBatchSize=1024;
r.ParallelSingleLayerWaterPass=1;
r.TranslucentLightingVolume=1;---------------🟢 0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;---------------🟢 32 for PERFORMANCE 🔵 EDITED
r.TranslucencyVolumeBlur=1;---------------🟢 0 for PERFORMANCE
r.GenerateLandscapeGIData=0;---------------🟢 0 for PERFORMANCE 🔵 req GenerateMeshDistanceFields
r.SSGI.Enable=0;---------------🟢 0 for PERFORMANCE
r.SSGI.Quality=0;---------------🟢 0,2 for PERFORMANCE 🔵 EDITED 🔵 req SSGI.Enable
r.AmbientOcclusionMipLevelFactor=0.5;
r.AmbientOcclusionMaxQuality=-25;---------------🔵 EDITED
r.AmbientOcclusionLevels=1;---------------🟢 0 for PERFORMANCE
r.AmbientOcclusionRadiusScale=1;
r.AmbientOcclusionStaticFraction=-1;---------------🟢 0 for PERFORMANCE
r.AmbientOcclusion.Compute=0;---------------🔵 WIP
r.DistanceFieldAO=1;---------------🟢 0 for PERFORMANCE 🔵 req GenerateMeshDistanceFields
r.AOQuality=1;---------------🟢 0,1 for PERFORMANCE 🔵 EDITED 🔵 req DistanceFieldAO
r.AOAsyncBuildQueue=1;
r.AOComputeShaderNormalCalculation=0;
r.AOOverwriteSceneColor=0;
r.AOApplyToStaticIndirect=0;
r.AOGlobalDFResolution=128;
r.AOHeightfieldOcclusion=0;
r.AOGlobalDistanceFieldRepresentHeightfields=0;
r.AOGlobalDistanceFieldCacheMostlyStaticSeparately=1;
r.AOGlobalDistanceField=0;---------------🟢 0 for PERFORMANCE 🔵 0 for adaptive method
r.AOUseSurfaceCache=1;
r.AOSampleSet=0;
r.AOObjectDistanceField=1;
r.AOSpecularOcclusionMode=1;
r.SkySpecularOcclusionStrength=1;
D3D12.AdjustTexturePoolSizeBasedOnBudget=0;---------------🟢 1 for PERFORMANCE
D3D12.DynamicTexturePoolSize=0;
D3D12.ForceThirtyHz=0;
D3D12.TexturePoolOnlyAccountStreamableTexture=1;
D3D12.UseUpdateTexture3DComputeShader=0;
D3D12.ZeroBufferSizeInMB=4;
r.LandscapeLODDistributionScale=1;
r.LandscapeLOD0DistributionScale=1;
r.ParticleLODBias=0;
r.LandscapeLODBias=0;
r.SkeletalMeshLODBias=0;
r.MipMapLODBias=0;---------------🟢 1 for PERFORMANCE
r.RenderTargetPoolMin=200;
r.Streaming.UsePerTextureBias=1;
r.Streaming.UseFixedPoolSize=1;
r.Streaming.LimitPoolSizeToVRAM=0;---------------🔵 EDITED
r.Streaming.PoolSize=500;---------------🔵 EDITED
r.Streaming.PoolSizeForMeshes=-1;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.MinMipForSplitRequest=0;
r.Streaming.FlushTimeOut=3;
r.Streaming.HiddenPrimitiveScale=1;---------------🟢 0.5 for PERFORMANCE
r.Streaming.FramesForFullUpdate=10;
r.Streaming.AmortizeCPUToGPUCopy=1;---------------🟢 1 for PERFORMANCE 🔵 EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=100;---------------🟢 1 for PERFORMANCE 🔵 EDITED 🔵 req AmortizeCPUToGPUCopy
r.Streaming.NumStaticComponentsProcessedPerFrame=1;
r.Streaming.MaxTempMemoryAllowed=100;---------------🔵 EDITED
r.Streaming.DropMips=2;
r.Streaming.FullyLoadUsedTextures=0;
r.NGX.LogLevel=0;---------------🔵 EDITED
r.NGX.DLSS.Sharpness=0;
r.NGX.DLSS.AutoExposure=1;
r.NGX.DLSS.Reflections.TemporalAA=0;
r.NGX.DLSS.WaterReflections.TemporalAA=0;
r.D3D12.GPUCrashDebuggingMode=0;
r.DX12NVAfterMathEnabled=0;
r.gpucrash.collectionenable=0;---------------🔵 EDITED
r.GPUCrashDebugging=0;
r.Shaders.Optimize=1;
r.Shaders.Validation=0;
r.ForceAllCoresForShaderCompiling=0;
r.ShaderDevelopmentMode=0;
r.CompileShadersForDevelopment=0;---------------🔵 EDITED
r.CreateShadersOnLoad=1;
r.DoInitViewsLightingAfterPrepass=0;---------------🔵 experimental
r.DoLazyStaticMeshUpdate=0;---------------🔵 experimental
r.AlsoUseSphereForFrustumCull=0;---------------🔵 experimental
r.SplineMesh.NoRecreateProxy=1;
r.FrustumCullNumWordsPerTask=64;
r.DiffuseIndirect.Denoiser=0;---------------🔵 EDITED
r.IndirectLightingCache=1;
r.LightCulling.Quality=1;
r.LightPropagationVolume=0;---------------🔵 WIP
r.UniformBufferPooling=1;
r.DBuffer=0;---------------🔵 EDITED
r.AllowDownsampledStandardTranslucency=1;---------------🔵 EDITED
r.SeparateTranslucency=1;
r.SeparateTranslucencyScreenPercentage=100;
r.SeparateTranslucencyAutoDownsample=1;
r.DefaultBackBufferPixelFormat=4;
r.SceneColorFormat=3;---------------🟢 2,3 for PERFORMANCE
Compat.UseDXT5NormalMaps=0;
r.ClearCoatNormal=1;---------------🟢 0 for PERFORMANCE
r.HighQualityLightMaps=1;
r.IrisNormal=1;---------------🟢 0 for PERFORMANCE
r.NormalMapsForStaticLighting=1;
r.AllowOcclusionQueries=1;
r.NumBufferedOcclusionQueries=1;
r.HZBOcclusion=0;
r.OneFrameThreadLag=1;
r.FinishCurrentFrame=0;---------------🟢 0 for PERFORMANCE 🔵 latency
r.GBufferFormat=1;---------------🟢 0 for PERFORMANCE
r.ClearSceneMethod=1;
r.UseClusteredDeferredShading=0;
r.TiledDeferredShading=1;---------------🟢 0 for PERFORMANCE
r.TiledDeferredShading.MinimumCount=1;---------------🔵 EDITED
```

---

<details><summary>in Scalability.ini put config under if settings dont load, or change cutscene dynamic Cine values</summary>
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
✂️📋

[ViewDistanceQuality@2]
✂️📋

[ShadowQuality@2]
✂️📋

[PostProcessQuality@2]
✂️📋

[TextureQuality@2]
✂️📋

[EffectsQuality@2]
✂️📋

[FoliageQuality@2]
✂️📋

[ShadingQuality@2]
✂️📋

[AntiAliasingQuality@Cine]
✂️📋

[ViewDistanceQuality@Cine]
✂️📋

[ShadowQuality@Cine]
✂️📋

[PostProcessQuality@Cine]
✂️📋

[TextureQuality@Cine]
✂️📋

[EffectsQuality@Cine]
✂️📋

[FoliageQuality@Cine]
✂️📋

[ShadingQuality@Cine]
✂️📋
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

[ScalabilityGroups]
sg.ResolutionQuality=50;---------------🟡 set correctly
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
InitialButtonRepeatDelay=0.2;
ButtonRepeatDelay=0.1;
DoubleClickTime=0.01;---------------🔵 EDITED
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
TextureLODGroups=(Group=TEXTUREGROUP_World,                 MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,        MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,         MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Character,             MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,    MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,     MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,                MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,       MinLODSize=128,  MaxLODSize=512,  OptionalMaxLODSize=256,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,        MinLODSize=128,  MaxLODSize=512,  OptionalMaxLODSize=256,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
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

###### win + r type cmd then press control+shift+enter (starts as admin) then add key. NVcleaninstall gives you more MSIs options. Newest drivers auto do this on 40 series cards, i wonder if its default or set to high.

```python
reg add "HKLM\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties" /v MSISupported /t REG_DWORD /d 1 /f
```

###### restart

###### in device manager/view/resources by connection/GPU name should have a negative number in parentheses if MSIs is enabled

#### Disable HPET (High Precision event timer) in device manager/system devices and/or in your bios to get lower latency and more fps
