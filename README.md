~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*Updated 7/3/2019
*For Squad/Insurgency Sandstorm/PS or other UE4 games for reference customization and optimization 
*Always testing stuff contact me twitch.tv/smoothschannel or discord for help or whatever
*PoolSizeVRAMPercentage=50 is how i can lower vram usage for streaming/recording default is 70 i believe, remove or modify if you have low texture problems. 50% uses around 7gb of vram out of my 8gbs in full server combat in squad.

Open Engine.ini and Copy/Paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 


; end ;


SQUAD* Max FPS Copy/Paste this:

when i get around to it


; end ;


SQUAD* My config Copy/Paste this:


[Audio]
MaxChannels=96 ;

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=50 ;

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
FX.AllowGPUSorting=0 ;
t.OverrideFPS=0 ;
t.MaxFPS=200 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.VSync=0 ;
r.OneFrameThreadLag=1 ;
r.HZBOcclusion=0 ;
r.RHICmdBypass=0 ;
r.FinishCurrentFrame=0 ;
r.CompileShadersForDevelopment=0 ;
r.CreateShadersOnLoad=1 ;
r.VirtualTexture=0 ;
r.GPUCrashDebugging=0 ;
r.bForceCPUAccessToGPUSkinVerts=1 ;
r.GBufferFormat=1 ;
r.SceneColorFormat=3 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=1 ;
ShowFlag.Tessellation=0 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.SeparateTranslucency=1 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.SeparateTranslucencyAutoDownsample=1 ;
r.TemporalAASamples=2 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.Upsampling=0 ;
r.AmbientOcclusionMipLevelFactor=0.4 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=0 ;
r.AmbientOcclusionRadiusScale=1 ;
r.AmbientOcclusion.FadeRadiusScale=1 ;
r.AmbientOcclusionStaticFraction=0 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.DistanceFieldAO=0 ;
r.DistanceFieldBuild.Compress=1 ;
r.ViewDistanceScale=0.8 ;
r.StaticMeshLODDistanceScale=0.6 ;
r.SkeletalMeshLODRadiusScale=0.6 ;
r.SkeletalMeshLODBias=0 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.AllowStaticLighting=0 ;
r.NormalMapsForStaticLighting=0 ;
r.ClearCoatNormal=0 ;
r.SupportStationarySkylight=1 ;
r.SkyLightingQuality=1 ;
r.SupportLowQualityLightmaps=0 ;
r.HighQualityLightMaps=1 ;
r.LightMaxDrawDistanceScale=0.8 ;
r.LightFunctionQuality=2 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=0 ;
r.Shadow.MaxResolution=256 ;
r.Shadow.MaxCSMResolution=1024 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=1 ;
r.Shadow.PreShadowResolutionFactor=0.5 ;
r.Shadow.CachePreshadow=1 ;
r.Shadow.CacheWholeSceneShadows=1 ;
r.ParallelShadows=1 ;
r.ParallelShadowsNonWholeScene=1 ;
r.DefaultFeature.LightUnits=1 ;
r.SupportPointLightWholeSceneShadows=0 ;
r.AllowPointLightCubemapShadows=0 ;
r.AllowLandscapeShadows=0 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.CapsuleDirectShadows=0 ;
r.CapsuleShadowsFullResolution=0 ;
r.DistanceFieldShadowing=1 ;
r.DFShadowQuality=1 ;
r.DFFullResolution=0 ;
r.DistanceFieldGI=0 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.VolumetricFog.InjectShadowedLightsSeparately=0 ;
r.MotionBlurQuality=0 ;
r.BlurGBuffer=0 ;
r.FastBlurThreshold=7 ;
r.DepthOfFieldQuality=0 ;
r.LensFlareQuality=0 ;
r.SceneColorFringeQuality=0 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0 ;
r.BloomQuality=0 ;
r.Upscale.Quality=0 ;
r.LightShaftQuality=0 ;
r.LightShaftDownSampleFactor=1 ;
r.LightShaftRenderToSeparateTranslucency=1 ;
r.Filter.SizeScale=1 ;
r.DefaultBackBufferPixelFormat=4 ;
r.Tonemapper.GrainQuantization=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.Sharpen=0.25 ;
r.Tonemapper.MergeWithUpscale.Mode=1 ;
r.RenderTargetPoolMin=400 ;
Compat.UseDXT5NormalMaps=0 ;
r.MaxAnisotropy=8 ;
r.TextureStreaming=1 ;
r.Streaming.DefragDynamicBounds=1 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=1 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=1 ;
r.Streaming.Boost=1 ;
r.Streaming.UsePerTextureBias=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.UseFixedPoolSize=1 ;
r.Streaming.LimitPoolSizeToVRAM=0 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.Streaming.NumStaticComponentsProcessedPerFrame=25 ;
r.Streaming.UseBackgroundThreadPool=1 ;
r.Streaming.UseNewMetrics=1 ;
r.HLOD=1 ;
r.HLOD.DistanceScale=0.6 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyLightingVolumeDim=24 ;
r.TranslucencyVolumeBlur=1 ;
r.DisableDistortion=0 ;
r.RefractionQuality=2 ;
r.DoTiledReflections=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.DetailMode=2 ;
r.MaterialQualityLevel=1 ;
r.SubsurfaceScattering=0 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.SSR.Temporal=1 ;
r.SSR.Stencil=0 ;
r.SSS.Checkerboard=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=0 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.GPUParticle.Simulate=1 ;
r.EmitterSpawnRateScale=0.25 ;
r.ParticleLODBias=0 ;
r.ParticleLightQuality=1 ;
r.AllowSimpleLights=1 ;
foliage.DensityScale=0.6 ;
grass.DensityScale=0.6 ;
grass.DisableDynamicShadows=1 ;
ShowFlag.Vignette=0 ;


