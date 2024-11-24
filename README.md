#### updated 11/24/2024 ✂️ 📋 :ramen: v1.200.02
---
#### for UE4 and UE5* games for reference/customization/optimization/learning
---
#### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)
---
#### my config are trying to be quality and perform well for any UE4/5 game, it might not be perfectly optimal for a specific game
---
#### you will have to adjust settings most likely per game
---
#### [Installing and optimizing nvidia drivers here](https://github.com/smo0ths/Installing-and-optimizing-new-nvidia-drivers-on-windows-11-gaming-PC)
---
#### 2560x1440 (~2k) use 58%(balance) 67%(quality) 70%(custom/TAAU) scaling for PERFORMANCE (higher if cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR)
#### 3328x1872 (3.25K) use 50%(performance/TAAU) scaling for PERFORMANCE (higher if cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR)
#### 3840x2160 (~4K UHD) use 33%(ultra performance) 50%(performance/TAAU) scaling for PERFORMANCE (higher if cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR)
#### negative LOD bias -1/-0.6 or 0 for PERFORMANCE (0 is best on proper mipmaps/textures) (set by nvidiaProfileInspector)
#### sg.ResolutionQuality=70; r.ScreenPercentage=70; r.ScreenPercentage.Default=70; r.SecondaryScreenPercentage.GameViewport=83.33; can help by forcing scaling on some games
#### check 🟢 options for more fps
---
#### Open Engine.ini and copy pasta %localappdata%
#### or UnrealPak method (pakchunk9999-Mods_CustomMod_P\Engine\Config\Windows\WindowsEngine.ini)
#### High config (works with UE5*)
---
#### Turn these off (0) in most games for performance unless its default in the project (game)
#### r.Lumen.DiffuseIndirect.Allow=0; 🔵 UE5 🔵 lumen global illumination
#### r.Lumen.Reflections.Allow=0; 🔵 UE5 🔵 lumen reflections
---

