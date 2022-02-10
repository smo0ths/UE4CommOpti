~~~~~~~~~~~~~~~~~~~~~~~~~


*updated 2/10/2022~

*for UE4 games for reference/customization/optimization/learning

*always testing stuff contact me twitch.tv/smoothschannel or discord (discord.gg/vB8f4fZ7EH)

*my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game


-----------------------------------------------------------------
-------------------------Open Engine.ini-------------------------
-----------------------------------------------------------------


Press:       Windows key + R
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Engine.ini


*copy and paste this in engine.ini under lines in the file


[Core.Log]
Global=off;

[Audio]
MaxChannels=64;--------------------------32 48 64 96 128 lower for PERFORMANCE
CommonAudioPoolSize=0;--------------------------default 0
UnfocusedVolumeMultiplier=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=70;--------------------------TEXTUREPOOL CACHE

[SystemSettings]
AllowAsyncRenderThreadUpdates=1;
AllowAsyncRenderThreadUpdatesDuringGamethreadUpdates=1;
r.ShaderDevelopmentMode=0;
r.Shaders.Optimize=1;
r.Shaders.FastMath=1;
au.RenderThreadPriority=3;--------------------------TEST 0 for PERFORMANCE default 3
AudioThread.EnableBatchProcessing=1;--------------------------TEST
AudioThread.BatchAsyncBatchSize=128;--------------------------TEST
r.Atmosphere=1;
r.FullScreenMode=0;
r.VSync=0;
r.MSAA.CompositingSampleCount=1;
r.MSAACount=1;
r.AllowHDR=0;
r.HDR.EnableHDROutput=0;
r.GPUCrashDebugging=0;
r.GPUCrash.CollectionEnable=0;
r.DX11NVAfterMathEnabled=0;
r.AsyncPipelineCompile=1;
r.CompileShadersForDevelopment=0;--------------------------default 1
r.CreateShadersOnLoad=1;--------------------------TEST
r.EarlyZPass=2;--------------------------default 3
r.EarlyZPassMovable=1;
r.EarlyZPassOnlyMaterialMasking=1;
r.D3D11.Depth24Bit=0;--------------------------default 1
r.D3D12.Depth24Bit=0;--------------------------default 1
r.Vulkan.Depth24Bit=0;--------------------------default 0
r.FinishCurrentFrame=0;
r.GTSyncType=0;
RHI.SyncInterval=0;
RHI.SyncSlackMS=0;
r.UniformBufferPooling=1;
r.DrawRectangleOptimization=1;--------------------------default 1
r.AlsoUseSphereForFrustumCull=1;--------------------------TEST 1 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0;--------------------------TEST 1 is EXPERIMENTAL
r.DoLazyStaticMeshUpdate=0;--------------------------1 is EXPERIMENTAL MESHES FLICKER ON 1
r.DeferUniformBufferUpdatesUntilVisible=1;--------------------------TEST
r.DeferUniformExpressionCaching=1;--------------------------TEST
r.DeferSkeletalDynamicDataUpdateUntilGDME=0;--------------------------TEST 1 is EXPERIMENTAL
r.DiscardUnusedQuality=0;--------------------------1 CRASHES GAMES default 0
r.RenderTargetPool.TransientAliasingMode=0;--------------------------TEST
r.RenderTargetPool.AllowMultipleAliasingDiscardsPerFrame=0;--------------------------TEST
r.MorphTarget.Mode=1;--------------------------0 CPU METHOD 1 GPU METHOD default 1
r.VertexFoggingForOpaque=1;
r.DistanceFields.ForceMaxAtlasSize=0;--------------------------TEST
r.DistanceFields.MaxPerMeshResolution=128;--------------------------default 128
r.AOGlobalDFResolution=128;--------------------------default 128
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1;--------------------------TEST
r.NormalMapsForStaticLighting=0;
r.HighQualityLightMaps=1;--------------------------TEST
r.Cache.LimitQuerySize=1;--------------------------default 1
r.Cache.LightingCacheMovableObjectAllocationSize=5;--------------------------TEST
r.AllowGlobalClipPlane=0;
r.HZBOcclusion=0;--------------------------OCCLUSION CULLING ALGORITHM default 1
r.AllowOcclusionQueries=1;
r.NumBufferedOcclusionQueries=1;
r.OneFrameThreadLag=1;--------------------------1 GAME SYNC WITH RENDER THREAD
r.AllowSubPrimitiveQueries=1;
r.SceneColorFormat=3;--------------------------2 for PERFORMANCE default 4
r.DefaultBackBufferPixelFormat=4;--------------------------default 4
r.ClearSceneMethod=1;
r.GBufferFormat=1;--------------------------default 1
r.ClearCoatNormal=0;--------------------------0 for PERFORMANCE
Compat.UseDXT5NormalMaps=0;
r.RayTracing=0;
r.FreeSkeletalMeshBuffers=0;--------------------------TEST default 0
r.GPUSkin.Limit2BoneInfluences=0;--------------------------TEST default 0
r.MinScreenRadiusForLights=0.04;--------------------------0.2 for PERFORMANCE default 0.03
r.MinScreenRadiusForDepthPrepass=0.03;--------------------------default 0.03
r.MinScreenRadiusForCSMDepth=0.01;--------------------------default 0.01
r.SupportAllShaderPermutations=0;
r.SupportStationarySkylight=1;--------------------------default 1
r.SupportPointLightWholeSceneShadows=1;--------------------------TEST default 1
r.SupportAtmosphericFog=1;--------------------------default 1
r.SupportSimpleForwardShading=0;
r.SupportMaterialLayers=1;
r.SupportReversedIndexBuffers=1;--------------------------TEST
r.SupportSkyAtmosphere=1;--------------------------default 1
r.SupportSkyAtmosphereAffectsHeightFog=0;--------------------------TEST default 0
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=1;--------------------------TEST 0 for PERFORMANCE default 0
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=1;--------------------------1 for PERFORMANCE
r.SkyLightingQuality=1;
r.SkylightIntensityMultiplier=1;--------------------------SKYLIGHT INTENSITY
r.SkyLight.RealTimeReflectionCapture=1;--------------------------0 for PERFORMANCE
r.SkyLight.RealTimeReflectionCapture.ShadowFromOpaque=0;--------------------------default 0
r.DefaultFeature.LightUnits=1;--------------------------default 1
r.LightCulling.Quality=1;--------------------------default 1
r.LightFunctionQuality=1;--------------------------0 or 1 for PERFORMANCE default 2
r.LightingDetailMode=150;--------------------------TEST 50 or 100 for PERFORMANCE default 150
r.LightMaxDrawDistanceScale=1;--------------------------DYNAMIC LIGHTS LOD SCALE 0 or 0.6 for PERFORMANCE
r.MipMapLODBias=0;--------------------------LODS
r.LandscapeLODBias=0;
r.SkeletalMeshLODBias=0;--------------------------1 for PERFORMANCE default 0
r.ParticleLODBias=0;--------------------------default 0
r.LandscapeLODDistributionScale=1;--------------------------default 1
r.LandscapeLOD0DistributionScale=1;--------------------------default 1
r.ViewDistanceScale=1;--------------------------VIEW DISTANCE 0.8 for PERFORMANCE default 1
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;
r.SkeletalMeshLODRadiusScale=1;--------------------------1 for PERFORMANCE default 1
r.StaticMeshLODDistanceScale=1;--------------------------1 for PERFORMANCE default 1
r.SplineMesh.NoRecreateProxy=1;
r.TextureStreaming=1;--------------------------TEXTURE STREAMING
r.Streaming.MipBias=0;--------------------------1 for PERFORMANCE default 0
r.Streaming.UseFixedPoolSize=0;
r.Streaming.LimitPoolSizeToVRAM=1;
r.Streaming.PoolSize=800;
r.Streaming.PoolSizeForMeshes=-1;--------------------------default -1
r.RenderTargetPoolMin=400;
r.Streaming.MaxTempMemoryAllowed=50;
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.UseAllMips=0;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.Boost=1;
r.Streaming.UsePerTextureBias=1;
r.Streaming.AmortizeCPUToGPUCopy=0;
r.Streaming.MaxNumTexturesToStreamPerFrame=0;
r.Streaming.FramesForFullUpdate=10;
r.Streaming.NumStaticComponentsProcessedPerFrame=50;
r.Streaming.FullyLoadUsedTextures=0;
r.Streaming.DefragDynamicBounds=1;
r.Streaming.HiddenPrimitiveScale=0.5;--------------------------default 0.5
r.Streaming.UseNewMetrics=1;
r.Streaming.MinMipForSplitRequest=10;
r.Streaming.UseMaterialData=1;
r.DistanceFieldAO=0;--------------------------DFAO 0 for PERFORMANCE
r.AOHeightfieldOcclusion=0;--------------------------LANDSCAPE DFAO 0 for PERFORMANCE
r.AOQuality=1;--------------------------1 for PERFORMANCE 0 off default 2
r.HeightFieldShadowing=1;--------------------------HEIGHT FIELD SHADOWING 0 off
r.HFShadowQuality=2;--------------------------default 2
r.ShadowQuality=3;--------------------------SHADOWS 3 for PERFORMANCE 0 off
r.Shadow.FilterMethod=0;--------------------------1 for PCSS
r.Shadow.FadeResolution=64;--------------------------default 64
r.Shadow.MaxResolution=2048;--------------------------1024 for PERFORMANCE
r.Shadow.MaxCSMResolution=2048;
r.Shadow.CSM.MaxCascades=4;--------------------------lower for PERFORMANCE
r.Shadow.CSM.TransitionScale=1.5;--------------------------default 1
r.Shadow.CSMShadowDistanceFadeoutMultiplier=1;--------------------------default 1
r.Shadow.TransitionScale=60;--------------------------default 60
r.Shadow.MinPreShadowResolution=8;--------------------------default 8
r.Shadow.PreShadowFadeResolution=16;--------------------------default 16
r.Shadow.PreShadowResolutionFactor=1;--------------------------0.5 for PERFORMANCE
r.Shadow.SpotLightTransitionScale=256;--------------------------TEST default 60
r.Shadow.SpotLightSlopeDepthBias=3;--------------------------default 3
r.Shadow.SpotLightReceiverBias=0.5;--------------------------default 0.5
r.Shadow.SpotLightDepthBias=3;--------------------------default 3
r.Shadow.RadiusThreshold=0.03;--------------------------0.03 for PERFORMANCE default 0.03
r.Shadow.DistanceScale=1;--------------------------0.6 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;--------------------------0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;--------------------------0 for PERFORMANCE
r.Shadow.CacheWholeSceneShadows=1;
r.Shadow.CacheWPOPrimitives=0;--------------------------TEST default 0
r.Shadow.OcclusionCullCascadedShadowMaps=1;--------------------------TEST default 0
r.Shadow.WholeSceneShadowCacheMb=150;--------------------------default 150
r.Shadow.UnbuiltPreviewInGame=1;
r.Shadow.ForceSingleSampleShadowingFromStationary=0;--------------------------TEST default 0
r.Shadow.TexelsPerPixel=1.27324;--------------------------default 1.27324
r.Shadow.TexelsPerPixelPointlight=1.27324;--------------------------default 1.27324
r.Shadow.TexelsPerPixelRectlight=1.27324;--------------------------default 1.27324
r.Shadow.TexelsPerPixelSpotlight=2.54648;--------------------------default 2.54648
r.ContactShadows=0;--------------------------0 for PERFORMANCE
r.ContactShadows.NonShadowCastingIntensity=0.2;
r.CapsuleShadows=0;--------------------------0 for PERFORMANCE
r.CapsuleShadowsFullResolution=0;--------------------------0 for PERFORMANCE
r.AllowLandscapeShadows=1;--------------------------LANDSCAPE SHADOWS 0 for PERFORMANCE
r.DistanceFieldShadowing=1;--------------------------DISTANCE FIELD SHADOWING 0 for PERFORMANCE
r.DFShadowQuality=3;--------------------------1 for PERFORMANCE 0 off default 3
r.Shadow.MaxNumFarShadowCascades=0;--------------------------TEST
r.DFFullResolution=1;--------------------------0 for PERFORMANCE
r.DFShadowScatterTileCulling=1;--------------------------1 for PERFORMANCE
r.DFTwoSidedMeshDistanceBias=5;
r.DFDistanceScale=1;--------------------------default 1
r.Upscale.Quality=2;
r.Downsample.Quality=1;--------------------------default 1
r.Tonemapper.Quality=0;
r.Tonemapper.GrainQuantization=1;--------------------------FIGHTS 8 BIT COLOR BANDING default 1
r.Tonemapper.Sharpen=0;
r.Tonemapper.EmulateHDR=0;
r.TonemapperGamma=0;
ShowFlag.Vignette=0;
ShowFlag.Grain=0;
r.MinRoughnessOverride=0.2;--------------------------0 with TAA 0.2 without TAA
r.DefaultFeature.AntiAliasing=1;--------------------------1 FXAA 2 TAA 3 MSAA 0 off
r.PostProcessAAQuality=1;--------------------------1 to 2 FXAA 3-4 TAA 0 off
r.TemporalAASamples=4;
r.TemporalAACurrentFrameWeight=0.1;
r.TemporalAA.R11G11B10History=0;--------------------------1 is EXPERIMENTAL
r.TemporalAA.Algorithm=0;--------------------------GEN 5 TAA 0 for PERFORMANCE
r.TemporalAA.Upsampling=0;--------------------------TAAU
r.TemporalAAUpsampleFiltered=1;
r.TemporalAAFilterSize=0.5;
r.ScreenPercentage=100;--------------------------INPUT RESOLUTION PERCENTAGE for TAAU
r.SecondaryScreenPercentage.GameViewport=0;
r.SceneRenderTargetResizeMethodForceOverride=1;
r.SceneRenderTargetResizeMethod=0;--------------------------default 0
r.EnableAsyncComputeTranslucencyLightingVolumeClear=1;--------------------------TEST
r.AllowDownsampledStandardTranslucency=0;--------------------------default 0
r.TranslucencyLightingVolume=1;--------------------------LIT TRANSLUCENCY
r.TranslucencyVolumeBlur=1;
r.TranslucencyLightingVolumeDim=48;--------------------------default 64
p.BatchPhysXTasksSize=3;--------------------------TEST default 3
p.ClothPhysics=1;--------------------------0 for PERFORMANCE default 1
p.ClothPhysics.UseTaskThread=1;--------------------------default 1
p.AllowCachedOverlaps=1;--------------------------default 1
p.AnimDynamics=1;--------------------------0 for PERFORMANCE
p.AnimDynamicsWind=1;--------------------------0 for PERFORMANCE
p.AnimDynamicsAdaptiveSubstep=0;--------------------------TEST
p.AnimDynamicsRestrictLOD=1;--------------------------TEST 0 for PERORMANCE default -1
p.AnimDynamicsLODThreshold=1;--------------------------TEST 0 for PERORMANCE default -1
p.RigidBodyNode=1;--------------------------TEST
p.RigidBodyLODThreshold=1;--------------------------TEST 0 for PERORMANCE default -1
r.SeparateTranslucency=1;--------------------------default 1
r.TranslucentSortPolicy=0;
r.DefaultFeature.AmbientOcclusion=1;--------------------------default 1
r.DefaultFeature.AmbientOcclusionStaticFraction=1;--------------------------default 1
r.AmbientOcclusionStaticFraction=-1;--------------------------0 for PERFORMANCE default -1
r.AmbientOcclusionLevels=2;--------------------------SSAO 0 for PERFORMANCE 0 off
r.AmbientOcclusionMipLevelFactor=0.5;--------------------------default 0.5
r.AmbientOcclusionMaxQuality=100;
r.AmbientOcclusionRadiusScale=0;
r.AmbientOcclusion.Compute=1;--------------------------1 for PERFORMANCE
r.AmbientOcclusion.Compute.Smooth=1;
r.LightShaftQuality=0;--------------------------LIGHT SHAFTS 0 for PERFORMANCE
r.LightShaftAllowTAA=1;--------------------------TEST default 1
r.LightShaftDownSampleFactor=2;
r.LightShaftFirstPassDistance=0.1;
r.LightShaftBlurPasses=3;
r.LightShaftNumSamples=12;
r.LightShaftRenderToSeparateTranslucency=0;
r.Fog=1;
r.EnableAsyncComputeVolumetricFog=1;--------------------------TEST
r.VolumetricFog=1;--------------------------0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=32;
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.HistoryWeight=0.9;
r.VolumetricFog.InjectShadowedLightsSeparately=0;
r.VolumetricFog.TemporalReprojection=1;
r.VolumetricFog.HistoryMissSupersampleCount=1;
r.VolumetricCloud.SkyAO=0;--------------------------TEST
r.VolumetricCloud.ShadowMap=0;--------------------------TEST
r.DoTiledReflections=1;--------------------------TILED REFLECTION default 1
r.ReflectionEnvironment=1;--------------------------REFLECTION ENVIRONMENT 0 for PERFORMANCE
r.chaos.ReflectionCaptureStaticSceneOnly=1;--------------------------1 for PERFORMANCE default 1
r.ReflectionCaptureSupersampleFactor=1;
r.ReflectionCaptureGPUArrayCopy=1;
r.ReflectionCaptureResolution=128;--------------------------64 for PERFORMANCE default 128
r.ReflectionEnvironmentLightmapMixing=1;
r.ReflectionEnvironmentBeginMixingRoughness=0.1;
r.ReflectionEnvironmentEndMixingRoughness=0.3;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;
r.ReflectionEnvironmentLightmapMixLargestWeight=10000;
r.TiledDeferredShading=1;--------------------------TILED DEFERRED SHADING 0 for PERFORMANCE
r.TiledDeferredShading.MinimumCount=80;--------------------------default 80
r.SSR.Quality=0;--------------------------SSR 0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;--------------------------1 for PERFORMANCE
r.SSR.MaxRoughness=-1;
r.SSR.Temporal=1;--------------------------default 1
r.SSR.ExperimentalDenoiser=0;
r.SSGI.Enable=0;--------------------------SSGI 0 for PERFORMANCE 0 off
r.SSGI.Quality=0;--------------------------0 for PERFORMANCE 0 off
r.SSGI.HalfRes=1;--------------------------1 for PERFORMANCE
r.SSGI.LeakFreeReprojection=0;--------------------------default 0
r.SubsurfaceScattering=1;--------------------------SSS 0 for PERFORMANCE
r.SSS.Scale=1;--------------------------default 1
r.SSS.SampleSet=1;--------------------------0 for PERFORMANCE default 2
r.SSS.Quality=-1;--------------------------0 for PERFORMANCE
r.SSS.HalfRes=1;
r.SSS.Filter=1;--------------------------TEST
r.SSS.Checkerboard=1;--------------------------1 for 32Bit SceneColorFormat
r.DefaultFeature.AutoExposure=1;--------------------------default 1
r.EyeAdaptationQuality=2;--------------------------1 for PERFORMANCE 0 off default 2
r.MaxAnisotropy=8;
r.AnisotropicMaterials=1;--------------------------0 for PERFORMANCE
ShowFlag.Tessellation=1;--------------------------0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=48;--------------------------9999999 for PERFORMANCE default 48
r.MaterialQualityLevel=1;--------------------------0 for PERFORMANCE 0 low 1 high 2 medium 3 epic
r.DetailMode=2;--------------------------TEST 0 or 1 for PERFORMANCE default 2
r.RefractionQuality=1;--------------------------0 or 1 for PERFORMANCE default 2
r.IrisNormal=1;--------------------------0 for PERFORMANCE
r.DepthOfFieldQuality=2;--------------------------DOF 0 or 1 for PERFORMANCE 0 off default 2
r.Filter.SizeScale=1;--------------------------default 1
r.Filter.NewMethod=1;
r.Filter.LoopMode=0;
r.DefaultFeature.Bloom=1;--------------------------default 1
r.BloomQuality=3;--------------------------BLOOM 0 off
r.Bloom.HalfResolutionFFT=0;
r.Bloom.Cross=0;--------------------------use -0.7777 for ANAMORPHIC BLOOM default 0
r.DefaultFeature.MotionBlur=1;--------------------------default 1
r.MotionBlurQuality=0;
r.FastBlurThreshold=0;
r.DefaultFeature.LensFlare=1;--------------------------default 1
r.LensFlareQuality=2;--------------------------LENS FLARES 0 for PERFORMANCE 0 off default 2
r.SceneColorFringeQuality=0;
r.SceneColorFringe.Max=-1;
r.AllowSimpleLights=1;--------------------------0 for PERFORMANCE
r.ParticleLightQuality=1;--------------------------PARTICLES 0 or 1 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=10;
r.Emitter.FastPoolEnable=1;--------------------------default 1
r.EmitterSpawnRateScale=0.5;--------------------------0.25 or 0.5 for PERFORMANCE
FX.QualityLevelSpawnRateScaleReferenceLevel=2;--------------------------TEST 0 or 1 for PERFORMANCE default 2
FX.BatchAsync=1;--------------------------TEST
FX.BatchAsyncBatchSize=32;--------------------------default 32
FX.AllowAsyncTick=1;
FX.EarlyScheduleAsync=0;--------------------------TEST
FX.AllowCulling=1;
FX.FXAllowParticleMeshLODs=1;--------------------------TEST
FX.MaxCPUParticlesPerEmitter=500;--------------------------TEST default 1000
FX.MaxGPUParticlesSpawnedPerFrame=25000;--------------------------TEST default 1048576
r.DBuffer=0;--------------------------DECAL METERIAL BLEND MODES 0 for PERFORMANCE default 1
r.ForceSceneHasDecals=0;--------------------------TEST
r.Decal.FadeDurationScale=1;--------------------------0.6 for PERFORMANCE default 1
r.Decal.FadeScreenSizeMult=1;
r.Decal.StencilSizeThreshold=0.1;--------------------------default 0.1
grass.DensityScale=0.6;--------------------------0.6 for PERFORMANCE
grass.DisableDynamicShadows=0;--------------------------1 for PERFORMANCE
grass.TickInterval=5;
foliage.DensityScale=0.6;--------------------------0.6 for PERFORMANCE
foliage.LODDistanceScale=1;--------------------------1 for PERFORMANCE default 1
foliage.OverestimateLOD=1;--------------------------TEST 1 for PERFORMANCE
foliage.MaxTrianglesToRender=1000000;--------------------------default 100000000
foliage.RandomLODRange=0;
foliage.MinimumScreenSize=0.0001;--------------------------default 0.0001
foliage.MinVertsToSplitNode=8192;
foliage.DitheredLOD=1;


