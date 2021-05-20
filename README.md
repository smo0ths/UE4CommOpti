~~~~~~~~~~~~~~~~~~~~~~~~~


*Updated 5/19/2021

*For UE4 games for reference/customization/optimization/learning

*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Engine.ini


my config is more of a quality balance you may need to tweak some commands, copy and paste under code

*testing r.SSGI.Enable=1 right now

[Core.Log]
Global=off;

[Audio]
MaxChannels=96; 32 64 96 128 test
CommonAudioPoolSize=0; default 0
UnfocusedVolumeMultiplier=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=38; texturePool cache percentage not enough will cause low quality textures

[/Script/Engine.StreamingSettings]
s.AsyncLoadingThreadEnabled=1;

[SystemSettings]
r.setres=2560x1440f; SET YOUR RESOLUTION
FX.BatchAsync=1;
FX.AllowAsyncTick=1;
FX.EarlyScheduleAsync=1;
FX.BatchAsyncBatchSize=32;
FX.AllowCulling=1;
FX.AllowGPUParticles=1;
FX.AllowGPUSorting=1;
AudioThread.UseBackgroundThreadPool=1;
r.Atmosphere=1;
r.VSync=0;
r.AllowHDR=0;
r.HDR.EnableHDROutput=0;
r.GPUCrashDebugging=0;
r.AsyncPipelineCompile=1;
r.XGEShaderCompile=1;
r.CompileShadersForDevelopment=0;
r.CreateShadersOnLoad=1;
r.EarlyZPass=2; default 3
r.EarlyZPassMovable=1;
r.EarlyZPassOnlyMaterialMasking=1;
r.FinishCurrentFrame=0;
r.GTSyncType=0;
rhi.SyncSlackMS=0;
r.RHICmdBypass=0;
r.D3D11.Depth24Bit=1;
r.DrawRectangleOptimization=1;
r.AlsoUseSphereForFrustumCull=1;
r.bForceCPUAccessToGPUSkinVerts=1; test
r.DeferSkeletalDynamicDataUpdateUntilGDME=1; 1 is EXPERIMENTAL
r.DoInitViewsLightingAfterPrepass=1; 1 is EXPERIMENTAL
r.DoLazyStaticMeshUpdate=1; 1 is EXPERIMENTAL
r.DiscardUnusedQuality=0; default 0
r.RenderTargetPoolMin=600; test
r.SelectiveBasePassOutputs=1;
r.OptimizeForUAVPerformance=0; faster but uses more gpu memory default 0
r.MorphTarget.Mode=1; 0 cpu method 1 gpu method default 1
r.ForwardShading=0;
r.SupportSimpleForwardShading=0;
r.SimpleForwardShading=0;
r.VertexFoggingForOpaque=1;
r.ShaderComplexity.CacheShaders=1;
r.GenerateMeshDistanceFields=1; 0 for PERFORMANCE
r.NormalMapsForStaticLighting=0;
r.GenerateLandscapeGIData=0;
r.DistanceFieldGI=0;
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1;
r.DBuffer=0; decal material blend modes 0 for PERFORMANCE default 1
r.AllowGlobalClipPlane=0;
r.LightPropagationVolume=0;
r.HZBOcclusion=0; occlusion culling algorithm default 1
r.AllowOcclusionQueries=1;
r.OneFrameThreadLag=1; 1 game sync with render thread
r.AllowSubPrimitiveQueries=1;
r.MinScreenRadiusForLights=0.03; default 0.03
r.MinScreenRadiusForDepthPrepass=0.03; default 0.03
r.MinScreenRadiusForCSMDepth=0.01;
r.MinScreenRadiusForSmallLights=0.01;
r.SceneColorFormat=3; 3 for PERFORMANCE default 4
r.DefaultBackBufferPixelFormat=4; default 4
r.ClearSceneMethod=1;
r.GBufferFormat=1; 1 to 3 QUALITY VALUES default 1
r.LightFunctionQuality=1; 0 for PERFORMANCE default 2
r.ClearCoatNormal=0; 0 for PERFORMANCE
Compat.UseDXT5NormalMaps=0;
r.SkyLightingQuality=1;
r.SupportStationarySkylight=1;
r.SkylightIntensityMultiplier=1; lower to darken skylight
r.LightMaxDrawDistanceScale=1; dynamic lights lod scale 0 for PERFORMANCE
r.MipMapLODBias=0; lods
r.LandscapeLODBias=0; 1 for PERFORMANCE
r.SkeletalMeshLODBias=0;
r.ParticleLODBias=-1;
r.ViewDistanceScale=1; view distance 0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;
r.SkeletalMeshLODRadiusScale=1; highest 0.25 low 1 default 1
r.StaticMeshLODDistanceScale=0.75; highest 0.25 low 1 default 1
r.SplineMesh.NoRecreateProxy=1;
r.TextureStreaming=1; texture streaming
r.Streaming.UseBackgroundThreadPool=1;
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.UseFixedPoolSize=0;
r.Streaming.LimitPoolSizeToVRAM=1;
r.Streaming.PoolSize=3000;
r.Streaming.UseAllMips=0;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.Boost=1;
r.Streaming.MipBias=0;
r.Streaming.UsePerTextureBias=1;
r.Streaming.AmortizeCPUToGPUCopy=1;
r.Streaming.MaxNumTexturesToStreamPerFrame=5;
r.Streaming.NumStaticComponentsProcessedPerFrame=50;
r.Streaming.FullyLoadUsedTextures=0;
r.Streaming.DefragDynamicBounds=1;
r.Streaming.ScaleTexturesByGlobalMyBias=1;
r.Streaming.HiddenPrimitiveScale=0.5; default 0.5
r.Streaming.HLODStrategy=0;
r.Streaming.UseNewMetrics=1;
r.Streaming.MinMipForSplitRequest=1;
r.Streaming.UseMaterialData=1;
r.DistanceFieldAO=0; 1 for dfao
r.ShadowQuality=3; shadows
r.Shadow.FilterMethod=0;
r.Shadow.TransitionScale=1;
r.Shadow.SpotLightTransitionScale=1;
r.Shadow.MaxResolution=1024;
r.Shadow.MaxCSMResolution=2048;
r.Shadow.CSM.MaxCascades=2; 1 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1;
r.Shadow.RadiusThreshold=0.03;
r.Shadow.DistanceScale=0.85; lower for PERFORMANCE
r.Shadow.PreShadowResolutionFactor=0.5; 0.5 for PERFORMANCE
r.ContactShadows=0; 0 for PERFORMANCE
r.ContactShadows.NonShadowCastingIntensity=0.2;
r.CapsuleShadows=0;
r.AllowLandscapeShadows=1; landscape shadows 0 for PERFORMANCE
r.DistanceFieldShadowing=1; distance field shadowing 0 for PERFORMANCE
r.DFShadowQuality=1; 1 to 2 QUALITY VALUES 0 off
r.Shadow.MaxNumFarShadowCascades=0; 0 for PERFORMANCE
r.DFFullResolution=0; 0 for PERFORMANCE
r.DFShadowScatterTileCulling=1; 1 is OPTIMAL
r.DFTwoSidedMeshDistanceBias=0;
r.Tonemapper.Quality=2;
r.TonemapperFilm=1;
r.Tonemapper.GrainQuantization=1; fights 8 bit color banding default 1
r.Tonemapper.Sharpen=0;
r.Tonemapper.MergeWithUpscale.Mode=0;
r.MinRoughnessOverride=0; 0.2 with no AA 0 with
r.DefaultFeature.AntiAliasing=2; 0 off 1 FXAA 2 TAA 3 MSAA
r.PostProcessAAQuality=3; 0 off 1 to 2 FXAA 3 to 6 TAA
r.MSAACount=0;
r.TemporalAASamples=4;
r.TemporalAAFilterSize=1;
r.TemporalAACurrentFrameWeight=0;
r.TemporalAA.R11G11B10History=1; 1 is EXPERIMENTAL
r.TemporalAA.Algorithm=1; 1 is EXPERIMENTAL
r.TemporalAA.Upsampling=0; TAAU
r.TemporalAAUpsampleFiltered=0;
r.ScreenPercentage=100; input resolution percentage for TAAU
r.SceneRenderTargetResizeMethod=0; default 0
r.SceneCaptureResizeMethod=0; default 0
r.Upscale.Quality=1;
r.EnableAsyncComputeTranslucencyLightingVolumeClear=1;
r.TranslucencyLightingVolume=1; translucency
r.TranslucencyVolumeBlur=1;
r.TranslucencyLightingVolumeDim=32;
r.SeparateTranslucency=1;
r.SeparateTranslucencyScreenPercentage=100;
r.SeparateTranslucencyAutoDownsample=1;
r.TranslucentSortPolicy=0;
r.AmbientOcclusionLevels=0; ssao 0 for PERFORMANCE
r.DefaultFeature.AmbientOcclusionStaticFraction=0; 0 for PERFORMANCE
r.AmbientOcclusionStaticFraction=0; 0 for PERFORMANCE
r.AmbientOcclusionMipLevelFactor=0.5;
r.AmbientOcclusionMaxQuality=0;
r.AmbientOcclusionSampleSetQuality=-1;
r.AmbientOcclusion.Compute=0;
r.AmbientOcclusionRadiusScale=0;
r.LightShaftQuality=0; lightshafts 0 for PERFORMANCE
r.LightShaftDownSampleFactor=0;
r.LightShaftFirstPassDistance=0.1;
r.LightShaftBlurPasses=2;
r.LightShaftNumSamples=1;
r.SupportSkyAtmosphere=1;
r.SupportSkyAtmosphereAffectsHeightFog=1;
r.SupportAtmosphericFog=1;
r.Fog=1;
r.VolumetricFog=0; 0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=32;
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.HistoryWeight=0.9;
r.VolumetricFog.InjectShadowedLightsSeparately=0;
r.VolumetricFog.TemporalReprojection=1;
r.VolumetricFog.HistoryMissSupersampleCount=1;
r.ReflectionEnvironment=1; reflection environment 0 for PERFORMANCE
r.HalfResReflections=1;
r.chaos.ReflectionCaptureStaticSceneOnly=1; 1 for PERFORMANCE
r.ReflectionCaptureGPUArrayCopy=1;
r.ReflectionCaptureResolution=128; default 128
r.TiledDeferredShading=1; tiled deferred shading 0 for PERFORMANCE
r.TiledDeferredShading.MinimumCount=20;
r.DoTiledReflections=0; tiled reflection 0 for PERFORMANCE
r.NoTiledReflections=0;
r.SSR.Quality=0; ssr 0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; 1 for PERFORMANCE
r.SSR.MaxRoughness=0.8;
r.SSGI.Enable=1; screen space global illumination 0 for PERFORMANCE
r.SSGI.Quality=1; 1 to 4 QUALITY VALUES 0 off
r.SSGI.HalfRes=0; 1 for PERFORMANCE
r.SSGI.LeakFreeReprojection=0; default 0
r.SubsurfaceScattering=1; sss 0 for PERFORMANCE
r.SSS.Scale=1;
r.SSS.SampleSet=0;
r.SSS.Quality=0;
r.SSS.HalfRes=1;
r.SSS.Filter=1;
r.SSS.Checkerboard=1;
r.ParticleLightQuality=1; particles 0 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=10;
r.EmitterSpawnRateScale=0.5; 0.25 for PERFORMANCE
r.Emitter.FastPoolEnable=1;
r.DefaultFeature.AutoExposure=1; eye adaptation
r.DefaultFeature.AutoExposure.Method=1;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0;
r.EyeAdaptationQuality=1;
r.UsePreExposure=0;
r.EyeAdaptation.PreExposureOverride=0;
r.MaxAnisotropy=8;
r.SupportMaterialLayers=0;
ShowFlag.Tessellation=0; 0 for PERFORMANCE
r.TessellationAdaptivePixelsPerTriangle=9999999; 9999999 for PERFORMANCE 48 for QUALITY
r.MaterialQualityLevel=1; 0 for PERFORMANCE
r.DetailMode=2; 0 for PERFORMANCE
r.RefractionQuality=1; 0 for PERFORMANCE default 2
r.IrisNormal=0; 0 for PERFORMANCE
r.DepthOfFieldQuality=1; dof 0 for PERFORMANCE
r.Filter.SizeScale=1;
r.BloomQuality=3; bloom
r.Bloom.HalfResoluionFFT=0;
r.Bloom.Cross=0;
r.BlurGBuffer=0;
r.MotionBlurQuality=0;
r.FastBlurThreshold=7;
r.LensFlareQuality=0; lens flares
r.SceneColorFringeQuality=0;
r.SceneColorFringe.Max=-1;
grass.DensityScale=0.6;
grass.DisableDynamicShadows=0; 1 for PERFORMANCE
grass.TickInterval=10;
foliage.DensityScale=0.6; 0.6 for PERFORMANCE
foliage.MinVertsToSplitNode=8192;
ShowFlag.Vignette=0;
r.Decal.FadeDurationScale=1; default 1
r.Decal.FadeScreenSizeMult=1;
r.Decal.StencilSizeThreshold=0.1; default 0.1


