~~~~~~~~~~~~~~~~~~~~~~~~~


*Updated 1/7/2022

*For UE4 games for reference/customization/optimization/learning

*Discord link discord.gg/vB8f4fZ7EH

*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/BendGame/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Engine.ini


my config is more of a quality balance you may need to tweak some commands, copy and paste under code

[Core.Log]
Global=off;

[Audio]
MaxChannels=64;--------------------------32 48 64 96 128 LOWER VALUES for PERFORMANCE
CommonAudioPoolSize=0;--------------------------default 0
UnfocusedVolumeMultiplier=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=70;--------------------------TEXTUREPOOL CACHE

[ConsoleVariables]
AllowAsyncRenderThreadUpdates=1;
AllowAsyncRenderThreadUpdatesDuringGamethreadUpdates=1;
r.ShaderDevelopmentMode=0;
r.Shaders.Optimize=1;
r.Shaders.FastMath=1;
au.RenderThreadPriority=3;--------------------------TEST 0 for PERFORMANCE default 3
AudioThread.EnableBatchProcessing=1;--------------------------TEST
AudioThread.BatchAsyncBatchSize=128;--------------------------TEST
r.Atmosphere=1;
r.VSync=0;
r.AllowHDR=0;
r.HDR.EnableHDROutput=0;
r.GPUCrashDebugging=0;
r.AsyncPipelineCompile=1;
r.CompileShadersForDevelopment=0;--------------------------default 1
r.CreateShadersOnLoad=0;--------------------------TEST
r.EarlyZPass=2;--------------------------default 3
r.EarlyZPassMovable=1;
r.EarlyZPassOnlyMaterialMasking=1;
r.DBuffer=1;--------------------------DECAL METERIAL BLEND MODES 0 for PERFORMANCE default 1
r.FinishCurrentFrame=0;
r.GTSyncType=0;
RHI.SyncInterval=0;
RHI.SyncSlackMS=0;
r.UniformBufferPooling=1;
r.DrawRectangleOptimization=1;--------------------------default 1
r.AlsoUseSphereForFrustumCull=0;--------------------------TEST 0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0;--------------------------TEST 1 is EXPERIMENTAL
r.DoLazyStaticMeshUpdate=0;--------------------------1 is EXPERIMENTAL MESHES FLICKER ON 1
r.DeferUniformBufferUpdatesUntilVisible=1;--------------------------TEST
r.DeferUniformExpressionCaching=1;--------------------------TEST
r.DeferSkeletalDynamicDataUpdateUntilGDME=0;--------------------------TEST 1 is EXPERIMENTAL
r.MeshStreaming=0;--------------------------1 is EXPERIMENTAL
r.DiscardUnusedQuality=0;--------------------------1 CRASHES GAMES default 0
r.RenderTargetPool.TransientAliasingMode=0;--------------------------TEST
r.RenderTargetPool.AllowMultipleAliasingDiscardsPerFrame=0;--------------------------TEST
r.MorphTarget.Mode=1;--------------------------0 CPU METHOD 1 GPU METHOD default 1
r.VertexFoggingForOpaque=1;
r.GenerateMeshDistanceFields=1;--------------------------0 for PERFORMANCE
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1;--------------------------TEST
r.NormalMapsForStaticLighting=0;
r.GenerateLandscapeGIData=0;--------------------------0 for PERFORMANCE
r.AllowGlobalClipPlane=0;
r.HZBOcclusion=0;--------------------------OCCLUSION CULLING ALGORITHM default 1
r.AllowOcclusionQueries=1;
r.OneFrameThreadLag=1;--------------------------1 GAME SYNC WITH RENDER THREAD
r.AllowSubPrimitiveQueries=1;
r.SceneColorFormat=4;--------------------------3 for PERFORMANCE default 4
r.DefaultBackBufferPixelFormat=4;--------------------------default 4
r.ClearSceneMethod=1;
r.ClearWithExcludeRects=2;--------------------------default 2
r.GBufferFormat=1;--------------------------default 1
r.ClearCoatNormal=0;--------------------------0 for PERFORMANCE
Compat.UseDXT5NormalMaps=0;
Compat.MAX_GPUSKIN_BONES=256;--------------------------TEST
r.FreeSkeletalMeshBuffers=0;--------------------------TEST default 0
r.GPUSkin.Limit2BoneInfluences=0;--------------------------TEST default 0
r.MinScreenRadiusForLights=0.03;--------------------------TEST 0.03 for PERFORMANCE default 0.03
r.MinScreenRadiusForDepthPrepass=0.03;--------------------------default 0.03
r.MinScreenRadiusForCSMDepth=0.03;
r.SupportAllShaderPermutations=0;--------------------------TEST
r.SupportStationarySkylight=1;--------------------------default 1
r.SupportPointLightWholeSceneShadows=1;--------------------------TEST default 1
r.SupportAtmosphericFog=1;--------------------------default 1
r.SupportSkyAtmosphere=1;--------------------------default 1
r.SupportSkyAtmosphereAffectsHeightFog=0;--------------------------TEST default 0
r.SupportSimpleForwardShading=0;
r.SupportMaterialLayers=1;
r.SupportReversedIndexBuffers=1;--------------------------TEST
r.SkyLightingQuality=1;--------------------------TEST 0 for PERFORMANCE
r.SkylightIntensityMultiplier=1;--------------------------SKYLIGHT INTENSITY
r.SkyLight.RealTimeReflectionCapture=1;--------------------------TEST
r.LightFunctionQuality=1;--------------------------0 or 1 for PERFORMANCE default 2
r.LightingDetailMode=100;--------------------------50 or 100 for PERFORMANCE default 150
r.LightMaxDrawDistanceScale=1;--------------------------DYNAMIC LIGHTS LOD SCALE 0 or 0.6 for PERFORMANCE
r.MipMapLODBias=0;--------------------------LODS
r.LandscapeLODBias=0;
r.SkeletalMeshLODBias=0;
r.ParticleLODBias=-1;
r.LandscapeLODDistributionScale=1;
r.LandscapeLOD0DistributionScale=1;
r.ViewDistanceScale=1;--------------------------VIEW DISTANCE 0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;
r.SkeletalMeshLODRadiusScale=1;--------------------------LOWER for QUALITY 0.25-1 default 1
r.StaticMeshLODDistanceScale=0.5;--------------------------1.5 for PERFORMANCE default 1
r.SplineMesh.NoRecreateProxy=1;
r.TextureStreaming=1;--------------------------TEXTURE STREAMING
r.Streaming.MipBias=0;
r.Streaming.UseFixedPoolSize=0;
r.Streaming.LimitPoolSizeToVRAM=1;
r.Streaming.PoolSize=2048;
r.RenderTargetPoolMin=512;--------------------------TEST
r.Streaming.MaxTempMemoryAllowed=50;--------------------------TEST
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.UseAllMips=0;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.Boost=1;
r.Streaming.UsePerTextureBias=1;
r.Streaming.AmortizeCPUToGPUCopy=0;--------------------------TEST
r.Streaming.MaxNumTexturesToStreamPerFrame=0;--------------------------TEST
r.Streaming.FramesForFullUpdate=10;
r.Streaming.NumStaticComponentsProcessedPerFrame=50;
r.Streaming.FullyLoadUsedTextures=0;
r.Streaming.DefragDynamicBounds=1;
r.Streaming.ScaleTexturesByGlobalMyBias=1;
r.Streaming.HiddenPrimitiveScale=0.5;--------------------------default 0.5
r.Streaming.UseNewMetrics=1;
r.Streaming.MinMipForSplitRequest=1;
r.Streaming.UseMaterialData=1;
r.DistanceFieldGI=0;
r.DistanceFieldAO=0;--------------------------DFAO 0 for PERFORMANCE
r.AOQuality=0;--------------------------0 for PERFORMANCE 0 off default 2
r.ShadowQuality=3;--------------------------SHADOWS
r.Shadow.FilterMethod=0;
r.Shadow.MaxResolution=1024;
r.Shadow.MaxCSMResolution=2048;
r.Shadow.CSM.MaxCascades=3;--------------------------TEST 1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1.5;--------------------------default 1
r.Shadow.RadiusThreshold=0.01;--------------------------default 0.03
r.Shadow.DistanceScale=1.5;--------------------------0.6 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;--------------------------0 for PERFORMANCE
r.ContactShadows=0;--------------------------0 for PERFORMANCE
r.ContactShadows.NonShadowCastingIntensity=0.2;
r.CapsuleShadows=0;--------------------------0 for PERFORMANCE
r.AllowLandscapeShadows=1;--------------------------LANDSCAPE SHADOWS 0 for PERFORMANCE
r.DistanceFieldShadowing=1;--------------------------DISTANCE FIELD SHADOWING 0 for PERFORMANCE
r.DFShadowQuality=3;--------------------------1 for PERFORMANCE 0 off default 3
r.Shadow.MaxNumFarShadowCascades=1;--------------------------0 for PERFORMANCE
r.DFFullResolution=0;--------------------------0 for PERFORMANCE
r.DFShadowScatterTileCulling=1;--------------------------1 is OPTIMAL
r.DFTwoSidedMeshDistanceBias=3;
r.DFDistanceScale=1.1;--------------------------default 1
r.Tonemapper.Quality=2;
r.TonemapperFilm=1;
r.Tonemapper.GrainQuantization=1;--------------------------FIGHTS 8 BIT COLOR BANDING default 1
r.Tonemapper.Sharpen=0;
r.Tonemapper.EmulateHDR=0;
ShowFlag.Vignette=0;
ShowFlag.Grain=0;
r.MinRoughnessOverride=0.2;--------------------------0.2 WITHOUT TAA 0 WITH TAA
r.DefaultFeature.AntiAliasing=0;--------------------------1 FXAA 2 TAA 3 MSAA 0 off
r.PostProcessAAQuality=0;--------------------------1 to 2 FXAA 3-4 TAA 0 off
r.MSAACount=0;
r.TemporalAASamples=4;
r.TemporalAACurrentFrameWeight=1;
r.TemporalAA.R11G11B10History=0;--------------------------1 is EXPERIMENTAL
r.TemporalAA.Algorithm=0;--------------------------GEN 5 TAA
r.TemporalAA.Upsampling=0;--------------------------TAAU
r.TemporalAAUpsampleFiltered=0;
r.ScreenPercentage=100;--------------------------INPUT RESOLUTION PERCENTAGE for TAAU
r.SceneRenderTargetResizeMethodForceOverride=1;
r.SceneRenderTargetResizeMethod=0;--------------------------default 0
r.SceneCaptureResizeMethod=0;--------------------------default 0
r.EnableAsyncComputeTranslucencyLightingVolumeClear=1;--------------------------TEST
r.AllowDownsampledStandardTranslucency=0;--------------------------TEST default 0
r.TranslucencyLightingVolume=1;--------------------------LIT TRANSLUCENCY
r.TranslucencyVolumeBlur=1;
r.TranslucencyLightingVolumeDim=48;--------------------------default 64
p.BatchPhysXTasksSize=3;--------------------------TEST
p.ClothPhysics=1;--------------------------default 1
p.AllowCachedOverlaps=1;
p.AnimDynamics=1;--------------------------0 for PERFORMANCE
p.AnimDynamicsWind=1;--------------------------0 for PERFORMANCE
p.AnimDynamicsAdaptiveSubstep=0;--------------------------TEST
p.AnimDynamicsRestrictLOD=-1;--------------------------TEST
p.AnimDynamicsLODThreshold=1;--------------------------0 for PERFORMANCE
p.RigidBodyLODThreshold=1;--------------------------0 for PERFORMANCE
r.SeparateTranslucency=1;--------------------------default 1
r.TranslucentSortPolicy=0;
r.AmbientOcclusionLevels=2;--------------------------SSAO 0 for PERFORMANCE
r.DefaultFeature.AmbientOcclusionStaticFraction=0;--------------------------0 for PERFORMANCE
r.AmbientOcclusionStaticFraction=0;--------------------------0 for PERFORMANCE
r.AmbientOcclusionMipLevelFactor=0.5;--------------------------default 0.5
r.AmbientOcclusionMaxQuality=100;
r.AmbientOcclusionSampleSetQuality=-1;
r.AmbientOcclusion.Compute=0;
r.AmbientOcclusionRadiusScale=0;
r.LightShaftQuality=1;--------------------------LIGHT SHAFTS 0 for PERFORMANCE
r.LightShaftDownSampleFactor=2;
r.LightShaftFirstPassDistance=0.1;
r.LightShaftBlurPasses=3;
r.LightShaftNumSamples=12;
r.LightShaftRenderToSeparateTranslucency=0;
r.Fog=1;
r.VolumetricFog=1;--------------------------0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=32;
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.HistoryWeight=0.9;
r.VolumetricFog.InjectShadowedLightsSeparately=0;
r.VolumetricFog.TemporalReprojection=1;
r.VolumetricFog.HistoryMissSupersampleCount=1;
r.ReflectionEnvironment=1;--------------------------REFLECTION ENVIRONMENT 0 for PERFORMANCE
r.chaos.ReflectionCaptureStaticSceneOnly=1;--------------------------1 for PERFORMANCE default 1
r.ReflectionCaptureGPUArrayCopy=1;
r.ReflectionCaptureResolution=128;--------------------------default 128
r.ReflectionEnvironmentLightmapMixing=1;
r.DoTiledReflections=1;--------------------------TILED REFLECTION default 1
r.TiledDeferredShading=1;--------------------------TILED DEFERRED SHADING 0 for PERFORMANCE
r.TiledDeferredShading.MinimumCount=80;--------------------------default 80
r.SSR.Quality=0;--------------------------SSR 0 for PERFORMANCE
r.SSR.HalfResSceneColor=0;--------------------------1 for PERFORMANCE
r.SSR.MaxRoughness=0.8;
r.SSGI.Enable=0;
r.SSGI.Quality=0;--------------------------SSGI 1 to 4 QUALITY VALUES 0 off
r.SSGI.HalfRes=0;--------------------------1 for PERFORMANCE
r.SSGI.LeakFreeReprojection=0;--------------------------default 0
r.SubsurfaceScattering=1;--------------------------SSS 0 for PERFORMANCE
r.SSS.Scale=1;--------------------------default 1
r.SSS.SampleSet=2;--------------------------0 for PERFORMANCE default 2
r.SSS.Quality=0;--------------------------default 0
r.SSS.HalfRes=0;--------------------------1 for PERFORMANCE
r.SSS.Filter=1;
r.SSS.Checkerboard=1;
r.ParticleLightQuality=2;--------------------------PARTICLES 0 or 1 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=10;
r.EmitterSpawnRateScale=1;--------------------------0.25 or 0.5 for PERFORMANCE
FX.QualityLevelSpawnRateScaleReferenceLevel=2;--------------------------TEST 0 or 1 for PERFORMANCE default 2
FX.BatchAsync=0;--------------------------TEST
FX.BatchAsyncBatchSize=32;--------------------------default 32
FX.AllowAsyncTick=1;
FX.EarlyScheduleAsync=0;--------------------------TEST
FX.AllowCulling=1;
r.MaxAnisotropy=8;
r.TessellationAdaptivePixelsPerTriangle=48;--------------------------9999999 for PERFORMANCE default 48
r.MaterialQualityLevel=1;--------------------------0 for PERFORMANCE
r.DetailMode=1;--------------------------0 for PERFORMANCE
r.RefractionQuality=1;--------------------------0 or 1 for PERFORMANCE default 2
r.IrisNormal=1;--------------------------0 for PERFORMANCE
r.DepthOfFieldQuality=0;--------------------------DOF 0 for PERFORMANCE
r.Filter.SizeScale=1;--------------------------default 1
r.Filter.NewMethod=1;
r.Filter.LoopMode=0;
r.BloomQuality=3;--------------------------BLOOM
r.Bloom.HalfResolutionFFT=0;
r.Bloom.Cross=0;--------------------------use -0.7777 for ANAMORPHIC BLOOM default 0
r.MotionBlurQuality=0;
r.FastBlurThreshold=0;
r.LensFlareQuality=2;--------------------------LENS FLARES 0 for PERFORMANCE default 2
r.SceneColorFringeQuality=0;
r.SceneColorFringe.Max=-1;
grass.DensityScale=0.9;
grass.DisableDynamicShadows=0;--------------------------1 for PERFORMANCE
foliage.DensityScale=1;
foliage.LODDistanceScale=0.9;--------------------------0.9 for PERFORMANCE default 1
foliage.MinVertsToSplitNode=8192;--------------------------default 8192
foliage.DitheredLOD=1;
r.Decal.FadeDurationScale=1;--------------------------0.6 for PERFORMANCE default 1
r.Decal.FadeScreenSizeMult=1;
r.Decal.StencilSizeThreshold=0.1;--------------------------default 0.1


