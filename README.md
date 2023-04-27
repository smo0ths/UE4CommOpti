
#### updated 4/27/2023~ :ramen:

###### for UE4 games for reference/customization/optimization/learning

###### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

###### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

###### def is pretty much reference to high scalablity group

###### Use Nvidia Image Scaling and turn down in game res for more fps (Enabled dlss quality with this for even more fps)

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
MaxChannels=128; ⚫️DEF 0 🟢64 for PERFORMANCE ⚪️EDITED
CommonAudioPoolSize=0; ⚫️DEF 0
UnfocusedVolumeMultiplier=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=64; ⚫️DEF 70 🟢texturepool cache ⚪️EDITED

[ConsoleVariables]
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=100; ⚫️DEF 100 🟢70 for PERFORMANCE 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.AllowDownsampling=1; ⚫️DEF 1
r.TemporalAA.HistoryScreenPercentage=100; ⚫️DEF 100
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0
r.TemporalAA.Upscaler=1; ⚫️DEF 1
r.TemporalAACatmullRom=0; ⚫️DEF 0
r.TemporalAACurrentFrameWeight=0.1; ⚫️DEF 0.1
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAAPauseCorrect=1; ⚫️DEF 1
r.TemporalAASamples=4; ⚫️DEF 8 ⚪️EDITED
r.TemporalAAUpsampleFiltered=1; ⚫️DEF 1
au.RenderThreadPriority=0; ⚫️DEF 0
AudioThread.BatchAsyncBatchSize=128; ⚫️DEF 128
AudioThread.EnableBatchProcessing=1; ⚫️DEF 1
Compat.UseDXT5NormalMaps=0; ⚫️DEF 0
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 🟣TEST ⚪️EDITED
D3D12.AsyncDeferredDeletion=1; ⚫️DEF 1
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DitheredLOD=1; ⚫️DEF 1
foliage.LODDistanceScale=1; ⚫️DEF 1
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinLOD=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.OverestimateLOD=0; ⚫️DEF 0
FX.AllowAsyncTick=1; ⚫️DEF 1
FX.AllowCulling=1; ⚫️DEF 1
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.BatchAsync=1; ⚫️DEF 0 ⚪️EDITED
FX.BatchAsyncBatchSize=32; ⚫️DEF 32
FX.EarlyScheduleAsync=0; ⚫️DEF 0
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=100; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=104858; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleCollisionIgnoreInvisibleTime=0.1; ⚫️DEF 0.1
FX.ParticleManagerAsyncBatchSize=8; ⚫️DEF 8
FX.ParticleSystemPool.CleanTime=30; ⚫️DEF 30
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
FX.ParticleSystemPool.KillUnusedTime=180; ⚫️DEF 180
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AllowCachedOverlaps=1; ⚫️DEF 1
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.AnimDynamicsLODThreshold=-1; ⚫️DEF -1
p.AnimDynamicsRestrictLOD=-1; ⚫️DEF -1
p.AnimDynamicsWind=1; ⚫️DEF 1
p.BatchPhysXTasksSize=3; ⚫️DEF 3
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
p.RigidBodyLODThreshold=-1; ⚫️DEF -1
p.RigidBodyNode=1; ⚫️DEF 1
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AllowGlobalClipPlane=0; ⚫️DEF 0
r.AllowHDR=0; ⚫️DEF 0
r.AllowLandscapeShadows=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowOcclusionQueries=1; ⚫️DEF 1
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowSimpleLights=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusion.AsyncComputeBudget=1; ⚫️DEF 1
r.AmbientOcclusion.Compute.Smooth=1; ⚫️DEF 1
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMaxQuality=100; ⚫️DEF 100
r.AmbientOcclusionMipLevelFactor=1; ⚫️DEF 0.6 ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=-1; ⚫️DEF -1
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AOApplyToStaticIndirect=0; ⚫️DEF 0
r.AOAsyncBuildQueue=1; ⚫️DEF 1
r.AOComputeShaderNormalCalculation=0; ⚫️DEF 0
r.AOGlobalDFResolution=128; ⚫️DEF 128
r.AOHeightfieldOcclusion=0; ⚫️DEF 0
r.AOOverwriteSceneColor=0; ⚫️DEF 0
r.AOQuality=1; ⚫️DEF 1
r.AOSampleSet=1; ⚫️DEF 1
r.AOViewFadeDistanceScale=0.7; ⚫️DEF 0.7
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.Bloom.HalfResolutionFFT=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.BloomQuality=4; ⚫️DEF 4
r.CapsuleShadows=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.CapsuleShadowsFullResolution=0; ⚫️DEF 0
r.chaos.ReflectionCaptureStaticSceneOnly=1; ⚫️DEF 1
r.ClearCoatNormal=0; ⚫️DEF 0
r.CompileShadersForDevelopment=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.D3D11.Depth24Bit=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.D3D12.Depth24Bit=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.LightUnits=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.DeferSkeletalDynamicDataUpdateUntilGDME=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DeferUniformExpressionCaching=1; ⚫️DEF 1
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DFDistanceScale=1; ⚫️DEF 1
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE ⚪️EDITED
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=5; ⚫️DEF 4 ⚪️EDITED
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DistanceFieldAO=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟣TEST
r.DistanceFieldShadowing=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟣TEST
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1; ⚫️DEF 1
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Downsample.Quality=1; ⚫️DEF 1
r.DrawRectangleOptimization=1; ⚫️DEF 1
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 for PERFORMANCE ⚪️EDITED
r.EnableAsyncComputeTranslucencyLightingVolumeClear=1; ⚫️DEF 1
r.EnableAsyncComputeVolumetricFog=1; ⚫️DEF ❓ 🟣TEST
r.FastBlurThreshold=3; ⚫️DEF 3
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.FinishCurrentFrame=0; ⚫️DEF 0
r.ForceSceneHasDecals=0; ⚫️DEF 0
r.FreeSkeletalMeshBuffers=0; ⚫️DEF 0
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟣TEST
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟢1 for DFSHADOWS DFAO 🟣TEST
r.GPUCrash.CollectionEnable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUCrashDebugging=0; ⚫️DEF 0
r.GPUSkin.Limit2BoneInfluences=0; ⚫️DEF 0
r.GTSyncType=1; ⚫️DEF 1
r.HairStrands.SkyLighting=1; ⚫️DEF 1
r.HDR.EnableHDROutput=0; ⚫️DEF 0
r.HighQualityLightMaps=1; ⚫️DEF 1
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.IrisNormal=0; ⚫️DEF 0
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LensFlareQuality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftAllowTAA=1; ⚫️DEF 1
r.LightShaftDownSampleFactor=1; ⚫️DEF 2 🟢2 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightShaftRenderToSeparateTranslucency=0; ⚫️DEF 0
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaxAnisotropy=8; ⚫️DEF 4 ⚪️EDITED
r.MaxQualityMode=0; ⚫️DEF 0
r.MinRoughnessOverride=0; ⚫️DEF 0
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.NormalMapsForStaticLighting=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.NumBufferedOcclusionQueries=1; ⚫️DEF 1
r.OneFrameThreadLag=1; ⚫️DEF 1
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=16; ⚫️DEF 16
r.PostProcessAllowBlendModes=1; ⚫️DEF 1
r.ReflectionCaptureSupersampleFactor=1; ⚫️DEF 1
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixLargestWeight=10000; ⚫️DEF 10000
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.RenderTargetPool.AllowMultipleAliasingDiscardsPerFrame=0; ⚫️DEF 0
r.RenderTargetPool.TransientAliasingMode=2; ⚫️DEF 2
r.RenderTargetPoolMin=512; ⚫️DEF 1024
r.RHICmdAsyncRHIThreadDispatch=1; ⚫️DEF 1 🟣TEST 🔴experimental
r.RHICmdBypass=0; ⚫️DEF 0
r.SceneColorFormat=3; ⚫️DEF 3
r.SceneColorFringe.Max=-1; ⚫️DEF -1
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SceneRenderTargetResizeMethod=0; ⚫️DEF 0
r.SceneRenderTargetResizeMethodForceOverride=0; ⚫️DEF 0
r.SeparateTranslucency=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ShaderDevelopmentMode=0; ⚫️DEF 0
r.Shaders.FastMath=1; ⚫️DEF 1
r.Shaders.Optimize=1; ⚫️DEF 1
r.Shadow.CachedShadowsCastFromMovablePrimitives=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1
r.Shadow.CacheWPOPrimitives=0; ⚫️DEF 0
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.CSMDepthBias=10; ⚫️DEF 10
r.Shadow.DistanceScale=1; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=4096; ⚫️DEF 2048 🟢512 or 1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxNumPointShadowCacheUpdatesPerFrame=-1; ⚫️DEF -1
r.Shadow.MaxNumSpotShadowCacheUpdatesPerFrame=-1; ⚫️DEF -1
r.Shadow.MaxResolution=2048; ⚫️DEF 2048 🟢1024 for PERFORMANCE
r.Shadow.OcclusionCullCascadedShadowMaps=0; ⚫️DEF 0
r.Shadow.PointLightDepthBias=0.02; ⚫️DEF 0.02
r.Shadow.PointLightSlopeScaleDepthBias=3; ⚫️DEF 3
r.Shadow.RadiusThreshold=0.04; ⚫️DEF 0.04
r.Shadow.SpotLightTransitionScale=60; ⚫️DEF 60
r.Shadow.TransitionScale=60; ⚫️DEF 60
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1; ⚫️DEF 1
r.SkinCache.SceneMemoryLimitInMB=128; ⚫️DEF 128
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=0; ⚫️DEF 0
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyLightingQuality=1; ⚫️DEF 1
r.SSGI.Quality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=1; ⚫️DEF 1
r.SSR.MaxRoughness=-1; ⚫️DEF -1
r.SSR.Quality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.Temporal=0; ⚫️DEF 0
r.SSS.Checkerboard=2; ⚫️DEF 2
r.SSS.HalfRes=1; ⚫️DEF 1
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Streaming.FramesForFullUpdate=5; ⚫️DEF 5
r.Streaming.FullyLoadUsedTextures=0; ⚫️DEF 0
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.MaxNumTexturesToStreamPerFrame=0; ⚫️DEF 0 🟢5 for PERFORMANCE
r.Streaming.MaxTempMemoryAllowed=256; ⚫️DEF 50
r.Streaming.MinLevelRenderAssetScreenSize=100; ⚫️DEF 100
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MipCalculationEnablePerLevelList=1; ⚫️DEF 1
r.Streaming.PoolSize.VRAMPercentageClamp=1024; ⚫️DEF 1024
r.Streaming.PoolSize=1024; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.UseFixedPoolSize=0; ⚫️DEF 0
r.Streaming.UsePerTextureBias=1; ⚫️DEF 1
r.SubsurfaceScattering=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportSkyAtmosphere=1; ⚫️DEF 1
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF 1
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.TextureStreaming=1; ⚫️DEF 1
r.TiledDeferredShading.MinimumCount=80; ⚫️DEF 80
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.EmulateHDR=0; ⚫️DEF 0
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.MergeWithUpscale.Mode=0; ⚫️DEF 0
r.Tonemapper.MergeWithUpscale.Threshold=0.49; ⚫️DEF 0.49
r.Tonemapper.Quality=3; ⚫️DEF 5 🟢0 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 0
r.TonemapperGamma=0; ⚫️DEF 0
r.TranslucencyLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.UITextureLODBias=0; ⚫️DEF 0
r.UniformBufferPooling=1; ⚫️DEF 1
r.UseClusteredDeferredShading=0; ⚫️DEF 0
r.UseFastIntersect=1; ⚫️DEF 1
r.UseParallelGetDynamicMeshElementsTasks=1; ⚫️DEF 0 🟣TEST ⚪️EDITED
r.ViewDistanceScale.ApplySecondaryScale=0; ⚫️DEF 0
r.ViewDistanceScale.SecondaryScale=1; ⚫️DEF 1
r.ViewDistanceScale=1; ⚫️DEF 1 🟢0.8 for PERFORMANCE
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridPixelSize=32; ⚫️DEF 16 ⚪️EDITED
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VSync=0; ⚫️DEF 0
r.Vulkan.Depth24Bit=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.RefractionDownsampleFactor=2; ⚫️DEF 2
r.Water.SingleLayer.SSR=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSRTAA=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.TiledComposite=1; ⚫️DEF 1
rhi.SyncInterval=0; ⚫️DEF 1 ⚪️EDITED
rhi.SyncSlackMS=0; ⚫️DEF 10 ⚪️EDITED
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
InitialButtonRepeatDelay=0.2;------def 0.2
ButtonRepeatDelay=0.1;------def 0.1
DoubleClickTime=0.1;------def 0.25
```

---

<details><summary>Open GameUserSettings.ini these commands will overwrite your config so make sure they are correct also set your scalability groups 0 low 1 med  2 high 3 epic 4 cinematic, check for new stuff after updates</summary>
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
TextureStreamPoolSizeStorage=(Value=800)
MaxAnisotropy=(Value=)
FoliageMinLOD=(Value=1)
HZBOcclusion=(Value=)
ContactShadows=(Value=)
DetailMode=(Value=1)
AudioQualityLevel=3
MaxAnisotropy=8
bUseVSync=0
GlobalSensitivity=0.183
MaxFPS=
FrameRateLimit=
MenuFrameRateLimit=
HDRDisplayOutputNits=300;
DoubleKeyPressTime=0.1
DistanceFieldShadows=1;
Gamma=2.2
TAASampleStorage=4
bRTXEnabled=0
bRTXReflectionsEnabled=0
bRTXShadowsEnabled=0
bRTXAmbientOcclusionEnabled=0
DlssQualitySetting=1
ResolutionScaleModifier=1
DFAO=
Tessellation=0
TessellationMode=9999999
Tessellation=(Value=0)
TessellationMode=(Value=9999999)
bTelemetryEnabled=0
bUseDynamicResolution=0
FullscreenMode=0
PreferredFullscreenMode=0
ContactShadows=0
PostFX_Saturation=1.2
PostFX_Sharpness=0
OverrideOptions=(("r.PlaceHolder1", (Value=0,bModified=True)),("r.PlaceHolder2", (Value=1,bModified=False)));------works like engineini but in gameusersettingsini
OverrideOptions=(("r.Streaming.PoolSize", (Value=800,bModified=True)));------another example

[ScalabilityGroups]
sg.ResolutionQuality=100
sg.ViewDistanceQuality=2
sg.AntiAliasingQuality=2
sg.PostProcessQuality=2
sg.ShadowQuality=2
sg.TextureQuality=2
sg.EffectsQuality=2
sg.FoliageQuality=2
sg.ShadingQuality=2
sg.AnimationQuality=2
```