-----------end-----------

Open Input.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Input.ini


edit input commands or add them

[/Script/Engine.InputSettings] 
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.1;
ButtonRepeatDelay=0.1;


-----------end-----------


Open GameUserSettings.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/GameUserSettings.ini


here are a few things to look for or tweak these overwrite engine.ini commands unfortunately

bUseVSync=0 
FullscreenMode=1
HDRDisplayOutputNits=
bUseDynamicResolution=0
AudioQualityLevel=3
FrameRateLimit=            
MenuFrameRateLimit=
MaxAnisotropy=
ContactShadows=0
PostFX_Saturation=1.200000
PostFX_Sharpness=0.000000
DistanceFieldShadows=1
TextureStreamPoolSizeStorage=3000
OverrideOptions=(("r.somerandomcommand", (Value=0,bModified=True)),("r.someotherrandomcommand", (Value=0,bModified=False))) ; if you want to override from GameUserSettings.ini


set your scalability groups

[ScalabilityGroups]
sg.ResolutionQuality=100.000000
sg.ViewDistanceQuality=0
sg.AntiAliasingQuality=0
sg.ShadowQuality=0
sg.PostProcessQuality=0
sg.TextureQuality=0
sg.EffectsQuality=0
sg.FoliageQuality=0
sg.ShadingQuality=0


-----------end-----------


Open DeviceProfiles.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini


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


-----------end-----------


for NVIDIA users

Reset settings "apply let the 3D app decide" then set "use the advanced 3D image settings" then apply, click take me there
Low latency mode:  off  (lower than ~85% gpu for lowest input lag)
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
TF anisotropic sample optimization:  On
TF Negative LOD bias:  Allow
Texture filtering quality:  High performance
Vertical sync:  Off


~~~~~~~~~~~~~~~~~~~~~~~~~