------------------------------------------------------------------------------------------------------
-------------------------AA settings i use Copy/Paste over or experiment------------------------------
------------------------------------------------------------------------------------------------------


TAA
r.MinRoughnessOverride=0;--------------------------0 with TAA 0.2 without TAA
r.DefaultFeature.AntiAliasing=2;--------------------------1 FXAA 2 TAA 3 MSAA 0 off
r.PostProcessAAQuality=3;--------------------------1 to 2 FXAA 3-4 TAA 0 off
r.TemporalAASamples=4;
r.TemporalAACurrentFrameWeight=0.1;
r.TemporalAA.R11G11B10History=0;--------------------------1 is EXPERIMENTAL
r.TemporalAA.Algorithm=0;--------------------------GEN 5 TAA 0 for PERFORMANCE
r.TemporalAA.Upsampling=0;--------------------------TAAU
r.TemporalAAUpsampleFiltered=1;
r.TemporalAAFilterSize=0.5;
r.ScreenPercentage=100;--------------------------INPUT RESOLUTION PERCENTAGE for TAAU

TAAU +15fps in scene
r.MinRoughnessOverride=0;--------------------------0 with TAA 0.2 without TAA
r.DefaultFeature.AntiAliasing=2;--------------------------1 FXAA 2 TAA 3 MSAA 0 off
r.PostProcessAAQuality=3;--------------------------1 to 2 FXAA 3-4 TAA 0 off
r.TemporalAASamples=4;
r.TemporalAACurrentFrameWeight=0.1;
r.TemporalAA.R11G11B10History=0;--------------------------1 is EXPERIMENTAL
r.TemporalAA.Algorithm=0;--------------------------GEN 5 TAA 0 for PERFORMANCE
r.TemporalAA.Upsampling=1;--------------------------TAAU
r.TemporalAAUpsampleFiltered=1;
r.TemporalAAFilterSize=0.5;
r.ScreenPercentage=86.66;--------------------------INPUT RESOLUTION PERCENTAGE for TAAU

