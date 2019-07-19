~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*Updated 7/19/2019
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
r.GBufferFormat=3 ;
r.SceneColorFormat=4 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
ShowFlag.Tessellation=0 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
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
r.ViewDistanceScale=1 ;
r.StaticMeshLODDistanceScale=1 ;
r.SkeletalMeshLODRadiusScale=1 ;
r.SkeletalMeshLODBias=0 ;
r.MipMapLODBias=-1 ;
r.LandscapeLODBias=0 ;
r.AllowStaticLighting=0 ;
r.SkyLightingQuality=1 ;
r.HighQualityLightMaps=1 ;
r.LightMaxDrawDistanceScale=1 ;
r.LightFunctionQuality=1 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.8 ;
r.Shadow.CSM.TransitionScale=1 ;
r.DefaultFeature.LightUnits=1 ;
r.AllowLandscapeShadows=1 ;
r.ContactShadows=1 ;
r.CapsuleShadows=0 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.VolumetricFog.InjectShadowedLightsSeparately=0 ;
r.MotionBlurQuality=0 ;
r.BlurGBuffer=0 ;
r.FastBlurThreshold=7 ;
r.DepthOfFieldQuality=2 ;
r.LensFlareQuality=2 ;
r.SceneColorFringeQuality=0 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0 ;
r.BloomQuality=3 ;
r.Upscale.Quality=3 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=1 ;
r.Filter.SizeScale=1 ;
r.DefaultBackBufferPixelFormat=4 ;
r.Tonemapper.GrainQuantization=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.Sharpen=0.25 ;
r.RenderTargetPoolMin=400 ;
Compat.UseDXT5NormalMaps=0 ;
r.MaxAnisotropy=8 ;
r.TextureStreaming=1 ;
r.Streaming.HiddenPrimitiveScale=1 ;
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
r.Streaming.NumStaticComponentsProcessedPerFrame=50 ;
r.HLOD=1 ;
r.HLOD.DistanceScale=1 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyLightingVolumeDim=48 ;
r.TranslucencyVolumeBlur=1 ;
r.DisableDistortion=0 ;
r.RefractionQuality=2 ;
r.DoTiledReflections=1 ;
r.chaos.ReflectionCaptureStaticSceneOnly=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionCaptureResolution=128
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.DetailMode=2 ;
r.MaterialQualityLevel=1 ;
r.SubsurfaceScattering=1 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.SSR.Temporal=1 ;
r.SSR.Stencil=0 ;
r.SSS.Checkerboard=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=0 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.EmitterSpawnRateScale=0.25 ;
r.ParticleLODBias=0 ;
r.ParticleLightQuality=1 ;
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
r.GBufferFormat=3 ;
r.SceneColorFormat=4 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
ShowFlag.Tessellation=0 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
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
r.ViewDistanceScale=1 ;
r.StaticMeshLODDistanceScale=1 ;
r.SkeletalMeshLODRadiusScale=1 ;
r.SkeletalMeshLODBias=0 ;
r.MipMapLODBias=-1 ;
r.LandscapeLODBias=0 ;
r.AllowStaticLighting=1 ;
r.SkyLightingQuality=1 ;
r.HighQualityLightMaps=1 ;
r.LightMaxDrawDistanceScale=1 ;
r.LightFunctionQuality=1 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=1024 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.8 ;
r.Shadow.CSM.TransitionScale=1 ;
r.DefaultFeature.LightUnits=1 ;
r.AllowLandscapeShadows=1 ;
r.ContactShadows=1 ;
r.CapsuleShadows=0 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.VolumetricFog.InjectShadowedLightsSeparately=0 ;
r.MotionBlurQuality=0 ;
r.BlurGBuffer=0 ;
r.FastBlurThreshold=7 ;
r.DepthOfFieldQuality=2 ;
r.LensFlareQuality=2 ;
r.SceneColorFringeQuality=0 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0 ;
r.BloomQuality=3 ;
r.Upscale.Quality=3 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=1 ;
r.Filter.SizeScale=1 ;
r.DefaultBackBufferPixelFormat=4 ;
r.Tonemapper.GrainQuantization=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.Sharpen=0.25 ;
r.RenderTargetPoolMin=400 ;
Compat.UseDXT5NormalMaps=0 ;
r.MaxAnisotropy=8 ;
r.TextureStreaming=1 ;
r.Streaming.HiddenPrimitiveScale=1 ;
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
r.Streaming.NumStaticComponentsProcessedPerFrame=50 ;
r.HLOD=1 ;
r.HLOD.DistanceScale=1 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyLightingVolumeDim=48 ;
r.TranslucencyVolumeBlur=1 ;
r.DisableDistortion=0 ;
r.RefractionQuality=2 ;
r.DoTiledReflections=1 ;
r.chaos.ReflectionCaptureStaticSceneOnly=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionCaptureResolution=128
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.DetailMode=2 ;
r.MaterialQualityLevel=1 ;
r.SubsurfaceScattering=1 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.SSR.Temporal=1 ;
r.SSR.Stencil=0 ;
r.SSS.Checkerboard=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=0 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.EmitterSpawnRateScale=0.25 ;
r.ParticleLODBias=0 ;
r.ParticleLightQuality=1 ;
foliage.DensityScale=1 ;
grass.DensityScale=1 ;
grass.DisableDynamicShadows=1 ;
ShowFlag.Vignette=0 ;
r.Dismemberment=1 ;


; end ;


Open: %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini

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