; end ;


INSURGENCY SANDSTORM* Max FPS Copy/Paste this:

when i get around to it


; end ;


INSURGENCY SANDSTORM* My config Copy/Paste this: 

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=50 ;

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
FX.AllowGPUSorting=0 ;
t.OverrideFPS=0 ;
t.MaxFPS=200 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.VSync=0 ;
r.OneFrameThreadLag=1 ;
r.HZBOcclusion=0 ;
r.RHICmdBypass=0 ;
r.FinishCurrentFrame=0 ;
r.CompileShadersForDevelopment=0 ;
r.CreateShadersOnLoad=1 ;
r.VirtualTexture=0 ;
r.GPUCrashDebugging=0 ;
r.bForceCPUAccessToGPUSkinVerts=1 ;
r.GBufferFormat=1 ;
r.SceneColorFormat=3 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=1 ;
ShowFlag.Tessellation=0 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.SeparateTranslucency=1 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.SeparateTranslucencyAutoDownsample=1 ;
r.TemporalAASamples=2 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.Upsampling=0 ;
r.AmbientOcclusionMipLevelFactor=0.4 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=0 ;
r.AmbientOcclusionRadiusScale=1 ;
r.AmbientOcclusion.FadeRadiusScale=1 ;
r.AmbientOcclusionStaticFraction=0 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.DistanceFieldAO=0 ;
r.DistanceFieldBuild.Compress=0 ;
r.ViewDistanceScale=0.8 ;
r.StaticMeshLODDistanceScale=0.6 ;
r.SkeletalMeshLODRadiusScale=0.6 ;
r.SkeletalMeshLODBias=0 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.AllowStaticLighting=1 ;
r.NormalMapsForStaticLighting=0 ;
r.ClearCoatNormal=0 ;
r.SupportStationarySkylight=1 ;
r.SkyLightingQuality=1 ;
r.SupportLowQualityLightmaps=0 ;
r.HighQualityLightMaps=1 ;
r.LightMaxDrawDistanceScale=0.8 ;
r.LightFunctionQuality=2 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=0 ;
r.Shadow.MaxResolution=256 ;
r.Shadow.MaxCSMResolution=1024 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=1 ;
r.Shadow.PreShadowResolutionFactor=0.5 ;
r.Shadow.CachePreshadow=1 ;
r.Shadow.CacheWholeSceneShadows=1 ;
r.ParallelShadows=1 ;
r.ParallelShadowsNonWholeScene=1 ;
r.DefaultFeature.LightUnits=1 ;
r.SupportPointLightWholeSceneShadows=0 ;
r.AllowPointLightCubemapShadows=0 ;
r.AllowLandscapeShadows=0 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.CapsuleDirectShadows=0 ;
r.CapsuleShadowsFullResolution=0 ;
r.DistanceFieldShadowing=1 ;
r.DFShadowQuality=1 ;
r.DFFullResolution=0 ;
r.DistanceFieldGI=0 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.VolumetricFog.InjectShadowedLightsSeparately=0 ;
r.MotionBlurQuality=0 ;
r.BlurGBuffer=0 ;
r.FastBlurThreshold=7 ;
r.DepthOfFieldQuality=0 ;
r.LensFlareQuality=0 ;
r.SceneColorFringeQuality=0 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0 ;
r.BloomQuality=0 ;
r.Upscale.Quality=0 ;
r.LightShaftQuality=0 ;
r.LightShaftDownSampleFactor=1 ;
r.LightShaftRenderToSeparateTranslucency=1 ;
r.Filter.SizeScale=1 ;
r.DefaultBackBufferPixelFormat=4 ;
r.Tonemapper.GrainQuantization=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.Sharpen=0.25 ;
r.Tonemapper.MergeWithUpscale.Mode=1 ;
r.RenderTargetPoolMin=400 ;
Compat.UseDXT5NormalMaps=0 ;
r.MaxAnisotropy=8 ;
r.TextureStreaming=1 ;
r.Streaming.DefragDynamicBounds=1 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=1 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=1 ;
r.Streaming.Boost=1 ;
r.Streaming.UsePerTextureBias=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.UseFixedPoolSize=1 ;
r.Streaming.LimitPoolSizeToVRAM=0 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.Streaming.NumStaticComponentsProcessedPerFrame=25 ;
r.Streaming.UseBackgroundThreadPool=1 ;
r.Streaming.UseNewMetrics=1 ;
r.HLOD=1 ;
r.HLOD.DistanceScale=0.8 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyLightingVolumeDim=24 ;
r.TranslucencyVolumeBlur=1 ;
r.DisableDistortion=0 ;
r.RefractionQuality=2 ;
r.DoTiledReflections=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.DetailMode=2 ;
r.MaterialQualityLevel=1 ;
r.SubsurfaceScattering=0 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.SSR.Temporal=1 ;
r.SSR.Stencil=0 ;
r.SSS.Checkerboard=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=0 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.GPUParticle.Simulate=1 ;
r.EmitterSpawnRateScale=0.25 ;
r.ParticleLODBias=0 ;
r.ParticleLightQuality=1 ;
r.AllowSimpleLights=1 ;
foliage.DensityScale=1 ;
grass.DensityScale=1 ;
grass.DisableDynamicShadows=1 ;
ShowFlag.Vignette=0 ;


; end ;


Open: %localappdata%/SquadGame/Saved/Config/WindowsClient/GameUserSettings.ini

Make sure these are set to 0

[ScalabilityGroups]
sg.ViewDistanceQuality=0
sg.ShadowQuality=0
sg.PostProcessQuality=0
sg.TextureQuality=0
sg.EffectsQuality=0
sg.FoliageQuality=0

Also this command is in GameUserSettings.ini set to 0.5 for little bit better SSAO, if you change settings in game it resets.

AmbientOcclusionRadiusScale=0.500000 


; end ;


EXTRA* For NVIDIA users in control panel change:

Maximum pre-rendered frames:  1 (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel:  Single display performance mode
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
Texture filtering anisotropic sample optimization:  On
Texture filtering quality:  High performance
Vertical sync:  Off


; end ;

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
