~~~~~~~~~~~~~~~~~~~~~~~~~


*Updated 6/14/2020~
*For UE4 games for reference/customization/optimization/learning
*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini and Copy/Paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 


-----------end-----------


Squad* PS* Sandstorm* other UE4 games* My config Copy/Paste this:

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=40 ;

[SystemSettings]
r.MSAACount=0 ;
r.VSync=0 ;
r.AllowHDR=0 ;
r.FinishCurrentFrame=0 ;
r.OneFrameThreadLag=1 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.GPUCrashDebugging=0 ;
r.CreateShadersOnLoad=1 ;
r.AllowOcclusionQueries=1 ;
r.MinScreenRadiusForLights=0.300000 ;
r.MinScreenRadiusForDepthPrepass=0.300000 ;
r.MinScreenRadiusForCSMDepth=0.300000 ;
r.HZBOcclusion=0 ;
r.DiscardUnusedQuality=1 ;
r.SceneColorFormat=3 ; 4 for SANDSTORM 3/2/1 for PERFORMANCE
r.VirtualTexture=1 ; 0 for PERFORMANCE
r.TextureStreaming=1 ;
r.RenderTargetPoolMin=400 ; 300 for PERFORMANCE
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.UseFixedPoolSize=0 ;
r.Streaming.PoolSize=1000 ; 400 for PERFORMANCE
r.Streaming.UseAllMips=0 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.UsePerTextureBias=1 ;
r.Streaming.AmortizeCPUToGPUCopy=1 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.NumStaticComponentsProcessedPerFrame=50 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.Streaming.DefragDynamicBounds=1 ;
r.Streaming.DropMips=2 ;
r.MaxAnisotropy=8 ; 4 for PERFORMANCE
r.MipMapLODBias=-1 ; 0 for PERFORMANCE
r.LandscapeLODBias=-1 ; 1 for PERFORMANCE
r.SkeletalMeshLODBias=-1 ; 1 for PERFORMANCE
r.SkeletalMeshLODRadiusScale=1 ;
r.StaticMeshLODDistanceScale=0.25 ; 1 for PERFORMANCE
r.ParticleLODBias=0 ; 1 for PERFORMANCE
r.ShadowQuality=3 ;
r.Shadow.PerObject=1 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=4 ; 3 for PERFORMANCE
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ; 1024 for PERFORMANCE
r.Shadow.RadiusThreshold=0.06 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=0.8 ;
r.Shadow.CachedShadowsCastFromMovablePrimitives=0 ;
r.Shadow.CSMDepthBias=25 ; (testing shadow artifacts)
r.Shadow.EnableModulatedSelfShadow=0 ;
r.AllowLandscapeShadows=1 ; 0 for PERFORMANCE
r.DistanceFieldShadowing=1 ; 0 for PERFORMANCE
r.DFFullResolution=0 ;
r.DFShadowQuality=1 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=0 ; 1 for SANDSTORM 0 for PERFORMANCE
r.NormalMapsForStaticLighting=0 ;
Compat.UseDXT5NormalMaps=0 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.Upscale.Quality=3 ; 1 for PERFORMANCE (test values)
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ; 0 for PERFORMANCE (could mess with color test)
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.GenerateMeshDistanceFields=1 ; 0 for PERFORMANCE
r.GenerateLandscapeGIData=0 ;
r.AmbientOcclusion.Compute=0 ;
r.AOSpecularOcclusionMode=1 ;
r.AOApplyToStaticIndirect=1 ;
r.DistanceFieldAO=1 ; 0 for PERFORMANCE
r.AOQuality=1 ; 0 for PERFORMANCE
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.5 ;
r.AmbientOcclusionMaxQuality=100 ; 0 for PERFORMANCE
r.AmbientOcclusionLevels=1 ; 0 for PERFORMANCE
r.AmbientOcclusionRadiusScale=0 ;
r.AmbientOcclusionSampleSetQuality=-1 ;
r.ReflectionEnvironment=1 ; 0 for PERFORMANCE
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.ViewDistanceScale=1 ; 0.8 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0 ; 1 for SANDSTORM 0 for PERFORMANCE
r.HLOD=0 ; 1 for SANDSTORM 0 for PERFORMANCE
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=10000 ;
r.LightFunctionQuality=1 ; 0 for PERFORMANCE (cloud shadows)
r.LightMaxDrawDistanceScale=0.8 ;
r.LightShaftQuality=1 ; 0 for PERFORMANCE
r.LightShaftDownSampleFactor=-1 ;
r.LightShaftFirstPassDistance=0.02 ;
r.LightCulling.Quality=1 ;
r.HighQualityLightMaps=1 ; 0 for PERFORMANCE
r.IndirectLightingCache=1 ;
r.TranslucencyLightingVolume=1 ; 0 for PERFORMANCE
r.TranslucencyVolumeBlur=1 ;
r.TranslucencyLightingVolumeDim=64 ;
r.VolumetricFog=0 ;
grass.DensityScale=0.6 ;
foliage.DensityScale=0.6 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.MaterialQualityLevel=1 ; 0 for PERFORMANCE
r.SupportMaterialLayers=0 ;
r.SubsurfaceScattering=1 ; 0 for PERFORMANCE
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=0 ;
r.SSS.Filter=1 ;
r.SSS.Checkerboard=2 ;
r.DetailMode=2 ; 0 for PERFORMANCE
r.RefractionQuality=1 ; 0 for PERFORMANCE
r.ParticleLightQuality=1 ; 0 for PERFORMANCE
r.ParticleMinTimeBetweenTicks=8 ; 16 for PERFORMANCE
r.EmitterSpawnRateScale=0.5 ; 0.25 for PERFORMANCE
r.MinTimeBetweenTicks=8 ; 16 for PERFORMANCE
r.LensFlareQuality=0 ;
r.MotionBlurQuality=0 ;
r.BloomQuality=1 ; 0 for PERFORMANCE
r.Filter.SizeScale=1 ; 0 for PERFORMANCE
r.DepthOfFieldQuality=0 ;
r.SeparateTranslucency=0 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.SceneColorFringeQuality=1 ; 0 for PERFORMANCE
r.SceneColorFringe.Max=0.25 ; -1 for SANDSTORM
r.EyeAdaptationQuality=2 ; 0 for PERFORMANCE
r.DefaultFeature.AutoExposure.Method=1 ;


