~~~~~~~~~~~~~~~~~~~~~~~~~


*Updated 6/5/2020
*For UE4 games for reference/customization/optimization/learning
*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini and Copy/Paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 


-----------end-----------


Squad* PS* My config Copy/Paste this:

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
r.SceneColorFormat=3 ;
r.VirtualTexture=1 ;
r.TextureStreaming=1 ;
r.RenderTargetPoolMin=400 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.UseFixedPoolSize=0 ;
r.Streaming.PoolSize=1000 ;
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
r.MaxAnisotropy=8 ;
r.MipMapLODBias=-1 ;
r.LandscapeLODBias=-1 ;
r.SkeletalMeshLODBias=-1 ;
r.ParticleLODBias=-1 ;
r.ShadowQuality=3 ;
r.Shadow.PerObject=1 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=4 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.06 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=0.8 ;
r.Shadow.CachedShadowsCastFromMovablePrimitives=1 ;
r.AllowLandscapeShadows=1 ;
r.DistanceFieldShadowing=1 ;
r.DFFullResolution=0 ;
r.DFShadowQuality=1 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=0 ;
r.NormalMapsForStaticLighting=1 ;
Compat.UseDXT5NormalMaps=0 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.Upscale.Quality=3 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.GenerateMeshDistanceFields=1 ;
r.GenerateLandscapeGIData=0 ;
r.AmbientOcclusion.Compute=0 ;
r.AOSpecularOcclusionMode=1 ;
r.AOApplyToStaticIndirect=0 ;
r.DistanceFieldAO=1 ;
r.AOQuality=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.5 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=1 ;
r.AmbientOcclusionRadiusScale=0 ;
r.AmbientOcclusionSampleSetQuality=-1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.ViewDistanceScale=1 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0 ;
r.HLOD=0 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=5000 ;
r.LightFunctionQuality=1 ;
r.LightMaxDrawDistanceScale=0.8 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=0 ;
r.LightShaftFirstPassDistance=1 ;
r.LightCulling.Quality=1 ;
r.HighQualityLightMaps=1 ;
r.IndirectLightingCache=1 ;
r.TranslucencyVolumeBlur=1 ;
r.TranslucencyLightingVolumeDim=64 ;
r.VolumetricFog=0 ;
grass.DensityScale=0.6 ;
foliage.DensityScale=0.6 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.MaterialQualityLevel=1 ;
r.SupportMaterialLayers=0 ;
r.SubsurfaceScattering=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=1 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.SSS.Filter=1 ;
r.SSS.Checkerboard=1 ;
r.DetailMode=2 ;
r.RefractionQuality=0 ;
r.ParticleLightQuality=1 ;
r.ParticleMinTimeBetweenTicks=8 ;
r.EmitterSpawnRateScale=0.5 ;
r.MinTimeBetweenTicks=8 ;
r.LensFlareQuality=0 ;
r.MotionBlurQuality=0 ;
r.BloomQuality=1 ;
r.Filter.SizeScale=1 ;
r.DepthOfFieldQuality=0 ;
r.SeparateTranslucency=1 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.SceneColorFringeQuality=1 ;
r.SceneColorFringe.Max=0.25 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=1 ;


-----------end-----------


Sandstorm* My config Copy/Paste this: 

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
r.SceneColorFormat=3 ;
r.VirtualTexture=1 ;
r.TextureStreaming=1 ;
r.RenderTargetPoolMin=400 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.UseFixedPoolSize=0 ;
r.Streaming.PoolSize=1000 ;
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
r.MaxAnisotropy=8 ;
r.MipMapLODBias=-1 ;
r.LandscapeLODBias=-1 ;
r.SkeletalMeshLODBias=-1 ;
r.ParticleLODBias=-1 ;
r.ShadowQuality=3 ;
r.Shadow.PerObject=1 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=4 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.06 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=0.8 ;
r.Shadow.CachedShadowsCastFromMovablePrimitives=1 ;
r.AllowLandscapeShadows=1 ;
r.DistanceFieldShadowing=1 ;
r.DFFullResolution=0 ;
r.DFShadowQuality=1 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=1 ;
r.NormalMapsForStaticLighting=1 ;
Compat.UseDXT5NormalMaps=0 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.Upscale.Quality=3 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.GenerateMeshDistanceFields=1 ;
r.GenerateLandscapeGIData=0 ;
r.AmbientOcclusion.Compute=0 ;
r.AOSpecularOcclusionMode=1 ;
r.AOApplyToStaticIndirect=0 ;
r.DistanceFieldAO=1 ;
r.AOQuality=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.5 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=1 ;
r.AmbientOcclusionRadiusScale=0 ;
r.AmbientOcclusionSampleSetQuality=-1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.ViewDistanceScale=1 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=1 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=10000 ;
r.LightFunctionQuality=1 ;
r.LightMaxDrawDistanceScale=0.8 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=0 ;
r.LightShaftFirstPassDistance=1 ;
r.LightCulling.Quality=1 ;
r.HighQualityLightMaps=1 ;
r.IndirectLightingCache=1 ;
r.TranslucencyVolumeBlur=1 ;
r.TranslucencyLightingVolumeDim=64 ;
r.VolumetricFog=0 ;
grass.DensityScale=0.6 ;
foliage.DensityScale=0.6 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.MaterialQualityLevel=1 ;
r.SupportMaterialLayers=0 ;
r.SubsurfaceScattering=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=1 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.SSS.Filter=1 ;
r.SSS.Checkerboard=1 ;
r.DetailMode=2 ;
r.RefractionQuality=0 ;
r.ParticleLightQuality=1 ;
r.ParticleMinTimeBetweenTicks=8 ;
r.EmitterSpawnRateScale=0.5 ;
r.MinTimeBetweenTicks=8 ;
r.LensFlareQuality=0 ;
r.MotionBlurQuality=0 ;
r.BloomQuality=1 ;
r.Filter.SizeScale=1 ;
r.DepthOfFieldQuality=0 ;
r.SeparateTranslucency=1 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.SceneColorFringeQuality=1 ;
r.SceneColorFringe.Max=0.25 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=1 ;


-----------end-----------


Open GameUserSettings.ini:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/GameUserSettings.ini 
Copy/Paste:  %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/GameUserSettings.ini 


Resets when you change in game for squad/ps devs dont do this:

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


Other commands to test:

bAltEnterTogglesFullscreen=1
bF11TogglesFullscreen=0
bUseDynamicResolution=0
bPauseOnLossOfFocus=0
bUseFixedFrameRate=0
bEnableMouseSmoothing=0
bEnableFrameRateSmoothing=0
bSmoothFrameRate=0
bUseVSync=0 
FrameRateLimit=120.000000
AudioQualityLevel=3
LastConfirmedAudioQualityLevel=3


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