---

<details><summary>Open DeviceProfiles.ini and textures lods, skip this and just use the games texture settings imo</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
</p>
</details>

```python
[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Cinematic,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ColorLookupTable,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=linear,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_HierarchicalLOD,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_IESLightProfile,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Impostor,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ImpostorNormalDepth,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_MAX,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_MobileFlattened,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=point,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_Face,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_LightMap,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project01,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project02,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project03,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project04,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project05,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project06,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project07,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project08,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project09,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project10,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project11,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project12,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project13,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project14,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project15,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,MinLODSize=256,MaxLODSize=1024,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,MinLODSize=256,MaxLODSize=1024,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_NoMipmaps,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=256,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=256,MaxLODSize_Tiniest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=0,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
```

---

#### in nvidia control panel

##### 1. 3D settings -> adjust image settings with preview -> use my preference emphasizing performance apply.

##### 2. click on use the advanced 3D image settings and apply then click "take me there"

##### 3. Anisotropic filtering:  set Application-controlled (you can force the setting in here if you can't notice it working in certain games)

##### 4. Antialiasing - mode: set Application-controlled

##### 5. Low latency mode (Only works with dx11 and lower api):

###### Off and ~85% gpu usage for multiple frame buffers sacrificing latency (cap fps til gpu usage is ~85%) (for visual fluidity of frames)

