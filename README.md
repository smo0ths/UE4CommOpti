~~~~~~~~~~~~~~~~~~~~~~~~~

*Updated 2/6/2020
*For UE4 games for reference/customization/optimization/learning
*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini and Copy/Paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 
Copy/Paste:  %localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 


-----------end-----------


Squad* Max fps Copy/Paste this: 

WIP ;


-----------end-----------


Squad* PS* My config Copy/Paste this:

[Audio]
MaxChannels=128 ;
CommonAudioPoolSize=0 ;
UseAudioThread=True ;
UnfocusedVolumeMultiplier=1.000000

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=50 ; use 40 for PS

[SystemSettings]
r.VSync=0 ;
r.AllowHDR=0 ;
r.FinishCurrentFrame=0 ;
r.OneFrameThreadLag=1 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.GPUCrashDebugging=0 ;
r.CreateShadersOnLoad=1 ;
Compat.UseDXT5NormalMaps=0 ;
r.SceneColorFormat=4 ;
r.SubsurfaceScattering=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.SSS.Filter=1 ;
r.SSS.Checkerboard=0 ;
r.MaxAnisotropy=8 ;
r.VirtualTexture=1 ;
r.RenderTargetPoolMin=300 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.SkeletalMeshLODBias=0 ;
r.ParticleLODBias=0 ;
r.TextureStreaming=1 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.UseFixedPoolSize=0 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.UsePerTextureBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=1 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=1 ;
r.Streaming.NumStaticComponentsProcessedPerFrame=50 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.Streaming.DefragDynamicBounds=1 ;
r.ShadowQuality=3 ;
r.Shadow.PerObject=1 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=4 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=0 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=1024 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.5 ;
r.Shadow.CSM.TransitionScale=0.8 ;
r.AllowLandscapeShadows=1 ;
r.DistanceFieldShadowing=1 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=0 ;
r.IndirectLightingCache=1 ;
r.PostProcessAAQuality=3 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.Upscale.Quality=2 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=0 ;
r.Filter.SizeScale=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=1 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=0 ;
r.GenerateMeshDistanceFields=1 ;
r.DistanceFieldGI=0 ;
r.GenerateLandscapeGIData=1 ;
r.DefaultFeature.AmbientOcclusion=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.4 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=-1 ;
r.AmbientOcclusionRadiusScale=1 ;
r.AmbientOcclusion.FadeRadiusScale=1 ;
r.AmbientOcclusion.Compute=0 ;
r.AOSpecularOcclusionMode=0 ;
r.AOApplyToStaticIndirect=0 ;
r.DistanceFieldAO=0 ;
r.AOQuality=0 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.DepthOfFieldQuality=0 ;
r.ViewDistanceScale=0.8 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0 ;
r.HLOD=0 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=5000 ;
r.SupportSimpleForwardShading=0 ;
r.SimpleForwardShading=0 ;
r.LightFunctionQuality=1 ;
r.LightMaxDrawDistanceScale=0.8 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=0 ;
r.LightShaftFirstPassDistance=0.06 ;
r.BloomQuality=3 ;
r.Bloom.HalfResoluionFFT=0 ;
r.Bloom.Cross=-0.6666 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0 ;
r.SSR.Quality=0 ;
r.VolumetricFog=0 ;
r.MotionBlurQuality=0 ;
r.MaterialQualityLevel=1 ;
r.SupportMaterialLayers=0 ;
r.RefractionQuality=0 ;
r.DetailMode=2 ;
r.ParticleLightQuality=1 ;
r.Atmosphere=1 ;
grass.DensityScale=0.6 ;
foliage.DensityScale=0.6 ;
r.TranslucencyVolumeBlur=1 ;
r.TranslucencyLightingVolumeDim=64 ;
r.TranslucencyLightingVolumeInnerDistance=1500 ;
r.TranslucencyLightingVolumeOuterDistance=5000 ;
r.EmitterSpawnRateScale=0.5 ;
r.MinTimeBetweenTicks=8 ;
r.ParticleMinTimeBetweenTicks=8 ;
r.SeparateTranslucency=0 ;
r.MinScreenRadiusForLights=0.300000 ;
r.MinScreenRadiusForDepthPrepass=0.300000 ;
r.MinScreenRadiusForCSMDepth=0.300000 ;
r.DefaultFeature.AutoExposure=1 ;
r.EyeAdaptationQuality=2 ;


-----------end-----------


Sandstorm* Max FPS Copy/Paste this:

WIP ;


-----------end-----------


Sandstorm* My config Copy/Paste this: 

[Audio]
MaxChannels=128 ;
CommonAudioPoolSize=0 ;
UseAudioThread=True ;
UnfocusedVolumeMultiplier=1.000000

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=40 ;

