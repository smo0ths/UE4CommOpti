#### updated 5/26/2023 x6 🍝 :ramen:

###### for UE4 games for reference/customization/optimization/learning

###### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

###### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

###### def is pretty much reference to high scalablity group

###### Use NIS and DLSS at the same time to get the most fps but you will be GPU scaling wich is not a big deal

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
MaxChannels=64; 🟣TEST
CommonAudioPoolSize=0;
UnfocusedVolumeMultiplier=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=70; ⚫️DEF 70 🟢texturepool cache 🟣TEST

[ConsoleVariables]
sg.ResolutionQuality=70;
sg.ViewDistanceQuality=2;
sg.AntiAliasingQuality=2;
sg.PostProcessQuality=2;
sg.ShadowQuality=2;
sg.TextureQuality=2;
sg.EffectsQuality=2;
sg.FoliageQuality=2;
sg.ShadingQuality=2;
sg.AnimationQuality=0;
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1; ⚫️DEF 1
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.SupportAllShaderPermutations=0; ⚫️DEF 0
r.SupportAnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportLowQualityLightmaps=0; ⚫️DEF 0
r.SupportMaterialLayers=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF ❓ 🟣TEST
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; ⚫️DEF 1
r.SkyAtmosphere.FastSkyLUT=1; ⚫️DEF 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟣TEST
r.AllowSimpleLights=1; ⚫️DEF 1 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟡req some light shadows 🟣TEST
r.Shadow.CachePreshadow=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWPOPrimitives=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🟣TEST
r.RayTracing=0; ⚫️DEF 0
r.EarlyZPass=2; ⚫️DEF 2
r.EarlyZPassMovable=1; ⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.EarlyZSortMasked=1; ⚫️DEF 1
au.SetAudioChannelCount=64; ⚫️DEF ❓ 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VSync=0; ⚫️DEF 0
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI 🟣TEST
r.DistanceFieldGI=0; ⚫️DEF ❓
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED 🟣TEST
r.DistanceFields=1; ⚫️DEF 1
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFields.AtlasSizeZ=1024; ⚫️DEF 1024
r.DistanceFields.AtlasSizeXY=512; ⚫️DEF 512
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.SkipPhysicsReplication=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=6; ⚫️DEF 3 ⚪️EDITED 🟣TEST
p.AnimDynamicsWind=1; ⚫️DEF 1
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
r.AOComputeShaderNormalCalculation=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED 🟣TEST
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GTSyncType=1; ⚫️DEF 1 🟣TEST
r.HZB.BuildUseCompute=1; ⚫️DEF 1 🟣TEST
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.StencilForLODDither=1; ⚫️DEF 1
r.StencilLODMode=2; ⚫️DEF 2
r.Emitter.FastPoolEnable=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
FX.AllowCulling=1; ⚫️DEF 1 🟣TEST
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=20; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
D3D12.UseUpdateTexture3DComputeShader=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE 🟣TEST
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03 🟣TEST
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01 🟣TEST
r.MinScreenRadiusForSmallLights=0.01; ⚫️DEF 0.01 🟣TEST
r.LightPropagationVolume=0; ⚫️DEF 0
r.PostProcessing.PreferCompute=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.CreateShadersOnLoad=0; ⚫️DEF 0 🟣TEST
r.ShaderPipelineCache.GameFileMaskEnabled=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.TextureStreaming=1; ⚫️DEF 1
r.MeshStreaming=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.PoolSize=1200; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟣TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=30; ⚫️DEF 0 🟣TEST
r.Streaming.MinBoost=0; ⚫️DEF 0
r.Streaming.Boost=1; ⚫️DEF 1
r.Streaming.HLODStrategy=0; ⚫️DEF 0
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟣TEST
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DensityScale=0.8; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=20; ⚫️DEF 30 ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.EyeAdaptation.MethodOverride=-1; ⚫️DEF -1
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.NormalMapsForStaticLighting=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ClearCoatNormal=0; ⚫️DEF 0
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.EmitterSpawnRateScale=1; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightCulling.Quality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightingDetailMode=100; ⚫️DEF 150 ⚪️EDITED 🟣TEST
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.LightShaftDownSampleFactor=2; ⚫️DEF 2
r.LightShaftFirstPassDistance=0.01; ⚫️DEF 0.1
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Upscale.Quality=2; ⚫️DEF 2
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟡for ScreenPercentage 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE 🟣TEST
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED 🟣TEST
r.AOGlobalDFResolution=128; ⚫️DEF 128 🟣TEST
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=0.6; ⚫️DEF 0.6 🟣TEST
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.85; ⚫️DEF 0.85 🟣TEST
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED 🟣TEST
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED 🟣TEST
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.HeightFieldShadowing=0; ⚫️DEF 0
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=2; ⚫️DEF 2
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED 🟣TEST
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Burley.BilateralFilterKernelFunctionType=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.Burley.Quality=1; ⚫️DEF 1 🟣TEST
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE 🟣TEST
r.Tonemapper.Sharpen=0.25; ⚫️DEF 2 ⚪️EDITED 🟣TEST
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24; ⚫️DEF 16 ⚪️EDITED 🟣TEST
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
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
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1; ⚫️DEF 1
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.SupportAllShaderPermutations=0; ⚫️DEF 0
r.SupportAnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportLowQualityLightmaps=0; ⚫️DEF 0
r.SupportMaterialLayers=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF ❓ 🟣TEST
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; ⚫️DEF 1
r.SkyAtmosphere.FastSkyLUT=1; ⚫️DEF 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟣TEST
r.AllowSimpleLights=1; ⚫️DEF 1 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟡req some light shadows 🟣TEST
r.Shadow.CachePreshadow=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWPOPrimitives=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🟣TEST
r.RayTracing=0; ⚫️DEF 0
r.EarlyZPass=2; ⚫️DEF 2
r.EarlyZPassMovable=1; ⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.EarlyZSortMasked=1; ⚫️DEF 1
au.SetAudioChannelCount=64; ⚫️DEF ❓ 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VSync=0; ⚫️DEF 0
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI 🟣TEST
r.DistanceFieldGI=0; ⚫️DEF ❓
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED 🟣TEST
r.DistanceFields=1; ⚫️DEF 1
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFields.AtlasSizeZ=1024; ⚫️DEF 1024
r.DistanceFields.AtlasSizeXY=512; ⚫️DEF 512
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.SkipPhysicsReplication=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=6; ⚫️DEF 3 ⚪️EDITED 🟣TEST
p.AnimDynamicsWind=1; ⚫️DEF 1
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
r.AOComputeShaderNormalCalculation=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED 🟣TEST
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GTSyncType=1; ⚫️DEF 1 🟣TEST
r.HZB.BuildUseCompute=1; ⚫️DEF 1 🟣TEST
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.StencilForLODDither=1; ⚫️DEF 1
r.StencilLODMode=2; ⚫️DEF 2
r.Emitter.FastPoolEnable=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
FX.AllowCulling=1; ⚫️DEF 1 🟣TEST
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=20; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
D3D12.UseUpdateTexture3DComputeShader=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE 🟣TEST
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03 🟣TEST
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01 🟣TEST
r.MinScreenRadiusForSmallLights=0.01; ⚫️DEF 0.01 🟣TEST
r.LightPropagationVolume=0; ⚫️DEF 0
r.PostProcessing.PreferCompute=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.CreateShadersOnLoad=0; ⚫️DEF 0 🟣TEST
r.ShaderPipelineCache.GameFileMaskEnabled=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.TextureStreaming=1; ⚫️DEF 1
r.MeshStreaming=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.PoolSize=1200; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟣TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=30; ⚫️DEF 0 🟣TEST
r.Streaming.MinBoost=0; ⚫️DEF 0
r.Streaming.Boost=1; ⚫️DEF 1
r.Streaming.HLODStrategy=0; ⚫️DEF 0
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟣TEST
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DensityScale=0.8; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=20; ⚫️DEF 30 ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.EyeAdaptation.MethodOverride=-1; ⚫️DEF -1
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.NormalMapsForStaticLighting=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ClearCoatNormal=0; ⚫️DEF 0
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.EmitterSpawnRateScale=1; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightCulling.Quality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightingDetailMode=100; ⚫️DEF 150 ⚪️EDITED 🟣TEST
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.LightShaftDownSampleFactor=2; ⚫️DEF 2
r.LightShaftFirstPassDistance=0.01; ⚫️DEF 0.1
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Upscale.Quality=2; ⚫️DEF 2
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟡for ScreenPercentage 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE 🟣TEST
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED 🟣TEST
r.AOGlobalDFResolution=128; ⚫️DEF 128 🟣TEST
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=0.6; ⚫️DEF 0.6 🟣TEST
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.85; ⚫️DEF 0.85 🟣TEST
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED 🟣TEST
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED 🟣TEST
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.HeightFieldShadowing=0; ⚫️DEF 0
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=2; ⚫️DEF 2
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED 🟣TEST
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Burley.BilateralFilterKernelFunctionType=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.Burley.Quality=1; ⚫️DEF 1 🟣TEST
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE 🟣TEST
r.Tonemapper.Sharpen=0.25; ⚫️DEF 2 ⚪️EDITED 🟣TEST
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24; ⚫️DEF 16 ⚪️EDITED 🟣TEST
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED

[ViewDistanceQuality@2]
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1; ⚫️DEF 1
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.SupportAllShaderPermutations=0; ⚫️DEF 0
r.SupportAnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportLowQualityLightmaps=0; ⚫️DEF 0
r.SupportMaterialLayers=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF ❓ 🟣TEST
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; ⚫️DEF 1
r.SkyAtmosphere.FastSkyLUT=1; ⚫️DEF 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟣TEST
r.AllowSimpleLights=1; ⚫️DEF 1 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟡req some light shadows 🟣TEST
r.Shadow.CachePreshadow=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWPOPrimitives=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🟣TEST
r.RayTracing=0; ⚫️DEF 0
r.EarlyZPass=2; ⚫️DEF 2
r.EarlyZPassMovable=1; ⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.EarlyZSortMasked=1; ⚫️DEF 1
au.SetAudioChannelCount=64; ⚫️DEF ❓ 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VSync=0; ⚫️DEF 0
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI 🟣TEST
r.DistanceFieldGI=0; ⚫️DEF ❓
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED 🟣TEST
r.DistanceFields=1; ⚫️DEF 1
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFields.AtlasSizeZ=1024; ⚫️DEF 1024
r.DistanceFields.AtlasSizeXY=512; ⚫️DEF 512
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.SkipPhysicsReplication=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=6; ⚫️DEF 3 ⚪️EDITED 🟣TEST
p.AnimDynamicsWind=1; ⚫️DEF 1
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
r.AOComputeShaderNormalCalculation=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED 🟣TEST
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GTSyncType=1; ⚫️DEF 1 🟣TEST
r.HZB.BuildUseCompute=1; ⚫️DEF 1 🟣TEST
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.StencilForLODDither=1; ⚫️DEF 1
r.StencilLODMode=2; ⚫️DEF 2
r.Emitter.FastPoolEnable=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
FX.AllowCulling=1; ⚫️DEF 1 🟣TEST
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=20; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
D3D12.UseUpdateTexture3DComputeShader=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE 🟣TEST
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03 🟣TEST
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01 🟣TEST
r.MinScreenRadiusForSmallLights=0.01; ⚫️DEF 0.01 🟣TEST
r.LightPropagationVolume=0; ⚫️DEF 0
r.PostProcessing.PreferCompute=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.CreateShadersOnLoad=0; ⚫️DEF 0 🟣TEST
r.ShaderPipelineCache.GameFileMaskEnabled=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.TextureStreaming=1; ⚫️DEF 1
r.MeshStreaming=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.PoolSize=1200; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟣TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=30; ⚫️DEF 0 🟣TEST
r.Streaming.MinBoost=0; ⚫️DEF 0
r.Streaming.Boost=1; ⚫️DEF 1
r.Streaming.HLODStrategy=0; ⚫️DEF 0
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟣TEST
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DensityScale=0.8; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=20; ⚫️DEF 30 ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.EyeAdaptation.MethodOverride=-1; ⚫️DEF -1
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.NormalMapsForStaticLighting=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ClearCoatNormal=0; ⚫️DEF 0
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.EmitterSpawnRateScale=1; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightCulling.Quality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightingDetailMode=100; ⚫️DEF 150 ⚪️EDITED 🟣TEST
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.LightShaftDownSampleFactor=2; ⚫️DEF 2
r.LightShaftFirstPassDistance=0.01; ⚫️DEF 0.1
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Upscale.Quality=2; ⚫️DEF 2
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟡for ScreenPercentage 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE 🟣TEST
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED 🟣TEST
r.AOGlobalDFResolution=128; ⚫️DEF 128 🟣TEST
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=0.6; ⚫️DEF 0.6 🟣TEST
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.85; ⚫️DEF 0.85 🟣TEST
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED 🟣TEST
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED 🟣TEST
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.HeightFieldShadowing=0; ⚫️DEF 0
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=2; ⚫️DEF 2
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED 🟣TEST
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Burley.BilateralFilterKernelFunctionType=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.Burley.Quality=1; ⚫️DEF 1 🟣TEST
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE 🟣TEST
r.Tonemapper.Sharpen=0.25; ⚫️DEF 2 ⚪️EDITED 🟣TEST
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24; ⚫️DEF 16 ⚪️EDITED 🟣TEST
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED

[PostProcessQuality@2]
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1; ⚫️DEF 1
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.SupportAllShaderPermutations=0; ⚫️DEF 0
r.SupportAnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportLowQualityLightmaps=0; ⚫️DEF 0
r.SupportMaterialLayers=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF ❓ 🟣TEST
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; ⚫️DEF 1
r.SkyAtmosphere.FastSkyLUT=1; ⚫️DEF 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟣TEST
r.AllowSimpleLights=1; ⚫️DEF 1 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟡req some light shadows 🟣TEST
r.Shadow.CachePreshadow=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWPOPrimitives=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🟣TEST
r.RayTracing=0; ⚫️DEF 0
r.EarlyZPass=2; ⚫️DEF 2
r.EarlyZPassMovable=1; ⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.EarlyZSortMasked=1; ⚫️DEF 1
au.SetAudioChannelCount=64; ⚫️DEF ❓ 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VSync=0; ⚫️DEF 0
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI 🟣TEST
r.DistanceFieldGI=0; ⚫️DEF ❓
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED 🟣TEST
r.DistanceFields=1; ⚫️DEF 1
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFields.AtlasSizeZ=1024; ⚫️DEF 1024
r.DistanceFields.AtlasSizeXY=512; ⚫️DEF 512
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.SkipPhysicsReplication=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=6; ⚫️DEF 3 ⚪️EDITED 🟣TEST
p.AnimDynamicsWind=1; ⚫️DEF 1
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
r.AOComputeShaderNormalCalculation=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED 🟣TEST
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GTSyncType=1; ⚫️DEF 1 🟣TEST
r.HZB.BuildUseCompute=1; ⚫️DEF 1 🟣TEST
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.StencilForLODDither=1; ⚫️DEF 1
r.StencilLODMode=2; ⚫️DEF 2
r.Emitter.FastPoolEnable=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
FX.AllowCulling=1; ⚫️DEF 1 🟣TEST
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=20; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
D3D12.UseUpdateTexture3DComputeShader=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE 🟣TEST
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03 🟣TEST
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01 🟣TEST
r.MinScreenRadiusForSmallLights=0.01; ⚫️DEF 0.01 🟣TEST
r.LightPropagationVolume=0; ⚫️DEF 0
r.PostProcessing.PreferCompute=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.CreateShadersOnLoad=0; ⚫️DEF 0 🟣TEST
r.ShaderPipelineCache.GameFileMaskEnabled=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.TextureStreaming=1; ⚫️DEF 1
r.MeshStreaming=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.PoolSize=1200; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟣TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=30; ⚫️DEF 0 🟣TEST
r.Streaming.MinBoost=0; ⚫️DEF 0
r.Streaming.Boost=1; ⚫️DEF 1
r.Streaming.HLODStrategy=0; ⚫️DEF 0
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟣TEST
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DensityScale=0.8; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=20; ⚫️DEF 30 ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.EyeAdaptation.MethodOverride=-1; ⚫️DEF -1
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.NormalMapsForStaticLighting=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ClearCoatNormal=0; ⚫️DEF 0
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.EmitterSpawnRateScale=1; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightCulling.Quality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightingDetailMode=100; ⚫️DEF 150 ⚪️EDITED 🟣TEST
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.LightShaftDownSampleFactor=2; ⚫️DEF 2
r.LightShaftFirstPassDistance=0.01; ⚫️DEF 0.1
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Upscale.Quality=2; ⚫️DEF 2
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟡for ScreenPercentage 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE 🟣TEST
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED 🟣TEST
r.AOGlobalDFResolution=128; ⚫️DEF 128 🟣TEST
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=0.6; ⚫️DEF 0.6 🟣TEST
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.85; ⚫️DEF 0.85 🟣TEST
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED 🟣TEST
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED 🟣TEST
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.HeightFieldShadowing=0; ⚫️DEF 0
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=2; ⚫️DEF 2
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED 🟣TEST
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Burley.BilateralFilterKernelFunctionType=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.Burley.Quality=1; ⚫️DEF 1 🟣TEST
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE 🟣TEST
r.Tonemapper.Sharpen=0.25; ⚫️DEF 2 ⚪️EDITED 🟣TEST
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24; ⚫️DEF 16 ⚪️EDITED 🟣TEST
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED

[TextureQuality@2]
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1; ⚫️DEF 1
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.SupportAllShaderPermutations=0; ⚫️DEF 0
r.SupportAnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportLowQualityLightmaps=0; ⚫️DEF 0
r.SupportMaterialLayers=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF ❓ 🟣TEST
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; ⚫️DEF 1
r.SkyAtmosphere.FastSkyLUT=1; ⚫️DEF 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟣TEST
r.AllowSimpleLights=1; ⚫️DEF 1 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟡req some light shadows 🟣TEST
r.Shadow.CachePreshadow=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWPOPrimitives=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🟣TEST
r.RayTracing=0; ⚫️DEF 0
r.EarlyZPass=2; ⚫️DEF 2
r.EarlyZPassMovable=1; ⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.EarlyZSortMasked=1; ⚫️DEF 1
au.SetAudioChannelCount=64; ⚫️DEF ❓ 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VSync=0; ⚫️DEF 0
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI 🟣TEST
r.DistanceFieldGI=0; ⚫️DEF ❓
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED 🟣TEST
r.DistanceFields=1; ⚫️DEF 1
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFields.AtlasSizeZ=1024; ⚫️DEF 1024
r.DistanceFields.AtlasSizeXY=512; ⚫️DEF 512
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.SkipPhysicsReplication=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=6; ⚫️DEF 3 ⚪️EDITED 🟣TEST
p.AnimDynamicsWind=1; ⚫️DEF 1
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
r.AOComputeShaderNormalCalculation=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED 🟣TEST
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GTSyncType=1; ⚫️DEF 1 🟣TEST
r.HZB.BuildUseCompute=1; ⚫️DEF 1 🟣TEST
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.StencilForLODDither=1; ⚫️DEF 1
r.StencilLODMode=2; ⚫️DEF 2
r.Emitter.FastPoolEnable=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
FX.AllowCulling=1; ⚫️DEF 1 🟣TEST
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=20; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
D3D12.UseUpdateTexture3DComputeShader=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE 🟣TEST
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03 🟣TEST
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01 🟣TEST
r.MinScreenRadiusForSmallLights=0.01; ⚫️DEF 0.01 🟣TEST
r.LightPropagationVolume=0; ⚫️DEF 0
r.PostProcessing.PreferCompute=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.CreateShadersOnLoad=0; ⚫️DEF 0 🟣TEST
r.ShaderPipelineCache.GameFileMaskEnabled=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.TextureStreaming=1; ⚫️DEF 1
r.MeshStreaming=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.PoolSize=1200; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟣TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=30; ⚫️DEF 0 🟣TEST
r.Streaming.MinBoost=0; ⚫️DEF 0
r.Streaming.Boost=1; ⚫️DEF 1
r.Streaming.HLODStrategy=0; ⚫️DEF 0
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟣TEST
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DensityScale=0.8; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=20; ⚫️DEF 30 ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.EyeAdaptation.MethodOverride=-1; ⚫️DEF -1
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.NormalMapsForStaticLighting=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ClearCoatNormal=0; ⚫️DEF 0
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.EmitterSpawnRateScale=1; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightCulling.Quality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightingDetailMode=100; ⚫️DEF 150 ⚪️EDITED 🟣TEST
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.LightShaftDownSampleFactor=2; ⚫️DEF 2
r.LightShaftFirstPassDistance=0.01; ⚫️DEF 0.1
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Upscale.Quality=2; ⚫️DEF 2
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟡for ScreenPercentage 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE 🟣TEST
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED 🟣TEST
r.AOGlobalDFResolution=128; ⚫️DEF 128 🟣TEST
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=0.6; ⚫️DEF 0.6 🟣TEST
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.85; ⚫️DEF 0.85 🟣TEST
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED 🟣TEST
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED 🟣TEST
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.HeightFieldShadowing=0; ⚫️DEF 0
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=2; ⚫️DEF 2
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED 🟣TEST
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Burley.BilateralFilterKernelFunctionType=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.Burley.Quality=1; ⚫️DEF 1 🟣TEST
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE 🟣TEST
r.Tonemapper.Sharpen=0.25; ⚫️DEF 2 ⚪️EDITED 🟣TEST
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24; ⚫️DEF 16 ⚪️EDITED 🟣TEST
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED

[EffectsQuality@2]
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1; ⚫️DEF 1
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.SupportAllShaderPermutations=0; ⚫️DEF 0
r.SupportAnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportLowQualityLightmaps=0; ⚫️DEF 0
r.SupportMaterialLayers=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF ❓ 🟣TEST
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; ⚫️DEF 1
r.SkyAtmosphere.FastSkyLUT=1; ⚫️DEF 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟣TEST
r.AllowSimpleLights=1; ⚫️DEF 1 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟡req some light shadows 🟣TEST
r.Shadow.CachePreshadow=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWPOPrimitives=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🟣TEST
r.RayTracing=0; ⚫️DEF 0
r.EarlyZPass=2; ⚫️DEF 2
r.EarlyZPassMovable=1; ⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.EarlyZSortMasked=1; ⚫️DEF 1
au.SetAudioChannelCount=64; ⚫️DEF ❓ 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VSync=0; ⚫️DEF 0
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI 🟣TEST
r.DistanceFieldGI=0; ⚫️DEF ❓
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED 🟣TEST
r.DistanceFields=1; ⚫️DEF 1
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFields.AtlasSizeZ=1024; ⚫️DEF 1024
r.DistanceFields.AtlasSizeXY=512; ⚫️DEF 512
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.SkipPhysicsReplication=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=6; ⚫️DEF 3 ⚪️EDITED 🟣TEST
p.AnimDynamicsWind=1; ⚫️DEF 1
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
r.AOComputeShaderNormalCalculation=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED 🟣TEST
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GTSyncType=1; ⚫️DEF 1 🟣TEST
r.HZB.BuildUseCompute=1; ⚫️DEF 1 🟣TEST
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.StencilForLODDither=1; ⚫️DEF 1
r.StencilLODMode=2; ⚫️DEF 2
r.Emitter.FastPoolEnable=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
FX.AllowCulling=1; ⚫️DEF 1 🟣TEST
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=20; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
D3D12.UseUpdateTexture3DComputeShader=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE 🟣TEST
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03 🟣TEST
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01 🟣TEST
r.MinScreenRadiusForSmallLights=0.01; ⚫️DEF 0.01 🟣TEST
r.LightPropagationVolume=0; ⚫️DEF 0
r.PostProcessing.PreferCompute=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.CreateShadersOnLoad=0; ⚫️DEF 0 🟣TEST
r.ShaderPipelineCache.GameFileMaskEnabled=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.TextureStreaming=1; ⚫️DEF 1
r.MeshStreaming=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.PoolSize=1200; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟣TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=30; ⚫️DEF 0 🟣TEST
r.Streaming.MinBoost=0; ⚫️DEF 0
r.Streaming.Boost=1; ⚫️DEF 1
r.Streaming.HLODStrategy=0; ⚫️DEF 0
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟣TEST
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DensityScale=0.8; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=20; ⚫️DEF 30 ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.EyeAdaptation.MethodOverride=-1; ⚫️DEF -1
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.NormalMapsForStaticLighting=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ClearCoatNormal=0; ⚫️DEF 0
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.EmitterSpawnRateScale=1; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightCulling.Quality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightingDetailMode=100; ⚫️DEF 150 ⚪️EDITED 🟣TEST
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.LightShaftDownSampleFactor=2; ⚫️DEF 2
r.LightShaftFirstPassDistance=0.01; ⚫️DEF 0.1
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Upscale.Quality=2; ⚫️DEF 2
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟡for ScreenPercentage 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE 🟣TEST
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED 🟣TEST
r.AOGlobalDFResolution=128; ⚫️DEF 128 🟣TEST
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=0.6; ⚫️DEF 0.6 🟣TEST
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.85; ⚫️DEF 0.85 🟣TEST
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED 🟣TEST
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED 🟣TEST
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.HeightFieldShadowing=0; ⚫️DEF 0
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=2; ⚫️DEF 2
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED 🟣TEST
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Burley.BilateralFilterKernelFunctionType=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.Burley.Quality=1; ⚫️DEF 1 🟣TEST
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE 🟣TEST
r.Tonemapper.Sharpen=0.25; ⚫️DEF 2 ⚪️EDITED 🟣TEST
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24; ⚫️DEF 16 ⚪️EDITED 🟣TEST
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED

[FoliageQuality@2]
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1; ⚫️DEF 1
r.DefaultFeature.Bloom=1; ⚫️DEF 1
r.DefaultFeature.LensFlare=1; ⚫️DEF 1
r.DefaultFeature.MotionBlur=0; ⚫️DEF 0
r.SupportAllShaderPermutations=0; ⚫️DEF 0
r.SupportAnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportLowQualityLightmaps=0; ⚫️DEF 0
r.SupportMaterialLayers=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SupportSkyAtmosphereAffectsHeightFog=1; ⚫️DEF ❓ 🟣TEST
r.SkyAtmosphere=1; ⚫️DEF 1
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; ⚫️DEF 1
r.SkyAtmosphere.FastSkyLUT=1; ⚫️DEF 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; ⚫️DEF 0
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟣TEST
r.AllowSimpleLights=1; ⚫️DEF 1 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF 1 🟢0 for PERFORMANCE 🟡req some light shadows 🟣TEST
r.Shadow.CachePreshadow=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWholeSceneShadows=1; ⚫️DEF 1 🟣TEST
r.Shadow.CacheWPOPrimitives=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED 🟣TEST
r.RayTracing=0; ⚫️DEF 0
r.EarlyZPass=2; ⚫️DEF 2
r.EarlyZPassMovable=1; ⚫️DEF 1
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.EarlyZSortMasked=1; ⚫️DEF 1
au.SetAudioChannelCount=64; ⚫️DEF ❓ 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VSync=0; ⚫️DEF 0
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI 🟣TEST
r.DistanceFieldGI=0; ⚫️DEF ❓
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED 🟣TEST
r.DistanceFields=1; ⚫️DEF 1
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFields.AtlasSizeZ=1024; ⚫️DEF 1024
r.DistanceFields.AtlasSizeXY=512; ⚫️DEF 512
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.SkipPhysicsReplication=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=6; ⚫️DEF 3 ⚪️EDITED 🟣TEST
p.AnimDynamicsWind=1; ⚫️DEF 1
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
r.AOComputeShaderNormalCalculation=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED 🟣TEST
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GTSyncType=1; ⚫️DEF 1 🟣TEST
r.HZB.BuildUseCompute=1; ⚫️DEF 1 🟣TEST
r.HZBOcclusion=0; ⚫️DEF ❓ 🟣TEST
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.StencilForLODDither=1; ⚫️DEF 1
r.StencilLODMode=2; ⚫️DEF 2
r.Emitter.FastPoolEnable=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
FX.AllowCulling=1; ⚫️DEF 1 🟣TEST
FX.AllowGPUParticles=1; ⚫️DEF 1
FX.AllowGPUSorting=1; ⚫️DEF 1
FX.FXAllowParticleMeshLODs=1; ⚫️DEF 0 ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=20; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
FX.ParticleSystemPool.Enable=1; ⚫️DEF 1
D3D12.UseUpdateTexture3DComputeShader=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MorphTarget.Mode=1; ⚫️DEF 1
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE 🟣TEST
r.MinScreenRadiusForDepthPrepass=0.03; ⚫️DEF 0.03 🟣TEST
r.MinScreenRadiusForCSMDepth=0.01; ⚫️DEF 0.01 🟣TEST
r.MinScreenRadiusForSmallLights=0.01; ⚫️DEF 0.01 🟣TEST
r.LightPropagationVolume=0; ⚫️DEF 0
r.PostProcessing.PreferCompute=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.CreateShadersOnLoad=0; ⚫️DEF 0 🟣TEST
r.ShaderPipelineCache.GameFileMaskEnabled=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DiscardUnusedQuality=0; ⚫️DEF 0
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.TextureStreaming=1; ⚫️DEF 1
r.MeshStreaming=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.Streaming.LimitPoolSizeToVRAM=1; ⚫️DEF 1
r.Streaming.PoolSize=1200; ⚫️DEF 2000
r.Streaming.PoolSizeForMeshes=-1; ⚫️DEF -1
r.Streaming.MipBias=0; ⚫️DEF 0
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟣TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=30; ⚫️DEF 0 🟣TEST
r.Streaming.MinBoost=0; ⚫️DEF 0
r.Streaming.Boost=1; ⚫️DEF 1
r.Streaming.HLODStrategy=0; ⚫️DEF 0
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟣TEST
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DensityScale=0.8; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinimumScreenSize=0.0001; ⚫️DEF 0.0001
foliage.MinVertsToSplitNode=8192; ⚫️DEF 8192
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.8; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=20; ⚫️DEF 30 ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=5; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.EyeAdaptation.MethodOverride=-1; ⚫️DEF -1
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Filter.SizeScale=0.8; ⚫️DEF 0.8
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.NormalMapsForStaticLighting=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ClearCoatNormal=0; ⚫️DEF 0
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AnisotropicMaterials=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.EmitterSpawnRateScale=1; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightCulling.Quality=1; ⚫️DEF 1
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightingDetailMode=100; ⚫️DEF 150 ⚪️EDITED 🟣TEST
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.LightShaftDownSampleFactor=2; ⚫️DEF 2
r.LightShaftFirstPassDistance=0.01; ⚫️DEF 0.1
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Upscale.Quality=2; ⚫️DEF 2
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟡for ScreenPercentage 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE 🟣TEST
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED 🟣TEST
r.AOGlobalDFResolution=128; ⚫️DEF 128 🟣TEST
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=0.6; ⚫️DEF 0.6 🟣TEST
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.85; ⚫️DEF 0.85 🟣TEST
r.Shadow.FilterMethod=0; ⚫️DEF 0
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED 🟣TEST
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED 🟣TEST
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.HeightFieldShadowing=0; ⚫️DEF 0
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSGI.Quality=2; ⚫️DEF 2
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED 🟣TEST
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSS.Burley.BilateralFilterKernelFunctionType=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.Burley.Quality=1; ⚫️DEF 1 🟣TEST
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=-1; ⚫️DEF -1 🟢0 for PERFORMANCE 🟣TEST
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE 🟣TEST
r.Tonemapper.Sharpen=0.25; ⚫️DEF 2 ⚪️EDITED 🟣TEST
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=24; ⚫️DEF 16 ⚪️EDITED 🟣TEST
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
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
bDepthOfField=
bMotionBlur=
bBounceLightEnabled=
bFlashlightShadowsEnabled=
AmbientOcclusion=(Value=1)
AntiAliasingMode=(Value=2)
AudioQualityLevel=3
bRTXAmbientOcclusionEnabled=
bRTXEnabled=
bRTXReflectionsEnabled=
bRTXShadowsEnabled=
bTelemetryEnabled=0
bUseDynamicResolution=0
bUseVSync=0
ContactShadows=(Value=0)
ContactShadows=0
DetailMode=(Value=)
DFAO=
DistanceFieldShadows=1
DlssQualitySetting=
DoubleKeyPressTime=0.1
FoliageMinLOD=(Value=0)
FullscreenMode=0
Gamma=2.2
GlobalSensitivity=0.183
GraphicsQuality=0
GraphicsPresetIndex=0
HDRDisplayOutputNits=
HZBOcclusion=(Value=)
MaxAnisotropy=(Value=)
MaxAnisotropy=8
bFrameLimitEnabled=
FrameRateLimit=
MaxFPS=
MenuFrameRateLimit=
OceanQuality=(Value=0)
OverrideOptions=(("r.9000FPS",(Value=1,bModified=True)),("r.OPTIMIZE",(Value=1,bModified=False)));
PostFX_Saturation=1.2
PostFX_Sharpness=0.25;      <- needed for squid to set tonemappersharp correctly
ResolutionScaleModifier=
ScreenPercentage=(Value=70)
SkeletalMeshLODBias=(Value=0)
TAASampleStorage=2
LastSavedAASamples=2
TemporalAASamples=(Value=2);   <- needed for squid to set to 2
Tessellation=(Value=0)
TessellationMode=(Value=9999999)
TextureStreamPoolSizeStorage=(Value=)
WakeSim=(Value=0)
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
InitialButtonRepeatDelay=0.2; ⚫️DEF 0.2
ButtonRepeatDelay=0.1; ⚫️DEF 0.1
DoubleClickTime=0.1; ⚫️DEF 0.25
```

---

#### AO options with my config

```python
dfao:
r.AmbientOcclusionLevels=0; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED

ssao med:
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED

ssao low:
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED 🟣TEST
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED

or both
```

---

<details><summary>Open DeviceProfiles.ini for textures lods, skip this and just use the games texture settings imo</summary>
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
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=1,MaxLODSize=256,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=9,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=1,MaxLODSize=256,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=9,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=3,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=11,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,MinLODSize=1,MaxLODSize=256,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=9,MipGenSettings=TMGS_SimpleAverage)
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