###### On forces 1 frame buffer (for lower latency than off) (for visual fluidity of frames)

###### Ultra and/or nvidia relfex (in-game dx12 only) and ~97% gpu usage for lowest latency (could be less fluid frames at low fps)

##### 6. Power management mode:  prefer max performance  (this is the "+ boost" in reflex + boost)

##### 7. Preferred refresh rate:  Highest available

##### 8. Texture filtering - anisotropic sample optimization:  on  (off will look better if this even works in your game) (you may need to reapply because NVCP will reset when you change other settings)

##### 9. Texture filtering - negative LOD bias:  allow (allows -1,-2 ect bias) clamp (0 mipmap bias) + integers give more performance at cost of bland textures, most game devs make their HQ textures with a -1 clamp so might want to just leave this on allow and change textures in game (you may need to re-apply because NVCP will reset when you change other settings)

##### 10. Texture filtering quality:  high performance

##### 11. Texture filtering - trilinear optimization:  on

#####  12. Vertical sync:  Off

#####  13. Display -> Adjust desktop size and position -> set no scaling and Perform scaling on: Display

<details><summary>14. Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method) click for how to</summary>
<p>
1. NVCleanstall enabling it in advanced settings before installing or
<br>
2. use Wtools enable it and restart or
<br>
3. find ID: open device manager right click your GPU properties and click on events tab
<br>
looks like this:
<br>
HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties
<br>
find in regedit and set MSISupported to 1 then restart
</p>
</details>