-----------end-----------


The TAA settings i use Copy/Paste over or experiment

r.MinRoughnessOverride=0;--------------------------0.2 WITHOUT TAA 0 WITH TAA
r.DefaultFeature.AntiAliasing=2;--------------------------1 FXAA 2 TAA 3 MSAA 0 off
r.PostProcessAAQuality=3;--------------------------1 to 2 FXAA 3-4 TAA 0 off
r.MSAACount=0;
r.TemporalAASamples=2;
r.TemporalAACurrentFrameWeight=1;
r.TemporalAA.R11G11B10History=0;--------------------------1 is EXPERIMENTAL
r.TemporalAA.Algorithm=0;--------------------------GEN 5 TAA 0 for PERFORMANCE
r.TemporalAA.Upsampling=0;--------------------------TAAU
r.TemporalAAUpsampleFiltered=0;
r.ScreenPercentage=100;--------------------------INPUT RESOLUTION PERCENTAGE for TAAU


-----------end-----------


Open Input.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Input.ini
Copy/Paste:  %localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Input.ini


edit input commands or add them

[/Script/Engine.InputSettings] 
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.2;--------------------------TEST default 0.2
ButtonRepeatDelay=0.1;
DoubleClickTime=0.25;--------------------------TEST


-----------end-----------