FXAA
r.MinRoughnessOverride=0.2;--------------------------0 with TAA 0.2 without TAA
r.DefaultFeature.AntiAliasing=1;--------------------------1 FXAA 2 TAA 3 MSAA 0 off
r.PostProcessAAQuality=1;--------------------------1 to 2 FXAA 3-4 TAA 0 off
r.TemporalAASamples=4;
r.TemporalAACurrentFrameWeight=0.1;
r.TemporalAA.R11G11B10History=0;--------------------------1 is EXPERIMENTAL
r.TemporalAA.Algorithm=0;--------------------------GEN 5 TAA 0 for PERFORMANCE
r.TemporalAA.Upsampling=0;--------------------------TAAU
r.TemporalAAUpsampleFiltered=1;
r.TemporalAAFilterSize=0.5;
r.ScreenPercentage=100;--------------------------INPUT RESOLUTION PERCENTAGE for TAAU

NONE
r.MinRoughnessOverride=0.2;--------------------------0 with TAA 0.2 without TAA
r.DefaultFeature.AntiAliasing=0;--------------------------1 FXAA 2 TAA 3 MSAA 0 off
r.PostProcessAAQuality=0;--------------------------1 to 2 FXAA 3-4 TAA 0 off
r.TemporalAASamples=4;
r.TemporalAACurrentFrameWeight=0.1;
r.TemporalAA.R11G11B10History=0;--------------------------1 is EXPERIMENTAL
r.TemporalAA.Algorithm=0;--------------------------GEN 5 TAA 0 for PERFORMANCE
r.TemporalAA.Upsampling=0;--------------------------TAAU
r.TemporalAAUpsampleFiltered=1;
r.TemporalAAFilterSize=0.5;
r.ScreenPercentage=100;--------------------------INPUT RESOLUTION PERCENTAGE for TAAU


