~~~~~~~~~~~~~~~~~~~~~~~~~


*Updated 10/25/2020~~~     

*For UE4 games for reference/customization/optimization/learning

*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini and copy/paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 
Copy/Paste:  %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 


My config:

[Core.Log]
Global=off;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;

[TextureStreaming]
PoolSizeVRAMPercentage=40;

[SystemSettings]
Compat.UseDXT5NormalMaps=0;
r.VSync=0;
r.AllowHDR=0;
r.FinishCurrentFrame=0;
r.OneFrameThreadLag=1;
r.GTSyncType=0;
r.GPUCrashDebugging=0;
r.CompileShadersForDevelopment=0;
r.CreateShadersOnLoad=1;
r.RHICmdBypass=0;
r.RHICmdUseParallelAlgorithms=1;
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1;
r.EarlyZPass=3;
r.EarlyZPassMovable=1;
r.HZBOcclusion=0;
r.DoInitViewsLightingAfterPrepass=1;
r.ScreenPercentage=100;
r.SceneRenderTargetResizeMethod=0;
r.Upscale.Quality=0;
r.SceneColorFormat=3;
r.DefaultBackBufferPixelFormat=4;
r.GBufferFormat=1;
r.GenerateMeshDistanceFields=1;      0 for SANDSTORM
r.DistanceFieldBuild.EightBit=0;
r.DistanceFieldBuild.Compress=0;
r.AllowStaticLighting=0;      1 for SANDSTORM
r.NormalMapsForStaticLighting=0;
r.HighQualityLightMaps=1;
r.SupportLowQualityLightmaps=0;
r.GenerateLandscapeGIData=1;
r.TessellationAdaptivePixelsPerTriangle=9999999;
r.VirtualTexture=1;
r.VirtualTexturedLightmaps=1;
r.IncludeNonVirtualTexturedLightmaps=1;
r.VT.EnableLossyCompressLightmaps=0;
r.VirtualTextureReducedMemory=0;
r.AllowOcclusionQueries=1;
r.MinScreenRadiusForLights=0.03;
r.MinScreenRadiusForDepthPrepass=0.03;
r.MinScreenRadiusForCSMDepth=0.01;
r.MipMapLODBias=0;
r.LandscapeLODBias=0;
r.SkeletalMeshLODBias=0;
r.ParticleLODBias=-1;
r.MaxAnisotropy=16;
r.TextureStreaming=1;
r.RenderTargetPoolMin=400;
r.Streaming.PoolSize.VRAMPercentageClamp=1024;
r.Streaming.LimitPoolSizeToVRAM=1;
r.Streaming.UseFixedPoolSize=0;
r.Streaming.PoolSize=1000;
r.Streaming.UseAllMips=0;
r.Streaming.MipBias=0;
r.Streaming.UsePerTextureBias=1;
r.Streaming.AmortizeCPUToGPUCopy=0;
r.Streaming.MaxNumTexturesToStreamPerFrame=0;
r.Streaming.NumStaticComponentsProcessedPerFrame=50;
r.Streaming.Boost=1;
r.Streaming.FullyLoadUsedTextures=0;
r.Streaming.MaxEffectiveScreenSize=0;
r.Streaming.DefragDynamicBounds=1;
r.Streaming.ScaleTexturesByGlobalMyBias=1;
r.Streaming.HiddenPrimitiveScale=0;
r.Streaming.HLODStrategy=0;
r.ViewDistanceScale=0.8;
r.ViewDistanceScale.ApplySecondaryScale=0;
r.ViewDistanceScale.SecondaryScale=1;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;
r.SkeletalMeshLODRadiusScale=1;
r.StaticMeshLODDistanceScale=1;
r.HLOD=0;
r.HLOD.MaximumLevel=-1;
r.HLOD.DistanceScale=1;
r.HLOD.DistanceOverride=10000;
r.ShadowQuality=3;
r.Shadow.CSM.MaxCascades=1;
r.Shadow.CSM.TransitionScale=1;
r.Shadow.CSMShadowDistanceFadeoutMultiplier=1;
r.Shadow.MaxResolution=1024;
r.Shadow.MaxCSMResolution=2048;
r.Shadow.RadiusThreshold=0.04;
r.Shadow.DistanceScale=0.6;
r.Shadow.SpotLightTransitionScale=2048;
r.Shadow.CacheWholeSceneShadows=1;
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;
r.Shadow.ForceSingleSampleShadowingFromStationary=1;
r.ParallelShadow=0;
r.SupportPointLightWholeSceneShadows=0;
r.ParallelShadowsNonWholeScene=0;
r.AllowLandscapeShadows=1;      0 for PERFORMANCE
r.ContactShadows=0;
r.CapsuleShadows=0;
r.Tonemapper.Quality=2;      0 for SANDSTORM
r.TonemapperFilm=1;
r.Tonemapper.GrainQuantization=0;
r.Tonemapper.MergeWithUpscale.Mode=0;
r.TemporalAASamples=2;
r.TemporalAACurrentFrameWeight=0.2;
r.TemporalAA.Upsampling=0;
r.TemporalAASharpness=0;
r.DistanceFieldShadowing=1;      0 for PERFORMANCE 0 for SANDSTORM
r.DFShadowQuality=1;
r.DFTwoSidedMeshDistanceBias=0;
r.DFFullResolution=0;
r.DistanceFieldAO=0;
r.AOSpecularOcclusionMode=1;
r.AOApplyToStaticIndirect=0;
r.AOHeightfieldOcclusion=0;
r.AOQuality=0;
r.DefaultFeature.AmbientOcclusionStaticFraction=0;
r.AmbientOcclusionStaticFraction=0;
r.AmbientOcclusionMipLevelFactor=1;
r.AmbientOcclusionMaxQuality=100;
r.AmbientOcclusionLevels=2;      0 for PERFORMANCE
r.AmbientOcclusionSampleSetQuality=0;
r.AmbientOcclusion.Compute=0;
r.AmbientOcclusionRadiusScale=0;
r.AmbientOcclusion.FadeRadiusScale=0.6;
r.SupportStationarySkylight=1;
r.SkyLightingQuality=1;
r.LightPropagationVolume=0;
r.LightCulling.Quality=1;
r.LightFunctionQuality=1;
r.LightMaxDrawDistanceScale=0.5;      0 for PERFORMANCE
r.LightShaftQuality=1;
r.LightShaftDownSampleFactor=0;
r.LightShaftFirstPassDistance=0.1;
r.LightShaftBlurPasses=2;
r.LightShaftNumSamples=1;
r.LightShaftRenderToSeparateTranslucency=0;
r.TranslucencyLightingVolume=1;
r.TranslucencyVolumeBlur=1;
r.TranslucencyLightingVolumeDim=32;
r.SeparateTranslucency=0;
r.TranslucentSortPolicy=0;
r.SeparateTranslucencyScreenPercentage=100;
r.SeparateTranslucencyAutoDownsample=1;
r.SupportAtmosphericFog=1;
r.VolumetricFog=0;
r.VolumetricFog.GridPixelSize=16;
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.InjectShadowedLightsSeparately=0;
r.ReflectionEnvironment=1;      0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;
r.ReflectionCaptureResolution=128;
r.SSR.Quality=0;
r.SSR.HalfResSceneColor=1;
r.SSR.MaxRoughness=0.8;
r.MaterialQualityLevel=1;      0 for PERFORMANCE
r.SupportMaterialLayers=0;
r.IrisNormal=0;
r.SubsurfaceScattering=0;
r.SSS.Scale=0;
r.SSS.SampleSet=0;
r.SSS.Quality=-1;
r.SSS.HalfRes=1;
r.SSS.Filter=0;
r.SSS.Checkerboard=2;
r.DetailMode=2;      0 for PERFORMANCE
r.RefractionQuality=1;      0 for PERFORMANCE
r.ParticleLightQuality=1;      0 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=8;
r.EmitterSpawnRateScale=1;      0.25 for PERFORMANCE
r.Emitter.FastPoolEnable=1;
r.GpuSkin.Pool=1;
FX.MaxCPUParticlesPerEmitter=50;
FX.MaxGPUParticlesSpawnedPerFrame=512;
FX.GPUSimulationTextureSizeX=1024;
FX.GPUSimulationTextureSizeY=1024;
r.DoTiledReflections=1;
r.TiledDeferredShading=0;
r.TiledDeferredShading.MinimumCount=0;
r.LensFlareQuality=0;
r.MotionBlurQuality=0;
r.BloomQuality=3;
r.Filter.SizeScale=0;
r.DepthOfFieldQuality=0;
r.SceneColorFringeQuality=0;
r.SceneColorFringe.Max=0;
r.DefaultFeature.AutoExposure=1;      0 for PERFORMANCE
r.EyeAdaptationQuality=2;      0 for PERFORMANCE
r.DefaultFeature.AutoExposure.Method=0;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0;
grass.DensityScale=0.6;
foliage.DensityScale=0.6;