-----------end-----------


Open GameUserSettings.ini:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/GameUserSettings.ini 
Copy/Paste:  %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/GameUserSettings.ini 


Resets when you change in game for squad/ps devs dont do this, also check this 
in your games because it will overwrite engine.ini changes:

MSAACompositingSampleCount=1
BloomQuality=1 
LensFlareQuality=2 
AmbientOcclusion=1
AmbientOcclusionStaticFraction=0
AmbientOcclusionLevels=1 
AmbientOcclusionRadiusScale=0.000000 
AutoExposure=1
EyeAdaptationQuality=2
TextureStreaming= ; 0 is on in ps.... 


Set these to what you want:

[ScalabilityGroups]
sg.ResolutionQuality=100.000000
sg.ViewDistanceQuality=0
sg.AntiAliasingQuality=3
sg.ShadowQuality=0
sg.PostProcessQuality=0
sg.TextureQuality=0
sg.EffectsQuality=0
sg.FoliageQuality=0


Other commands to test some devs forget to turn off mouse smoothing in games:

bAltEnterTogglesFullscreen=1
bF11TogglesFullscreen=0
bUseDynamicResolution=0
bPauseOnLossOfFocus=0
bUseFixedFrameRate=0
bEnableMouseSmoothing=0
bEnableFrameRateSmoothing=0
bSmoothFrameRate=0
bUseVSync=0 
FrameRateLimit=145.000000
AudioQualityLevel=3


-----------end-----------


EXTRA* For NVIDIA users in control panel change:

Image sharpening:  :)
Low latency mode:  off and lower than ~85% gpu utilization for lowest input lag
Multi/mixed gpu accel:  Single display performance mode
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
Texture filtering anisotropic sample optimization:  On
Texture filtering quality:  High performance
Vertical sync:  Off


~~~~~~~~~~~~~~~~~~~~~~~~~
