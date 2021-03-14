~~~~~~~~~~~~~~~~~~~~~~~~~


*Updated 3/14/2021~

*For UE4 games for reference/customization/optimization/learning

*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini and copy/paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Engine.ini


My config:

[Core.Log]
Global=off;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=70;---------texturePool cache lower if vram runs OOM

[/Script/Engine.StreamingSettings]
s.AsyncLoadingThreadEnabled=1;

[SystemSettings]
FX.BatchAsync=1;
FX.AllowAsyncTick=1;
FX.EarlyScheduleAsync=1;
FX.BatchAsyncBatchSize=9999999;
FX.AllowCulling=1;
FX.AllowGPUParticles=1;
FX.AllowGPUSorting=1;
FX.MaxCPUParticlesPerEmitter=50;
FX.MaxGPUParticlesSpawnedPerFrame=512;
FX.GPUSpawnWarningThreshold=1024;
AudioThread.BatchAsyncBatchSize=9999999;
AudioThread.UseBackgroundThreadPool=1;
AudioThread.EnableBatchProcessing=1;
r.Atmosphere=1;
r.setres=1920x1080wf;
r.VSync=0;
r.AllowHDR=0;
r.HDR.EnableHDROutput=0;
r.GPUCrashDebugging=0;
r.bForceCPUAccessToGPUSkinVerts=1;---------more cpu usage
r.DeferSkeletalDynamicDataUpdateUntilGDME=1;---------1 is experimental option
r.CompileShadersForDevelopment=0;
r.CreateShadersOnLoad=1;
r.EarlyZPass=3;
r.EarlyZPassMovable=1;
r.EarlyZPassOnlyMaterialMasking=1;---------always 1
r.FinishCurrentFrame=0;
r.OneFrameThreadLag=1;----------default 1 game sync w render thread
r.GTSyncType=0;
rhi.SyncSlackMS=0;
r.RHICmdBypass=0;
r.DrawRectangleOptimization=1;
r.AlsoUseSphereForFrustumCull=1;
r.DoLazyStaticMeshUpdate=1;
r.DiscardUnusedQuality=1;
r.VertexFoggingForOpaque=0;
r.ForceAllCoresForShaderCompiling=0;---------1 could run faster but use a lot of mem
r.AllowCachedUniformExpressions=1;
r.Cache.LimitQuerySize=1;
r.Cache.LightingCacheMovableObjectAllocationSize=3;
r.D3D11.Depth24Bit=1;
r.VirtualTexture=1;
r.VirtualTexturedLightmaps=1;
r.VirtualTextureReducedMemory=1;---------
r.VT.TileSize=64;---------
r.VT.TileBorderSize=2;---------
r.VT.FeedbackFactor=16;---------
r.VT.EnableCompressZlib=1;---------
r.VT.EnableCompressCrunch=1;---------
r.IncludeNonVirtualTexturedLightmaps=0;---------
r.VT.PoolSizeScale=0.5;---------
r.VT.MaxUploadsPerFrame=1;---------
r.VT.RVT.TileCountBias=0;---------
r.VT.EnableLossyCompressLightmaps=0;---------
r.VT.MaxAnisotropy=0;---------
r.ShaderComplexity.CacheShaders=1;
r.MorphTarget.Mode=1;---------default 1 gpu method
r.AllowStaticLighting=0;---------1 for SANDSTORM
r.GenerateMeshDistanceFields=1;---------0 for PERFORMANCE
r.NormalMapsForStaticLighting=0;
r.DistanceFieldBuild.EightBit=0;
r.GenerateLandscapeGIData=1;---------0 for PERFORMANCE
r.DistanceFieldGI=0;
r.AOAsyncBuildQueue=1;
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1;
r.AOComputeShaderNormalCalculation=1;
r.DistanceFieldBuild.Compress=0;---------1 for GROUND BRANCH and other games if you crash
r.SSGI.Quality=0;----------0 for PERFORMANCE 1 to 4 quality levels for screen space global illumination
r.SSGI.HalfRes=0;----------1 for PERFORMANCE
r.SSGI.LeakFreeReprojection=1;----------1 for better quality results
r.DBuffer=1;---------decals 0 for PERFORMANCE
r.AllowGlobalClipPlane=0;
r.LightPropagationVolume=0;
r.RenderTargetPoolMin=256;
r.OptimizeForUAVPerformance=0;---------1 can render targets faster but use more GPU vram
r.DoInitViewsLightingAfterPrepass=1;---------1 is a experimental optimization
r.HZBOcclusion=0;---------occlusion culling algorithm
r.AllowOcclusionQueries=1;
r.NumBufferedOcclusionQueries=0;
r.AllowSubPrimitiveQueries=1;
r.MinScreenRadiusForLights=0.03;
r.MinScreenRadiusForDepthPrepass=0.03;
r.MinScreenRadiusForCSMDepth=0.01;
r.MinScreenRadiusForSmallLights=0.01;
r.SceneColorFormat=4;---------3 for PERFORMANCE
r.DefaultBackBufferPixelFormat=4;---------0 for PERFORMANCE
r.ClearSceneMethod=1;
r.GBufferFormat=1;---------0 8bit per component 1 is default
r.IndirectLightingCache=1;
r.LightFunctionQuality=1;---------0 for PERFORMANCE
r.ClearCoatNormal=0;---------0 for PERFORMANCE
Compat.UseDXT5NormalMaps=0;
r.HighQualityLightMaps=1;
r.SupportLowQualityLightmaps=1;
r.SupportStationarySkylight=1;
r.SkyLightingQuality=1;---------0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1;---------0 or 0.5 for PERFORMANCE
r.MipMapLODBias=0;---------lods
r.LandscapeLODBias=0;---------1 for PERFORMANCE
r.SkeletalMeshLODBias=0;
r.ParticleLODBias=-1;
r.ViewDistanceScale=1;---------view distance 0.8 for PERFORMANCE
r.ViewDistanceScale.SecondaryScale=0;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;
r.SkeletalMeshLODRadiusScale=1;
r.StaticMeshLODDistanceScale=1;
r.SplineMesh.NoRecreateProxy=1;
r.TextureStreaming=1;---------texture streaming
r.Streaming.UseBackgroundThreadPool=1;
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.MaxTempMemoryAllowed=128;
r.Streaming.UseFixedPoolSize=0;
r.Streaming.LimitPoolSizeToVRAM=1;
r.Streaming.PoolSize=3000;
r.Streaming.UseAllMips=0;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.Boost=1;
r.Streaming.MipBias=0;
r.Streaming.UsePerTextureBias=1;
r.Streaming.AmortizeCPUToGPUCopy=0;
r.Streaming.MaxNumTexturesToStreamPerFrame=0;
r.Streaming.NumStaticComponentsProcessedPerFrame=50;
r.Streaming.FullyLoadUsedTextures=0;
r.Streaming.DefragDynamicBounds=1;
r.Streaming.ScaleTexturesByGlobalMyBias=1;
r.Streaming.HiddenPrimitiveScale=0;
r.Streaming.HLODStrategy=0;
r.Streaming.UseNewMetrics=1;
r.Streaming.MinMipForSplitRequest=1;
r.Streaming.UseMaterialData=1;
r.HLOD=0;
r.HLOD.MaximumLevel=-1;
r.HLOD.DistanceScale=1;
r.HLOD.DistanceOverride=10000;
r.DistanceFieldAO=0;---------1 for DFAO
r.AOQuality=0;---------1-2 for DFAO
r.SkySpecularOcclusionStrength=1;---------1 is default for DFAO
r.AOObjectDistanceField=0;
r.AOGlobalDistanceField=1;----------1 optimize occlusion cone traces test
r.AOUseSurfaceCache=0;----------1 older method
r.AOSpecularOcclusionMode=1;
r.AOApplyToStaticIndirect=0;
r.AOHeightfieldOcclusion=0;
r.ShadowQuality=4;---------shadows 0 for no shadows
r.Shadow.FilterMethod=0;
r.Shadow.CSM.MaxCascades=2;
r.Shadow.CSM.TransitionScale=1;
r.Shadow.PreShadowResolutionFactor=1;---------0.5 for PERFORMANCE
r.Shadow.PreShadowFadeResolution=64;
r.Shadow.MinPreShadowResolution=32;
r.Shadow.FadeResolution=64;
r.Shadow.MinResolution=32;
r.Shadow.MaxResolution=1024;
r.Shadow.MaxCSMResolution=2048;
r.Shadow.RadiusThreshold=0.01;
r.Shadow.RadiusThresholdRSM=0.06;
r.Shadow.DistanceScale=0.6;---------0.6 for PERFORMANCE
r.Shadow.ForceSingleSampleShadowingFromStationary=0;
r.Shadow.CachePreshadow=1;
r.Shadow.CacheWholeSceneShadows=1;
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;
r.Shadow.CacheWPOPrimitives=1;
r.Shadow.UnbuiltPreviewInGame=0;
r.Shadow.PerObject=1;
r.Shadow.PerObjectDirectionalDepthBias=0.5;
r.Shadow.CSMDepthBias=5;
r.Shadow.ConservativeBounds=1;
r.SupportPointLightWholeSceneShadows=1;
r.AllowPointLightCubemapShadows=1;
r.ParallelShadow=1;---------0 for PERFORMANCE
r.ParallelShadowsNonWholeScene=0;
r.ContactShadows=0;
r.CapsuleShadows=0;
r.AllowLandscapeShadows=1;---------0 for PERFORMANCE
r.DistanceFieldShadowing=1;---------0 for PERFORMANCE
r.DFShadowQuality=1;---------1 or 2 quality level 0 for PERFORMANCE
r.DFFullResolution=0;---------0 for PERFORMANCE
r.DFShadowScatterTileCulling=1;----------1 is optimal
r.DistanceFields.ForceMaxAtlasSize=1;
r.AOGlobalDistanceFieldCacheMostlyStaticSeparately=1;
r.DFTwoSidedMeshDistanceBias=0;
r.Tonemapper.Quality=2;
r.TonemapperFilm=1;
r.Tonemapper.GrainQuantization=1;---------0 if using HDR
r.Tonemapper.Sharpen=0.7;
r.DefaultFeature.AntiAliasing=2;---------2 for TAA 1 for FXAA
r.PostProcessAAQuality=3;---------0-off 1-2-FXAA 3-4-5-6-TAA i use 3 for TAA 1 for FXAA
r.MSAA.CompositingSampleCount=1;
r.TemporalAASamples=8;
r.TemporalAAFilterSize=0.25;---------only works with 6+ TAA samples
r.TemporalAACurrentFrameWeight=0.2;
r.TemporalAA.R11G11B10History=0;
r.TemporalAA.Algorithm=1;---------Gen 5 TAA
r.TemporalAA.Upsampling=0;---------allow Gen 5 TAAU
r.TemporalAAUpsampleFiltered=1;---------0 makes TAAU faster
r.SceneRenderTargetResizeMethod=0;
r.ScreenPercentage=100;---------lower input res for Gen 4 or 5 TAA i use 86.66 if using TAA
r.Upscale.Quality=1;
r.Upscale.Softness=1;
r.AmbientOcclusionLevels=2;---------ssao 0 for no ssao
r.AmbientOcclusionStaticFraction=0;
r.AmbientOcclusionMipLevelFactor=0.5;
r.AmbientOcclusionMaxQuality=100;
r.AmbientOcclusionSampleSetQuality=0;
r.AmbientOcclusion.Compute=0;
r.AmbientOcclusionRadiusScale=0;
r.LightShaftQuality=0;---------lightshafts
r.LightShaftDownSampleFactor=0;
r.LightShaftFirstPassDistance=0.1;
r.LightShaftBlurPasses=2;
r.LightShaftNumSamples=1;
r.LightShaftRenderToSeparateTranslucency=0;
r.TranslucencyLightingVolume=1;---------translucency
r.TranslucencyVolumeBlur=1;
r.TranslucencyLightingVolumeDim=32;
r.SeparateTranslucency=1;
r.SeparateTranslucencyScreenPercentage=100;
r.SeparateTranslucencyAutoDownsample=1;
r.TranslucentSortPolicy=0;
r.CustomDepth=3;
r.CustomDepth.Order=0;---------0 more efficient with async 1 is default
r.SupportSkyAtmosphere=1;
r.SupportSkyAtmosphereAffectsHeightFog=0;
r.SupportAtmosphericFog=1;---------fog
r.Fog=1;
r.VolumetricFog=1;---------0 for PERFORMANCE
r.VolumetricFog.GridPixelSize=16;
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.HistoryWeight=0.9;
r.VolumetricFog.InjectShadowedLightsSeparately=0;
r.VolumetricFog.TemporalReprojection=1;
r.ReflectionEnvironment=1;---------reflection environment 0 for PERFORMANCE
r.HalfResReflections=0;---------1 for halfres reflection environment and PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;
r.ReflectionEnvironmentBeginMixingRoughness=0.1;
r.ReflectionEnvironmentEndMixingRoughness=0.3;
r.ReflectionEnvironmentLightmapMixing=1;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000;
r.chaos.ReflectionCaptureStaticSceneOnly=1;
r.DoTiledReflections=1;---------tiled reflection
r.NoTiledReflections=0;
r.ReflectionCaptureGPUArrayCopy=1;
r.ReflectionCaptureResolution=128;
r.SSR.Quality=1;---------ssr 0 for PERFORMANCE
r.SSR.Temporal=1;
r.SSR.HalfResSceneColor=1;
r.SSR.MaxRoughness=0.8;
r.SubsurfaceScattering=1;---------sss 0 for PERFORMANCE
r.SSS.Scale=3;
r.SSS.SampleSet=0;
r.SSS.Quality=0;
r.SSS.HalfRes=1;
r.SSS.Filter=1;
r.SSS.Checkerboard=1;
r.ParticleLightQuality=1;---------particles 0 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=8;---------16 for around 60 fps
r.EmitterSpawnRateScale=1;---------0.25 for PERFORMANCE
r.Emitter.FastPoolEnable=1;
r.TiledDeferredShading=1;---------tiled deferred shading
r.TiledDeferredShading.MinimumCount=80;
r.DefaultFeature.AutoExposure=0;---------eye adaptation
r.DefaultFeature.AutoExposure.Method=0;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0;
r.EyeAdaptationQuality=2;
r.UsePreExposure=0;
r.EyeAdaptation.PreExposureOverride=0;
r.MaxAnisotropy=8;
r.SupportMaterialLayers=0;
r.TessellationAdaptivePixelsPerTriangle=9999999;---------9999999 for PERFORMANCE
r.MaterialQualityLevel=1;---------0 for PERFORMANCE
r.DetailMode=2;---------0 for PERFORMANCE
r.RefractionQuality=1;---------0 for PERFORMANCE
r.IrisNormal=1;---------0 for PERFORMANCE
r.DepthOfFieldQuality=1;---------dof
r.DOF.Recombine.Quality=2;
r.Filter.NewMethod=1;
r.Filter.SizeScale=1;
r.DOF.Algorithm=1;
r.BloomQuality=3;---------bloom
r.Bloom.HalfResoluionFFT=1;
r.MotionBlurQuality=0;
r.FastBlurThreshold=7;
r.LensFlareQuality=0;
r.SceneColorFringeQuality=0;
r.SceneColorFringe.Max=-1;
grass.DensityScale=0.6;
grass.DisableDynamicShadows=0;---------1 for PERFORMANCE
foliage.DensityScale=0.6;
foliage.DitheredLOD=1;
ShowFlag.Vignette=0;
ShowFlag.SceneColorFringe=0;
r.DefaultFeature.LightUnits=1;