[SystemSettings]
r.VSync=0 ;
r.AllowHDR=0 ;
r.FinishCurrentFrame=0 ;
r.OneFrameThreadLag=1 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.GPUCrashDebugging=0 ;
r.CreateShadersOnLoad=1 ;
Compat.UseDXT5NormalMaps=0 ;
r.SceneColorFormat=4 ;
r.SubsurfaceScattering=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.SSS.Filter=1 ;
r.SSS.Checkerboard=0 ;
r.MaxAnisotropy=8 ;
r.VirtualTexture=1 ;
r.RenderTargetPoolMin=300 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.SkeletalMeshLODBias=0 ;
r.ParticleLODBias=0 ;
r.TextureStreaming=1 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.UseFixedPoolSize=0 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.UsePerTextureBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=1 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=1 ;
r.Streaming.NumStaticComponentsProcessedPerFrame=50 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.Streaming.DefragDynamicBounds=1 ;
r.ShadowQuality=3 ;
r.Shadow.PerObject=1 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=4 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=0 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=1024 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.5 ;
r.Shadow.CSM.TransitionScale=0.8 ;
r.AllowLandscapeShadows=1 ;
r.DistanceFieldShadowing=1 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=1 ;
r.IndirectLightingCache=1 ;
r.PostProcessAAQuality=4 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.Upscale.Quality=2 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=0 ;
r.Filter.SizeScale=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=1 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=0 ;
r.GenerateMeshDistanceFields=1 ;
r.DistanceFieldGI=0 ;
r.GenerateLandscapeGIData=1 ;
r.DefaultFeature.AmbientOcclusion=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.4 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=-1 ;
r.AmbientOcclusionRadiusScale=1 ;
r.AmbientOcclusion.FadeRadiusScale=1 ;
r.AmbientOcclusion.Compute=0 ;
r.AOSpecularOcclusionMode=1 ;
r.AOApplyToStaticIndirect=0 ;
r.DistanceFieldAO=0 ;
r.AOQuality=0 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.DepthOfFieldQuality=0 ;
r.ViewDistanceScale=0.8 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=1 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=10000 ;
r.SupportSimpleForwardShading=0 ;
r.SimpleForwardShading=0 ;
r.LightFunctionQuality=1 ;
r.LightMaxDrawDistanceScale=0.8 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=0 ;
r.LightShaftFirstPassDistance=0.06 ;
r.BloomQuality=3 ;
r.Bloom.HalfResoluionFFT=0 ;
r.Bloom.Cross=-0.6666 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0 ;
r.SSR.Quality=0 ;
r.VolumetricFog=0 ;
r.MotionBlurQuality=0 ;
r.MaterialQualityLevel=1 ;
r.SupportMaterialLayers=0 ;
r.RefractionQuality=0 ;
r.DetailMode=2 ;
r.ParticleLightQuality=1 ;
r.Atmosphere=1 ;
grass.DensityScale=1 ;
foliage.DensityScale=1 ;
r.TranslucencyVolumeBlur=1 ;
r.TranslucencyLightingVolumeDim=64 ;
r.TranslucencyLightingVolumeInnerDistance=1500 ;
r.TranslucencyLightingVolumeOuterDistance=5000 ;
r.EmitterSpawnRateScale=0.5 ;
r.MinTimeBetweenTicks=8 ;
r.ParticleMinTimeBetweenTicks=8 ;
r.SeparateTranslucency=0 ;
r.MinScreenRadiusForLights=0.300000 ;
r.MinScreenRadiusForDepthPrepass=0.300000 ;
r.MinScreenRadiusForCSMDepth=0.300000 ;
r.DefaultFeature.AutoExposure=1 ;
r.EyeAdaptationQuality=2 ;


-----------end-----------


Session* My config Copy/Paste this: 

WIP ;


-----------end-----------


Open GameUserSettings.ini:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/GameUserSettings.ini 
Copy/Paste:  %localappdata%/SessionGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini 
Copy/Paste:  %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/GameUserSettings.ini 


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


Other options to add under the [~GameUserSettings] part:

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
FrameLimit=120
AudioQualityLevel=3
LastConfirmedAudioQualityLevel=3

In sandstorm r.Streaming.PoolSize needs to be changed here:

("r.Streaming.PoolSize", (Value=1000,bModified=True)


-----------end-----------


EXTRA* For NVIDIA users in control panel change:

Image sharpening:  sharpen ~0.65 ignore film grain ~0.10
Low latency mode:  off and lower than ~85% gpu utilization 
Multi/mixed gpu accel:  Single display performance mode
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
Texture filtering anisotropic sample optimization:  On
Texture filtering quality:  High performance
Vertical sync:  Off
Desktop tab: Enable developer settings: Click Allow access to the GPU performance counters to all users test this yourself 

~~~~~~~~~~~~~~~~~~~~~~~~~