----------------------------------------------------------------
-------------------------Open Input.ini-------------------------
----------------------------------------------------------------


%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Input.ini


*edit input commands or add them


[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.2;--------------------------default 0.2
ButtonRepeatDelay=0.1;--------------------------default 0.1
DoubleClickTime=0.1;--------------------------default 0.25
ConsoleKeys=Tilde;


---------------------------------------------------------------------------
-------------------------Open GameUserSettings.ini-------------------------
---------------------------------------------------------------------------

 
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/GameUserSettings.ini


*here are a few things to look for or tweak these overwrite engine.ini commands unfortunately


AudioQualityLevel=3
MaxAnisotropy=8
bUseVSync=0
MaxFPS=163
FrameRateLimit=163
MenuFrameRateLimit=163
HDRDisplayOutputNits=300;--------------------------set your monitors nits if using hdr
DoubleKeyPressTime=0.1
TextureStreamPoolSizeStorage=800;--------------------------for squad
DistanceFieldShadows=1;--------------------------for squad
Gamma=2.2
TAASampleStorage=4
bRTXEnabled=1
bRTXReflectionsEnabled=0
bRTXShadowsEnabled=0
bRTXAmbientOcclusionEnabled=0
DlssQualitySetting=1
ResolutionScaleModifier=1
DFAO=0
Tessellation=1
TessellationMode=48
bTelemetryEnabled=0
bUseDynamicResolution=0
FullscreenMode=0
PreferredFullscreenMode=0
ContactShadows=0
PostFX_Saturation=1.2
PostFX_Sharpness=0
OverrideOptions=(("r.somerandomcommand", (Value=0,bModified=True)),("r.someotherrandomcommand", (Value=0,bModified=False)));--------------------------if you want to override from GameUserSettings.ini


*set your scalability groups, 0=low/1=medium/2=high/3=epic/4=cinematic (4 gets clamped)


[ScalabilityGroups]
sg.ResolutionQuality=100;
sg.ViewDistanceQuality=2;
sg.ViewDistanceQuality.NumLevels=5;
sg.AntiAliasingQuality=2;
sg.AntiAliasingQuality.NumLevels=5;
sg.PostProcessQuality=2;
sg.PostProcessQuality.NumLevels=5;
sg.ShadowQuality=2;
sg.ShadowQuality.NumLevels=5;
sg.TextureQuality=2;
sg.TextureQuality.NumLevels=5;
sg.EffectsQuality=2;
sg.EffectsQuality.NumLevels=5;
sg.FoliageQuality=2;
sg.FoliageQuality.NumLevels=5;
sg.ShadingQuality=2;
sg.ShadingQuality.NumLevels=5;
sg.AnimationQuality=2;
sg.AnimationQuality.NumLevels=5;


-------------------------------------------------------------------------
-------------------------Open DeviceProfiles.ini-------------------------
-------------------------------------------------------------------------

   
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/DeviceProfiles.ini


*textures lods experiment for performance or just use the games default texture settings


[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Cinematic,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=linear,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_NoMipmaps,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_MobileFlattened,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_Face,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_LightMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=1,MaxLODSize=2048,OptionalMaxLODSize=1,OptionalLODBias=1,MaxLODSize_Smaller=1,MaxLODSize_Smallest=1,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ColorLookupTable,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,MinLODSize=1,MaxLODSize=4096,MaxLODSize_Smallest=1,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,MinLODSize=1,MaxLODSize=4096,MaxLODSize_Smallest=1,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Bokeh,MinLODSize=1,MaxLODSize=256,OptionalMaxLODSize=128,OptionalLODBias=1,MaxLODSize_Smaller=128,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=linear,MipFilter=linear,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_IESLightProfile,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=point,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_HierarchicalLOD,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Impostor,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_ImpostorNormalDepth,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_8BitData,LODBias=0,MinMagFilter=point,MipFilter=linear,MipGenSettings=TMGS_NoMipmaps)
TextureLODGroups=(Group=TEXTUREGROUP_16BitData,LODBias=0,MinMagFilter=point,MipFilter=linear,MipGenSettings=TMGS_NoMipmaps)
TextureLODGroups=(Group=TEXTUREGROUP_Project01,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project02,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project03,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project04,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project05,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project06,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project07,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project08,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project09,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project10,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project11,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project12,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project13,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project14,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Project15,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_MAX,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=1024,MaxLODSize_Smallest=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)


-------------------------------------------------------------------
-------------------------for NVIDIA users--------------------------
-------------------------------------------------------------------


Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method)