```python
[Core.Log]
Global=off;

[Audio]
bEnableBinauralRendering=1;
bEnableHRTF=1;
CommonAudioPoolSize=0; 🟡 def 0
MaxChannels=0; 🟡 def 0
UseAudioThread=1;

[/Script/Engine.Engine]
bPauseOnLossOfFocus=0;
bSmoothFrameRate=0;
bUseFixedFrameRate=0;

[TextureStreaming]
PoolSizeVRAMPercentage=90; ⚪️ EDITED 🟡 def 70 🔵 50 to lower vram usage 🔵 texturepool cache

[ConsoleVariables]
au.RenderThreadPriority=3; 🟡 def 3
Compat.UseDXT5NormalMaps=0; 🟡 def 3
D3D12.PSOPrecache.KeepLowLevel=0; 🟡 def 0 🔵 UE5
foliage.DensityScale=1; 🟢 0.6 for PERFORMANCE 🟡 def 1
foliage.DitheredLOD=1; 🟡 def 1
foliage.LODDistanceScale=1; 🟡 def 1
foliage.MinimumScreenSize=0.0001; ⚪️ EDITED
fx.Budget.Enabled=1; 🔵 experimental
fx.Niagara.QualityLevel=2; 🔵 0,1,2,3,4 low,med,high,ultra,cine
fx.Niagara.UseGlobalFXBudget=1; 🔵 experimental
fx.NiagaraAllowRuntimeScalabilityChanges=1;
grass.CullDistanceScale=1; 🟡 def 1
grass.DensityScale=0.8; 🟢 0.6 for PERFORMANCE
grass.DisableDynamicShadows=0; 🟢 1 for PERFORMANCE 🟡 def 0
grass.MaxAsyncTasks=4; 🟡 def 4
grass.MaxCreatePerFrame=1; 🟡 def 1
grass.MaxUpdateFrequency=1; ⚪️ EDITED
grass.TickInterval=10; ⚪️ EDITED
p.AnimDynamics=1; 🟢 0 for PERFORMANCE 🟡 def 1
p.AnimDynamicsWind=1; 🟢 0 for PERFORMANCE 🟡 def 1
p.ClothPhysics=1; 🟡 def 1
p.RigidBodyNode=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.AllowGlobalClipPlane=0; 🟢 0 for PERFORMANCE 🟡 def 0
r.AllowLandscapeShadows=1; 🟢 0 for PERFORMANCE
r.AllowSimpleLights=1; 🟢 0 for PERFORMANCE
r.AmbientOcclusion.Denoiser=1; 🟢 1 for PERFORMANCE ⚪️ EDITED 🟡 def 2 🔵 denoiser
r.AmbientOcclusion.Method=0; 🔵 SSAO,GTAO
r.AmbientOcclusionLevels=2; 🟢 0,1 for PERFORMANCE 🟡 def -1
r.AmbientOcclusionMaxQuality=100; 🟡 def 100
r.AmbientOcclusionMipLevelFactor=0.5; 🟡 def 0.5
r.AmbientOcclusionRadiusScale=1;
r.AmbientOcclusionStaticFraction=-1; 🟢 0 for PERFORMANCE 🟡 def -1
r.AnisotropicMaterials=1; 🟢 0 for PERFORMANCE 🔵 0,1 low,med
r.AOApplyToStaticIndirect=0; 🟡 def 0
r.AOGlobalDistanceField.MipFactor=4; 🟢 8 for PERFORMANCE ⚪️ EDITED 🟡 def 4
r.AOGlobalDistanceField=1; 🟡 def 1 🔵 adaptive method
r.AOQuality=0; 🟢 0,1 for PERFORMANCE 🔵 req distancefieldao
r.Bloom.Cross=0; 🟡 def 0
r.BloomQuality=4; 🟢 0 for PERFORMANCE ⚪️ EDITED
r.BlurGBuffer=0; ⚪️ EDITED
r.CapsuleDirectShadows=1; 🟡 def 1
r.CapsuleIndirectShadows=1; 🟡 def 1
r.CapsuleShadows=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.CapsuleShadowsFullResolution=0; 🟡 def 0
r.chaos.ReflectionCaptureStaticSceneOnly=1; 🟡 def 1
r.ClearCoatNormal=0; 🟡 def 0
r.CompileShadersForDevelopment=1; 🟢 1 for PERFORMANCE 🟡 def 1
r.ContactShadows.OverrideLength=-1; 🟡 def -1
r.ContactShadows=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.D3D11.UseAllowTearing=1; 🟡 dxgi flip mode 🟡 def 1
r.D3D12.GPUCrashDebuggingMode=0; 🟡 debug
r.D3D12.UseAllowTearing=1; 🟡 dxgi flip mode 🟡 def 1
r.DefaultFeature.AmbientOcclusion=1;
r.DefaultFeature.AutoExposure.Method=0; 🟡 def 0 🔵 eyeadaptation,autoexposure
r.DefaultFeature.AutoExposure=1; 🟡 def 1 🔵 eyeadaptation,autoexposure
r.DefaultFeature.MotionBlur=0; ⚪️ EDITED
r.DepthOfFieldQuality=1; 🟢 0,1 for PERFORMANCE
r.DetailMode=1; 🟢 0,1 for PERFORMANCE ⚪️ EDITED 🟡 def 3 🔵 0,1,2,3 low,med,high,epic
r.DFFullResolution=0; 🟢 0 for PERFORMANCE 🟡 def 0
r.DFShadowQuality=3; 🟢 0,1,2 for PERFORMANCE 🟡 def 3 🔵 req distancefieldshadowing
r.DFShadowScatterTileCulling=1; 🟢 1 for PERFORMANCE 🟡 def 1
r.DiffuseIndirect.Denoiser=1; 🟢 1 for PERFORMANCE 🟡 def 1 🔵 denoiser
r.DistanceFieldAO=0; 🟢 0 for PERFORMANCE 🔵 req generatemeshdistancefields
r.DistanceFields.AtlasSizeXY=512;
r.DistanceFields.AtlasSizeZ=1024;
r.DistanceFields.ForceMaxAtlasSize=1; ⚪️ EDITED
r.DistanceFields.MaxPerMeshResolution=128; 🟢 128 for PERFORMANCE ⚪️ EDITED 🟡 def 256
r.DistanceFieldShadowing=1; 🟢 0 for PERFORMANCE 🔵 req generatemeshdistancefields
r.DOF.Gather.AccumulatorQuality=0; ⚪️ EDITED 🟡 def 1
r.DOF.Gather.EnableBokehSettings=0; ⚪️ EDITED 🟡 def 1
r.DOF.Gather.PostfilterMethod=0; ⚪️ EDITED 🟡 def 1
r.DOF.Gather.RingCount=3; ⚪️ EDITED 🟡 def 5
r.DOF.Kernel.MaxBackgroundRadius=0.012; ⚪️ EDITED 🟡 def 0.025
r.DOF.Kernel.MaxForegroundRadius=0.012; ⚪️ EDITED 🟡 def 0.025
r.DOF.Recombine.Quality=0; ⚪️ EDITED 🟡 def 2
r.DOF.Scatter.BackgroundCompositing=1; ⚪️ EDITED 🟡 def 2
r.DOF.Scatter.EnableBokehSettings=0; ⚪️ EDITED 🟡 def 1
r.DOF.Scatter.ForegroundCompositing=1; 🟡 def 1
r.DOF.Scatter.MaxSpriteRatio=0.04; 🟡 def 0.1
r.DOF.TemporalAAQuality=0; ⚪️ EDITED 🟡 def 1
r.DynamicRes.OperationMode=0;
r.EmitterSpawnRateScale=1; 🟢 0.125,0.25 for PERFORMANCE 🟡 def 1
r.EnableCameraAndMeshMotionBlur=0;
r.EyeAdaptation.Basic.Compute=1; 🟡 def 1 🔵 eyeadaptation,autoexposure
r.EyeAdaptation.MethodOverride=-1; 🟡 def -1 🔵 eyeadaptation,autoexposure
r.EyeAdaptation.PreExposureOverride=0; 🟡 def 0 🔵 eyeadaptation,autoexposure
r.EyeAdaptationQuality=2; 🟡 def 2 🟢 1 for PERFORMANCE 🔵 eyeadaptation,autoexposure
r.FilmGrain=0;
r.Filter.SizeScale=1; 🟡 def 1
r.FinishCurrentFrame=0;
r.GenerateLandscapeGIData=0; 🟢 0 for PERFORMANCE 🔵 req generatemeshdistancefields
r.GenerateMeshDistanceFields=1; 🟢 0 for PERFORMANCE 🔵 dfs and dfao mesh
r.gpucrash.collectionenable=0; 🟡 debug
r.GPUCrashDebugging=0; 🟡 debug
r.GTSyncType=0; 🟡 Sync
r.HairStrands.Enable=1; 🟢 0 for PERFORMANCE
r.HeightfieldGlobalIllumination=0; 🟢 0 for PERFORMANCE
r.HeightFieldShadowing=0; 🟢 0 for PERFORMANCE
r.HFShadowQuality=0; 🟢 0,1 for PERFORMANCE 🟡 def 2 🔵 req heightfieldshadowing
r.HLOD.DistanceScale=0.8;
r.HLOD.ForceDisableCastDynamicShadow=0; 🟡 def 0
r.HZBOcclusion=1; 🟢 test 0 per game 🟡 def 1
r.IrisNormal=0; 🟡 def 0
r.LandscapeLODBias=0; 🟢 1 for PERFORMANCE
r.LensFlareQuality=2; 🟢 0,1 for PERFORMANCE
r.LightFunctionQuality=2; 🟢 0,1 for PERFORMANCE 🟡 def 2
r.LightMaxDrawDistanceScale=1; 🟢 0.5,0.6 for PERFORMANCE
r.LightShaftBlurPasses=2; ⚪️ EDITED 🟡 def 3
r.LightShaftDownSampleFactor=2; 🟡 def 2
r.LightShaftFirstPassDistance=0.08; ⚪️ EDITED 🟡 def 0.1
r.LightShaftQuality=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Lumen.DiffuseIndirect.Allow=1; 🔵 UE5 🔵 lumen global illumination
r.Lumen.HardwareRayTracing=1; ⚪️ EDITED 🟡 def 0 🔵 UE5
r.Lumen.Reflections.Allow=1; 🔵 UE5 🔵 lumen reflections
r.Lumen.Reflections.BilateralFilter=1; 🟡 def 1 🔵 UE5 🔵 denoiser
r.Lumen.Reflections.HardwareRayTracing=1; ⚪️ EDITED 🟡 def 1 🔵 UE5
r.Lumen.Reflections.ScreenSpaceReconstruction.NumSamples=5; 🟡 def 5 🔵 UE5
r.Lumen.Reflections.ScreenSpaceReconstruction=1; 🟡 def 1 🔵 UE5
r.Lumen.Reflections.ScreenTraces=1; 🟢 0 for PERFORMANCE 🟡 def 1 🔵 UE5
r.Lumen.Reflections.Temporal=1; 🟡 def 1 🔵 UE5
r.MaterialQualityLevel=1; 🟢 0,2 for PERFORMANCE 🔵 0,1,2,3 low,high,med,epic
r.MaxAnisotropy=16; 🟢 0,4,8 for PERFORMANCE
r.MinRoughnessOverride=0; 🟡 def 0
r.MinScreenRadiusForCSMDepth=0.01; 🟡 def 0.01
r.MinScreenRadiusForDepthPrepass=0.03; 🟡 def 0.03
r.MinScreenRadiusForLights=0.03; 🟢 0.04,0.06 for PERFORMANCE 🟡 def 0.03
r.MipMapLODBias=0; 🟡 def 0
r.MotionBlurQuality=0; ⚪️ EDITED
r.Nanite=1; 🔵 UE5
r.NGX.DLSS.AutoExposure=0; 🟡 def 1 🔵 eyeadaptation,autoexposure
r.NGX.DLSS.DenoiserMode=0; 🟡 def 0 🔵 UE5
r.NGX.DLSS.DilateMotionVectors=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.NGX.DLSS.PreferNISSharpen=0; ⚪️ EDITED 🟡 def 1
r.NGX.DLSS.Quality.Auto=0; 🟢 0 for PERFORMANCE
r.NGX.DLSS.Quality=1; ⚪️ EDITED 🔵 -2,-1,0,1,2 ultra perf,perf,balanced,quality,ultra
r.NGX.DLSS.Reflections.TemporalAA=0; 🔵 TAA pass on the denoised reflections
r.NGX.DLSS.Sharpness=0; 🟡 def 0
r.NGX.DLSS.WaterReflections.TemporalAA=0; 🔵 TAA pass on the denoised water reflections
r.NGX.LogLevel=0; ⚪️ EDITED 🟡 def 1 🔵 debug
r.NIS.Enable=0; 🔵 nvidia image scaling
r.OneFrameThreadLag=1; 🟢 1 for PERFORMANCE
r.ParallelShadow=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.ParallelShadowsNonWholeScene=0; 🟡 def 0
r.ParallelTranslucency=1; 🟡 def 1
r.ParticleLightQuality=2; 🟢 0,1 for PERFORMANCE 🟡 def 2
r.PostProcessAAQuality=6; ⚪️ EDITED 🟡 def 4 🟣 0 off 1,2 FXAA 3,4,5,6 TAA
r.PSOWarmup.WarmupMaterials=1; 🔵 after compiling shaders once set 0 for faster loading
r.Reflections.Denoiser.TemporalAccumulation=0; ⚪️ EDITED 🟡 def 1 🔵 denoiser
r.Reflections.Denoiser=0; 🟢 0 for PERFORMANCE ⚪️ EDITED 🟡 def 2 🔵 denoiser
r.RefractionQuality=2; 🟢 0 for PERFORMANCE 🟡 def 2
r.RenderTargetPoolMin=400; 🟡 def 400
r.SceneColorFormat=3; 🟢 2,3 for PERFORMANCE ⚪️ EDITED 🟡 def 4
r.SceneColorFringe.Max=0; ⚪️ EDITED
r.SceneColorFringeQuality=1;
r.ScreenPercentage.Default=100; 🟡 def 100
r.ScreenPercentage=0; 🟡 def 0
r.SecondaryScreenPercentage.GameViewport=0; 🟡 def 0
r.ShaderDevelopmentMode=0; 🟡 def 0 🟡 debug
r.Shadow.CachedShadowsCastFromMovablePrimitives=1; 🟢 0 for PERFORMANCE 🟡 def 1 🔵 movable light shadows
r.Shadow.CacheWholeSceneShadows=1; 🟡 def 1
r.Shadow.CacheWPOPrimitives=0; 🟡 def 0
r.Shadow.CSM.MaxCascades=2; 🟢 1,2 for PERFORMANCE 🟡 def 10
r.Shadow.CSM.TransitionScale=1; ⚪️ EDITED
r.Shadow.Denoiser.MaxBatchSize=8; ⚪️ EDITED 🟡 def 4 🔵 denoiser
r.Shadow.Denoiser=0; 🟡 def 0 🔵 denoiser
r.Shadow.DistanceScale=0.85;
r.Shadow.FilterMethod=0; 🟢 0 for PERFORMANCE 🔵 pcss shadows
r.Shadow.ForceSingleSampleShadowingFromStationary=0; 🟢 1 for PERFORMANCE 🔵 def 0
r.Shadow.MaxCSMResolution=2048; 🟢 512,1024 for PERFORMANCE
r.Shadow.MaxNumFarShadowCascades=4; ⚪️ EDITED 🟡 def 10
r.Shadow.MaxResolution=512; 🟢 512,1024 for PERFORMANCE
r.Shadow.PreShadowResolutionFactor=0.5; 🟡 def 0.5
r.Shadow.RadiusThreshold=0.06; 🟢 0.04,0.05,0.06 for PERFORMANCE
r.Shadow.Virtual.Cache.MaxMaterialPositionInvalidationRange=0; 🔵 UE5
r.Shadow.Virtual.Cache.StaticSeparate=1; 🟡 def 1 🔵 UE5
r.Shadow.Virtual.Cache=1; 🟡 def 1 🔵 UE5
r.Shadow.Virtual.Enable=0; 🔵 UE5
r.Shadow.Virtual.ForceOnlyVirtualShadowMaps=1; 🟡 def 1 🔵 UE5
r.Shadow.Virtual.NonNanite.IncludeInCoarsePages=0; 🔵 UE5
r.Shadow.Virtual.OnePassProjection.MaxLightsPerPixel=16; 🟡 def 16 🔵 UE5
r.Shadow.Virtual.OnePassProjection=1; 🟡 def 1 🔵 UE5
r.ShadowQuality=5; 🟢 3,4 for PERFORMANCE 🟡 def 5
r.SkeletalMeshLODBias=0; 🟢 1 for PERFORMANCE 🔵 0,1,2 high,med,low
r.SkipDrawOnPSOPrecaching=0; 🟡 def 0 🔵 UE5
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; 🟡 def 1
r.SkyAtmosphere.DistantSkyLightLUT=1; 🟡 def 1
r.SkyAtmosphere.FastSkyLUT=0; ⚪️ EDITED 🟡 def 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0;
r.SkyAtmosphere.SampleLightShadowmap=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.SkyLight.RealTimeReflectionCapture=1; 🟢 0 for PERFORMANCE
r.SSGI.Enable=0; 🟢 0 for PERFORMANCE
r.SSGI.HalfRes=1; 🟢 1 for PERFORMANCE ⚪️ EDITED
r.SSGI.LeakFreeReprojection=1; 🟡 def 1
r.SSGI.Quality=0; 🟢 0,2 for PERFORMANCE ⚪️ EDITED 🔵 req ssgi enable
r.SSR.ExperimentalDenoiser=0; 🟡 def 0 🔵 denoiser
r.SSR.HalfResSceneColor=1; 🟢 1 for PERFORMANCE ⚪️ EDITED 🟡 def 0
r.SSR.MaxRoughness=-1; 🟡 def -1
r.SSR.Quality=3; 🟢 0,2 for PERFORMANCE 🔵 EDITED 🟡 def 3
r.SSR.Temporal=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.SSS.Checkerboard=1; 🟢 1 for PERFORMANCE ⚪️ EDITED 🟡 def 2
r.SSS.HalfRes=1; 🟡 def 1
r.SSS.Quality=0; 🟡 def 0
r.SSS.SampleSet=0; 🟡 def 0
r.SSS.Scale=1; 🟡 def 1
r.Streaming.AmortizeCPUToGPUCopy=0; 🟡 def 0
r.Streaming.Boost=1; 🟡 def 1
r.Streaming.FramesForFullUpdate=5; 🟡 def 5
r.Streaming.HiddenPrimitiveScale=0.5; 🟢 0.5 for PERFORMANCE 🟡 def 0.5
r.Streaming.LimitPoolSizeToVRAM=0; 🟡 def 0
r.Streaming.MaxEffectiveScreenSize=0; 🟡 def 0
r.Streaming.MaxNumTexturesToStreamPerFrame=0; 🟡 def 0
r.Streaming.MipBias=0; 🟢 1 for PERFORMANCE 🟡 def 0
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.PoolSize=-1; 🟡 def -1
r.Streaming.PoolSizeForMeshes=-1; 🟡 def -1
r.Streaming.UseFixedPoolSize=0; 🟡 def 0
r.Streaming.UseMaterialData=1; 🟡 def 1
r.Streaming.UseNewMetrics=1; 🟡 def 1
r.SubsurfaceScattering=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.SupportMaterialLayers=1; 🟢 0 for PERFORMANCE
r.TemporalAA.Algorithm=1; 🟢 0 for PERFORMANCE 🟣 0,1 gen4,gen5 TAAU
r.TemporalAA.HistoryScreenPercentage=100; 🟡 def 100
r.TemporalAA.R11G11B10History=1; 🟡 def 1
r.TemporalAA.Upsampling=1; 🟡 def 1 🔵 TAAU
r.TemporalAACurrentFrameWeight=0.03; ⚪️ EDITED 🟡 def 0.04
r.TemporalAAFilterSize=1; 🟡 def 1 🔵 req gen5 TAAU
r.TemporalAASamples=8; 🟡 def 8
r.TessellationAdaptivePixelsPerTriangle=999999; 🟢 999999 for PERFORMANCE ⚪️ EDITED 🟡 def 48
r.TiledDeferredShading=1; 🟢 0 for PERFORMANCE 🔵 gpu lights
r.Tonemapper.GrainQuantization=0; ⚪️ EDITED 🟡 def 1
r.Tonemapper.Quality=2; ⚪️ EDITED 🟡 def 5
r.Tonemapper.Sharpen=-1; 🟡 def -1
r.TranslucencyLightingVolumeDim=48; 🟢 32,48 for PERFORMANCE ⚪️ EDITED 🟡 def 64
r.TranslucencyVolumeBlur=1; 🟢 0 for PERFORMANCE
r.UniformBufferPooling=1; 🔵 debug
r.Upscale.Quality=3; 🟡 def 3
r.UseClusteredDeferredShading=0; 🟡 def 0 🔵 UE5 🔵 with Shadow.Virtual.OnePassProjection
r.UsePreExposure=1; 🟡 def 1 🔵 eyeadaptation,autoexposure
r.ViewDistanceScale=0.8; 🟢 0.8 for PERFORMANCE
r.VolumetricCloud.DisableCompute=0; 🟡 def 0
r.VolumetricCloud.EnableAerialPerspectiveSampling=0; 🟡 def 0
r.VolumetricCloud.EnableAtmosphericLightsSampling=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.VolumetricCloud.EnableDistantSkyLightSampling=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.VolumetricCloud.EnableLocalLightsSampling=0; 🟡 def 0
r.VolumetricCloud.HighQualityAerialPerspective=0; 🟡 def 0
r.VolumetricCloud.Shadow.SampleAtmosphericLightShadowmap=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.VolumetricCloud.ShadowMap=2048; 🟢 1024 for PERFORMANCE 🟡 def 2048
r.VolumetricCloud.SkyAO=0; 🟢 0 for PERFORMANCE ⚪️ EDITED 🟡 def 1
r.VolumetricFog.GridPixelSize=16; 🟡 def 16
r.VolumetricFog.GridSizeZ=64; 🟡 def 64
r.VolumetricFog.HistoryMissSupersampleCount=1; 🟢 1 for PERFORMANCE ⚪️ EDITED 🟡 def 4
r.VolumetricFog.HistoryWeight=0.95; ⚪️ EDITED 🟡 def 0.9
r.VolumetricFog.Jitter=1;
r.VolumetricFog.TemporalReprojection=1; 🟡 def 1
r.VolumetricFog=1; 🟢 0 for PERFORMANCE
r.VSync=0; 🔵 Sync
r.VT.MaxAnisotropy=4;
r.Water.EnableShallowWaterSimulation=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Water.EnableUnderwaterPostProcess=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Water.SingleLayer.DepthPrepass=1; 🟡 def 1
r.Water.SingleLayer.Reflection=1; 🟢 0 for PERFORMANCE 🟡 def 1
r.Water.SingleLayer.RefractionDownsampleFactor=1; 🟡 def 1
r.Water.SingleLayer.ShadersSupportDistanceFieldShadow=1; 🟡 def 1
r.Water.SingleLayer.SSR=0; 🟢 0 for PERFORMANCE ⚪️ EDITED 🟡 def 1
r.Water.SingleLayer.SSRTAA=0; 🟢 0 for PERFORMANCE ⚪️ EDITED 🟡 def 1 🔵 denoiser
r.Water.SingleLayer.TiledComposite=1; 🟡 def 1
r.Water.SingleLayer.UnderwaterFogWhenCameraIsAboveWater=0; 🟡 def 0
r.Water.SingleLayerWater.SupportCloudShadow=0; 🟡 def 0
r.Water.WaterMesh.LODCountBias=0; 🟡 def 0
r.Water.WaterMesh.LODMorphEnabled=1; 🟡 def 1 🔵 experimental
r.Water.WaterMesh.LODScaleBias=0; 🟡 def 0
r.Water.WaterMesh.TessFactorBias=0; 🟢 -1 for PERFORMANCE 🟡 def 0
rhi.SyncInterval=0; 🔵 Sync
rhi.SyncSlackMS=0; 🔵 Sync
t.Streamline.Reflex.Enable=1; 🔵 nvidia reflex
t.Streamline.Reflex.Mode=2; 🔵 reflex on with boost
```