-----------end-----------


Open Input.ini

%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/Insurgency/Saved/Config/WindowsClient/Input.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Input.ini


Edit input commands copy/paste: 

[/Script/Engine.InputSettings] 
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.1;
ButtonRepeatDelay=0.1;


-----------end-----------


Open GameUserSettings.ini

%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/Insurgency/Saved/Config/WindowsClient/GameUserSettings.ini 
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/GameUserSettings.ini


settings in here are in game options, they will overwrite your engine.ini yay jk, change them before starting game to get disired setting, don't add unless you are using OverrideOptions:

bUseVSync=0 
FullscreenMode=1
bUseDynamicResolution=0
AudioQualityLevel=3
LastConfirmedAudioQualityLevel=3
FrameRateLimit=0
MenuFrameRateLimit=0
MaxCSMResolution=4096
MaxAnisotropy=8
ContactShadows=0
PostFX_Saturation=1.200000
BloomQuality=3
LensFlareQuality=0
AmbientOcclusion=1
AmbientOcclusionStaticFraction=0
AmbientOcclusionLevels=2
AmbientOcclusionRadiusScale=0.000000
AutoExposure=0
EyeAdaptationQuality=0
DistanceFieldShadows=1
TextureStreamPoolSizeStorage=3000
OverrideOptions=(("r.somerandomcommand", (Value=0,bModified=True)),("r.someotherrandomcommand", (Value=0,bModified=False)))

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

%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
%localappdata%/Insurgency/Saved/Config/WindowsClient/DeviceProfiles.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini


Textures or you can just use in game settings (sg.TextureQuality=) copy/paste:

[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverag,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=1,MaxLODSize=512,LODBias=0,MinMagFilter=linear,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=1,MaxLODSize=512,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=1,MaxLODSize=512,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=1,MaxLODSize=4096,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=512,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=-1)


-----------end-----------


for NVIDIA users:

Reset settings "apply let the 3D app decide" then set "use the advanced 3D image settings" then apply, click take me there
Anisotropic filter: 8x  (to make sure its on)
Low latency mode:  off  (lower than ~85% gpu for lowest input lag)
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
TF anisotropic sample optimization:  On
TF Negative LOD bias:  Clamp  (allow for performance as stated by nvidia)
Texture filtering quality:  High performance
Vertical sync:  Off


~~~~~~~~~~~~~~~~~~~~~~~~~