Adjust image settings set to Performance and apply then Select Use the advanced 3D image settings and apply

In manage 3D settings:

Anisotropic filtering:  Off for perf. App-controlled or force your own setting for quality (8x is nice)

Low latency mode:  
1. Off and ~85% gpu usage for most med-lower end systems (assuming you cap fps correctly)
2. On feels consistent (i use this and reflex in games that support it)
3. Ultra and relfex (in-game) feels good when gpu usage is ~97%

Power management mode:  Prefer max performance  (this is the "+ boost" in reflex + boost)

Preferred refresh rate:  Highest available

Texture filtering - anisotropic sample optimization:  on

Texture filtering - Negative LOD bias:  Allow

Texture filtering quality:  High performance

Vertical sync:  Off


---------------------------------------------------------------------------------------------------
-------------------------How to enable Message-signaled interrupts (MSIs)--------------------------
---------------------------------------------------------------------------------------------------


use Wtools v1.0.2.0.exe (Wagnardsoft Tools) enable it and restart

or

when you make your driver setup.exe using NVCleanstall enabling it in advanced settings

or

find ID: open device manager right click your GPU properties and click on events tab

looks like this:

HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties

find in regedit and set MSISupported to 1 then restart


~~~~~~~~~~~~~~~~~~~~~~~~~