Open GameUserSettings.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/GameUserSettings.ini


here are a few things to look for or tweak these overwrite engine.ini commands unfortunately

MaxFPS=163
FrameRateLimit=163
TextureStreamPoolSizeStorage=2048;--------------------------important for squad
ResolutionScaleModifier=1
DFAO=
DistanceFieldShadows=1
Gamma=2.2
bRTXEnabled=True
bRTXReflectionsEnabled=False
bRTXShadowsEnabled=False
bRTXAmbientOcclusionEnabled=False
DlssQualitySetting=1
bTelemetryEnabled=0
bUseVSync=0 
DesiredScreenWidth=
DesiredScreenHeight=
FullscreenMode=0
HDRDisplayOutputNits=
bUseDynamicResolution=0
AudioQualityLevel=3
FrameRateLimit=            
MenuFrameRateLimit=
MaxAnisotropy=
ContactShadows=0
PostFX_Saturation=1.2
PostFX_Sharpness=0
OverrideOptions=(("r.somerandomcommand", (Value=0,bModified=True)),("r.someotherrandomcommand", (Value=0,bModified=False)));--------------------------if you want to override from GameUserSettings.ini


set your scalability groups

0=low/1=medium/2=high/3=epic/4=cinematic (4 gets clamped)

[ScalabilityGroups]
sg.ResolutionQuality=100.000000
sg.ViewDistanceQuality=3
sg.ViewDistanceQuality.NumLevels=3
sg.AntiAliasingQuality=3
sg.AntiAliasingQuality.NumLevels=3
sg.PostProcessQuality=3
sg.PostProcessQuality.NumLevels=3
sg.ShadowQuality=3
sg.ShadowQuality.NumLevels=3
sg.TextureQuality=3
sg.TextureQuality.NumLevels=3
sg.EffectsQuality=3
sg.EffectsQuality.NumLevels=3
sg.FoliageQuality=3
sg.FoliageQuality.NumLevels=3
sg.ShadingQuality=3
sg.ShadingQuality.NumLevels=3
sg.AnimationQuality=3
sg.AnimationQuality.NumLevels=3


-----------end-----------


Open DeviceProfiles.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
Copy/Paste:  %localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/DeviceProfiles.ini


textures or you can just use in game settings (sg.TextureQuality=) copy and paste

[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverag,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=256,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)


-----------end-----------


for NVIDIA users:

Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method)

Adjust image settings set to Performance and apply then Select Use the advanced 3D image settings and apply

In manage 3D settings:

Anisotropic filtering:  Off for perf. App-controlled or force your own setting for quality

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


-----------end-----------


How to enable Message-signaled interrupts (MSIs):

use Wtools v1.0.2.0.exe (Wagnardsoft Tools) enable it and restart

or 

find ID: open device manager right click your GPU properties and click on events tab

looks like this:

HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties

find in regedit and set MSISupported to 1 then restart


~~~~~~~~~~~~~~~~~~~~~~~~~
