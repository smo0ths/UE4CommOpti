~~~~~~~~~~~~~~~~~~~~~~~~~


*Updated 12/30/2020

*For UE4 games for reference/customization/optimization/learning

*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini and copy/paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 

My config:

[Core.Log]
Global=off;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;

[TextureStreaming]
PoolSizeVRAMPercentage=35;

[SystemSettings]
FX.BatchAsyncBatchSize=9999999;
FX.MaxCPUParticlesPerEmitter=50;
FX.MaxGPUParticlesSpawnedPerFrame=2048;
AudioThread.BatchAsyncBatchSize=9999999;
AudioThread.UseBackgroundThreadPool=1;
AudioThread.EnableBatchProcessing=1;
r.setres=1920x1080wf;
r.GPUCrashDebugging=0;
r.CompileShadersForDevelopment=0;
r.CreateShadersOnLoad=1;
r.DBuffer=0;
r.SelectiveBasePassOutputs=0;
r.EarlyZPass=3;
r.EarlyZPassMovable=1;
r.EarlyZPassOnlyMaterialMasking=1;
r.FinishCurrentFrame=0;
r.OneFrameThreadLag=1;
r.GTSyncType=0;
r.AsyncPipelineCompile=1;
r.DrawRectangleOptimization=1;
r.AlsoUseSphereForFrustumCull=1;
r.DoLazyStaticMeshUpdate=1;
r.DiscardUnusedQuality=0;
r.VertexFoggingForOpaque=0;
r.ForceAllCoresForShaderCompiling=1;
r.AllowCachedUniformExpressions=1;
r.D3D11.Depth24Bit=0;
r.VirtualTexture=0;
r.VirtualTexturedLightmaps=0;
r.ShaderComplexity.CacheShaders=1;
r.SkinCache.CompileShaders=0;
r.SkinCache.SceneMemoryLimitInMB=128;
r.ShaderPipelines=1;
r.Shaders.FastMath=1;
r.MorphTarget.Mode=1;
r.GenerateMeshDistanceFields=1;--------0 for PERFORMANCE
r.GenerateLandscapeGIData=0;
r.AOAsyncBuildQueue=1;
r.DistanceFieldBuild.Compress=0;
r.DistanceFields.ParallelAtlasUpdate=1;
r.DistanceFields.ThrottleCopyToAtlasInBytes=1;
r.DFShadowScatterTileCulling=1;
r.HZBOcclusion=0;----------------------0 could improve frames if GPU bound
r.AllowOcclusionQueries=1;-------------occlusion queries
r.AllowSubPrimitiveQueries=1;
r.MinScreenRadiusForLights=0.2;
r.MinScreenRadiusForDepthPrepass=0.2;
r.MinScreenRadiusForCSMDepth=0.2;
r.MinScreenRadiusForSmallLights=0.2;
r.SceneColorFormat=4;------------------format
r.DefaultBackBufferPixelFormat=0;
r.ScreenPercentage=100;----------------scaling stuff
r.SceneRenderTargetResizeMethod=0;
r.Upscale.Quality=0;
r.ClearSceneMethod=1;
r.GBufferFormat=0;---------------------lightstuff
r.AllowStaticLighting=0;---------------1 for SANDSTORM
r.IndirectLightingCache=0;
r.LightFunctionQuality=1;--------------0 for PERFORMANCE
r.NormalMapsForStaticLighting=0;
r.ClearCoatNormal=0;
Compat.UseDXT5NormalMaps=0;
r.HighQualityLightMaps=1;
r.SupportLowQualityLightmaps=0;
r.SupportStationarySkylight=1;
r.SkyLightingQuality=1;
r.LightPropagationVolume=0;
r.LightCulling.Quality=1;
r.LightMaxDrawDistanceScale=0.5;-------0 for PERFORMANCE
r.MipMapLODBias=0;---------------------lods
r.LandscapeLODBias=0;------------------1 for PERFORMANCE
r.SkeletalMeshLODBias=0;
r.ParticleLODBias=-1;
r.ViewDistanceScale=0.8;---------------view distance
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;
r.SkeletalMeshLODRadiusScale=1;
r.StaticMeshLODDistanceScale=1;
r.TextureStreaming=1;------------------texture streaming
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
r.Streaming.AmortizeCPUToGPUCopy=1;
r.Streaming.MaxNumTexturesToStreamPerFrame=1;
r.Streaming.NumStaticComponentsProcessedPerFrame=50;
r.Streaming.FullyLoadUsedTextures=0;
r.Streaming.DefragDynamicBounds=1;
r.Streaming.ScaleTexturesByGlobalMyBias=1;
r.Streaming.HiddenPrimitiveScale=0;
r.Streaming.HLODStrategy=0;
r.Streaming.UseNewMetrics=1;
r.Streaming.MinMipForSplitRequest=1;
r.Streaming.UseMaterialData=1;
r.ShadowQuality=3;---------------------shadows 0 for no shadows
r.Shadow.CSM.MaxCascades=2;
r.Shadow.CSM.TransitionScale=1;
r.Shadow.MinPreShadowResolution=256;
r.Shadow.MinResolution=256;
r.Shadow.MaxResolution=1024;
r.Shadow.MaxCSMResolution=2048;
r.Shadow.RadiusThreshold=0.03;
r.Shadow.RadiusThresholdRSM=0.03;
r.Shadow.DistanceScale=0.6;
r.Shadow.PreShadowResolutionFactor=0.5;
r.Shadow.ForceSingleSampleShadowingFromStationary=1;
r.Shadow.CacheWholeSceneShadows=1;
r.Shadow.CachedShadowsCastFromMovablePrimitives=0;
r.Shadow.CachePreshadow=1;
r.Shadow.UnbuiltPreviewInGame=0;
r.AllowPointLightCubemapShadows=0;
r.SupportPointLightWholeSceneShadows=0;
r.ParallelShadow=0;
r.ParallelShadowsNonWholeScene=0;
r.ContactShadows=0;
r.CapsuleShadows=0;
r.AllowLandscapeShadows=1;-------------0 for PERFORMANCE
r.DistanceFieldShadowing=1;------------0 for PERFORMANCE 0 for SANDSTORM
r.DFShadowQuality=1;
r.DFTwoSidedMeshDistanceBias=0;
r.DFFullResolution=0;
r.Tonemapper.Quality=2;
r.TonemapperFilm=1;
r.Tonemapper.GrainQuantization=1;
r.Tonemapper.Sharpen=0.7;
r.TemporalAASamples=2;-----------------taa
r.TemporalAACurrentFrameWeight=0.2;
r.TemporalAA.Upsampling=0;
r.TemporalAASharpness=0;
r.TemporalAAFilterSize=0.5;
r.DistanceFieldAO=0;-------------------dfao 0 for PERFORMANCE
r.AOQuality=0;
r.AOComputeShaderNormalCalculation=0;
r.SkySpecularOcclusionStrength=0;
r.AOSpecularOcclusionMode=1;
r.AOApplyToStaticIndirect=0;
r.AOHeightfieldOcclusion=0;
r.AmbientOcclusionLevels=2;------------ssao 0 for no ssao
r.AmbientOcclusionStaticFraction=0;
r.AmbientOcclusionMipLevelFactor=0.4;
r.AmbientOcclusionMaxQuality=75;
r.AmbientOcclusionSampleSetQuality=2;
r.AmbientOcclusion.Compute=0;
r.AmbientOcclusionRadiusScale=0;
r.LightShaftQuality=0;-----------------lightshafts
r.LightShaftDownSampleFactor=0;
r.LightShaftFirstPassDistance=0.1;
r.LightShaftBlurPasses=2;
r.LightShaftNumSamples=1;
r.LightShaftRenderToSeparateTranslucency=0;
r.TranslucencyLightingVolume=1;--------translucency
r.TranslucencyVolumeBlur=1;
r.TranslucencyLightingVolumeDim=32;
r.EnableAsyncComputeTranslucencyLightingVolumeClear=1;
r.SeparateTranslucency=1;
r.SeparateTranslucencyScreenPercentage=100;
r.SeparateTranslucencyAutoDownsample=1;
r.TranslucentSortPolicy=0;
TranslucentSortAxis=(X=0.000000,Y=-1.000000,Z=0.000000);
r.CustomDepth=3;
r.CustomDepth.Order=1;
r.SupportAtmosphericFog=1;-------------fog
r.VolumetricFog=0;
r.VolumetricFog.GridPixelSize=16;
r.VolumetricFog.GridSizeZ=64;
r.VolumetricFog.InjectShadowedLightsSeparately=0;
r.ReflectionEnvironment=1;-------------reflection environment 0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1;
r.chaos.ReflectionCaptureStaticSceneOnly=1;
r.DoTiledReflections=1;----------------tiled reflection
r.NoTiledReflections=0;
r.ReflectionCaptureGPUArrayCopy=1;
r.ReflectionCaptureResolution=128;
r.SSR.Quality=0;-----------------------ssr 0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;
r.SSR.MaxRoughness=0.8;
r.SubsurfaceScattering=0;--------------sss 0 for PERFORMANCE
r.SSS.Scale=1;
r.SSS.SampleSet=0;
r.SSS.Quality=-1;
r.SSS.HalfRes=1;
r.SSS.Filter=0;
r.SSS.Checkerboard=2;
r.ParticleLightQuality=1;--------------particles 0 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=8;-------16 for around 60 fps
r.EmitterSpawnRateScale=1;-------------0.25 for PERFORMANCE
r.Emitter.FastPoolEnable=1;
r.TiledDeferredShading=1;--------------tiled deferred shading
r.TiledDeferredShading.MinimumCount=10;
r.DefaultFeature.AutoExposure=1;-------eye adaptation
r.EyeAdaptationQuality=0;
r.DefaultFeature.AutoExposure.Method=0;
r.VSync=0;-----------------------------misc
r.AllowHDR=0;
r.RenderTargetPoolMin=400;
r.TessellationAdaptivePixelsPerTriangle=9999999;
r.MaxAnisotropy=16;
r.SupportMaterialLayers=0;
r.MaterialQualityLevel=1;--------------0 for PERFORMANCE
r.DetailMode=2;------------------------0 for PERFORMANCE
r.RefractionQuality=1;-----------------0 for PERFORMANCE
r.IrisNormal=0;
r.BloomQuality=3;
r.Bloom.HalfResoluionFFT=1;
r.LensFlareQuality=0;
r.Filter.SizeScale=1;
r.Filter.NewMethod=1;
r.MotionBlurQuality=0;
r.DOF.Algorithm=1;
r.DepthOfFieldQuality=0;
r.SceneColorFringeQuality=0;
r.SceneColorFringe.Max=0;
r.StencilForLODDither=0;
grass.DensityScale=0.6;
grass.DisableDynamicShadows=1;
foliage.DensityScale=0.6;
foliage.DitheredLOD=1;


-----------end-----------


Open Input.ini

%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/Insurgency/Saved/Config/WindowsClient/Input.ini


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


settings in here are in game options, they will overwrite your engine.ini commands if they manipulate the same command, change them before starting game to get disired setting: 

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
AmbientOcclusionRadiusScale=0.000000;--------i set this to 0 it will reset to default when toggled in game
AutoExposure=
EyeAdaptationQuality=
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


Textures or you can just use in game settings (sg.TextureQuality=) copy/paste:

[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverag,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_SimpleAverage,NumStreamedMips=3)


-----------end-----------


for NVIDIA users:

Reset settings "apply let the 3D app decide" then set "use the advanced 3D image settings" then apply, click take me there
Low latency mode:  off  (lower than ~85% gpu for lowest input lag)
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
TF anisotropic sample optimization:  On (Off for quality) 
TF Negative LOD bias:  Allow
Texture filtering quality:  High performance (Quality for newer GPU)
Vertical sync:  Off


~~~~~~~~~~~~~~~~~~~~~~~~~