---

#### Open Input.ini and copy pasta %localappdata%
#### or UnrealPak method (pakchunk9999-Mods_CustomMod_P\Engine\Config\Windows\WindowsInput.ini)

```python
[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bEnableMouseSmoothing=0;
bF11TogglesFullscreen=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.1; ⚪️ EDITED 🟡 def 0.2
ButtonRepeatDelay=0.1;
DoubleClickTime=0.01; ⚪️ EDITED 🟡 def 0.1
```

---

#### Open GameUserSettings.ini these commands can overwrite your config if they are here %localappdata%
#### you can turn down used scalability groups here or in game if they are being used

```python
[ScalabilityGroups]
sg.AnimationQuality=?;
sg.AntiAliasingQuality=?;
sg.DOFQuality=?;
sg.EffectsQuality=?;
sg.FoliageQuality=?;
sg.GlobalIlluminationQuality=?;
sg.HairQuality=?;
sg.MaterialQuality=?;
sg.MeshQuality=?;
sg.MotionBlurQuality=?;
sg.ObjectDetailQuality=?;
sg.PhysicsQuality=?;
sg.PopulationQuality=?;
sg.PostProcessQuality=?;
sg.RaytracingQuality=?;
sg.ReflectionQuality=?;
sg.ResolutionQuality=?;
sg.ShadingQuality=?;
sg.ShadowQuality=?;
sg.SkyQuality=?;
sg.TextureQuality=?;
sg.ViewDistanceQuality=?;
sg.VolumetricCloudsQuality=?;
sg.VolumetricFogQuality=?;
sg.VolumetricsQuality=?;

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