-----------end-----------


Open Input.ini

%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/Insurgency/Saved/Config/WindowsClient/Input.ini
%localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Input.ini


Edit input commands copy/paste: 

[/Script/Engine.InputSettings] 
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;


-----------end-----------


Open GameUserSettings.ini

%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/Insurgency/Saved/Config/WindowsClient/GameUserSettings.ini 
%localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/GameUserSettings.ini 


Some settings in here will overwrite Engine.ini so set them the way you want and search for more, edit:

bUseVSync=0 
FullscreenMode=1
bUseDynamicResolution=0
FrameRateLimit=0
AudioQualityLevel=3
BloomQuality=3 
LensFlareQuality=0
AmbientOcclusion=1
AmbientOcclusionStaticFraction=0
AmbientOcclusionLevels=2
AmbientOcclusionRadiusScale=0.000000
AutoExposure=0
EyeAdaptationQuality=0
OverrideOptions=(("r.somerandomcommand", (Value=0,bModified=True)),("r.someotherrandomcommand", (Value=0,bModified=True)))

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
%localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/DeviceProfiles.ini


Test yourself, copy/paste:   (don't use these unless you are testing stuff or they actually help you with perf or bugs) 

[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverag)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage)


-----------end-----------


for NVIDIA users:

Low latency mode:  off  (lower than ~85% gpu for lowest input lag)
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
TF anisotropic sample optimization:  On (Off for quality) 
TF Negative LOD bias:  Allow
Texture filtering quality:  High performance (Quality for newer GPU)
Vertical sync:  Off


~~~~~~~~~~~~~~~~~~~~~~~~~
