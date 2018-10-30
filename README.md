*Updated 10/30/2018
*Insurgency Sandstorm configs added
*Post Scriptum and Squad configs
*Customize your UE4 game settings with this if you want 
*Always testing stuff contact me twitch.tv/smoothschannel or discord

Open Engine.ini and Copy/Paste commands/configs:

Press:         Windows key + R      
Copy/Paste:    %localappdata%/Squad/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:    %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:    %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

Max FPS for Insurgency Sandstorm* paste this:

Copy/Paste:  

[Core.Log]
Global=all off

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
t.MaxFPS=300 ;
t.OverrideFPS=0 ;
r.FullScreenMode=0 ;
r.VSync=0 ;
r.HZBOcclusion=1 ;
r.ClearSceneMethod=1 ;
r.OneFrameThreadLag=1 ;
r.FinishCurrentFrame=0 ;
r.RHICmdBypass=0 ;
r.CompileShadersForDevelopment=0 ;
r.CreateShadersOnLoad=1 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.Cache.LimitQuerySize=1 ;
r.BasePassOutputsVelocity=1 ;
r.VirtualTexture=0 ;
r.AlsoUseSphereForFrustumCull=-1 ;
a.ParallelBlendPhysics=0 ;
r.Atmosphere=1 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.DefaultFeature.AntiAliasing=0 ;
r.PostProcessAAQuality=0 ;
r.RenderTargetPoolMin=200 ;
r.SkeletalMeshLODBias=2 ;
r.SkeletalMeshLODRadiusScale=1.0 ;
r.StaticMeshLODDistanceScale=0.25 ;
r.ViewDistanceScale=0.4 ;
r.ForceLOD=-1 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=0.6 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.TextureStreaming=1 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=2 ;
r.Streaming.Boost=1 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.PoolSize=-1 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.MaxAnisotropy=0 ;
r.SkyLightingQuality=0 ;
r.IndirectLightingCache=1 ;
r.LightFunctionQuality=0 ;
r.ShadowQuality=0 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.7 ;
r.Shadow.CSM.TransitionScale=1.0 ;
r.Shadow.PreShadowResolutionFactor=0.5 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.CSMDepthBias=30 ;
r.Shadow.CachePreshadow=1 ;
r.Shadow.CacheWholeSceneShadows=1 ;
r.AllowLandscapeShadows=0 ;
r.CapsuleShadows=0 ;
r.CapsuleShadowsFullResolution=0 ;
r.DistanceFieldShadowing=0 ;
r.AllowStaticLighting=1 ;
r.HighQualityLightMaps=0 ;
r.MultithreadedLightmapEncode=1 ;
r.MultithreadedShadowmapEncode=1 ;
r.DistanceFieldGI=0 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyVolumeBlur=0 ;
r.TranslucencyLightingVolumeDim=16 ;
r.TranslucencyLightingVolumeInnerDistance=1500 ;
r.TranslucencyLightingVolumeOuterDistance=5000 ;
r.LightShaftQuality=0 ;
r.LightShaftDownSampleFactor=4 ;
r.SupportAtmosphericFog=0 ;
r.Fog=1 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.DefaultFeature.AmbientOcclusion=0 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0 ;
r.AmbientOcclusionMaxQuality=0 ;
r.AmbientOcclusionLevels=0 ;
r.AmbientOcclusionRadiusScale=0.1 ; 
r.AmbientOcclusion.FadeRadiusScale=1.0 ;
r.AmbientOcclusion.Compute=0 ;
r.AmbientOcclusion.AsyncComputeBudget=1 ; 
r.GenerateMeshDistanceFields=0 ;
r.DistanceFieldAO=0 ;
r.LightMaxDrawDistanceScale=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.GrainQuantization=1 ;
ShowFlag.Vignette=0 ;
ShowFlag.Grain=0 ;
r.BlurGBuffer=0 ;
r.DefaultFeature.MotionBlur=0 ;
r.MotionBlurQuality=0 ;
r.FastBlurThreshold=7 ;
r.SeparateTranslucency=1 ;
r.DepthOfFieldQuality=0 ;
r.DefaultFeature.LensFlare=0 ;
r.LensFlareQuality=0 ;
r.DefaultFeature.AutoExposure=1 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.Bloom=0 ;
r.BloomQuality=0 ;
r.Filter.SizeScale=1 ;
r.Upscale.Quality=0 ;
r.RefractionQuality=0 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=1 ;
r.SSR.Temporal=0 ;
r.GBufferFormat=0 ;
r.SceneColorFormat=3 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0.5 ;
r.DetailMode=0 ;
r.MaterialQualityLevel=0 ;
r.ClearCoatNormal=0 ;
r.SubsurfaceScattering=0 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.ParticleLightQuality=0 ;
r.ParticleMinTimeBetweenTicks=16 ;
r.MinTimeBetweenTicks=16 ;
r.EmitterSpawnRateScale=0.1 ;
foliage.DensityScale=0 ;
grass.DensityScale=0 ;
grass.MaxUpdateFrequency=10 ;
r.FoliageInteractionQuality=0 ;
r.RenderTargetViewportSize=1.0 ;
r.CustomDepth=0 ;
r.CustomDepth.Order=1 ;
r.DisableDistortion=1 ;
r.ForwardShading=0 ;
r.SupportSimpleForwardShading=0 ;
r.SimpleForwardShading=0 ;
r.TiledDeferredShading=0 ;
r.TiledDeferredShading.MinimumCount=80 ;
r.TiledReflectionEnvironmentMinimumCount=10 ;
r.DoTiledReflections=0 ; 
r.NoTiledReflections=0 ;
r.HalfResReflections=0 ;
r.ReflectionEnvironment=0 ;
r.ReflectionCaptureGPUArrayCopy=1 ;
r.ReflectionCaptureResolution=128 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.DefaultFeature.PointLightUnits=0 ;
r.DefaultFeature.SpotLightUnits=0 ;

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

My config for Insurgency Sandstorm* paste this:

[Core.Log]
Global=all off

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
t.MaxFPS=300 ;
t.OverrideFPS=0 ;
r.FullScreenMode=0 ;
r.VSync=0 ;
r.HZBOcclusion=1 ;
r.ClearSceneMethod=1 ;
r.OneFrameThreadLag=1 ;
r.FinishCurrentFrame=0 ;
r.RHICmdBypass=0 ;
r.CompileShadersForDevelopment=0 ;
r.CreateShadersOnLoad=1 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.Cache.LimitQuerySize=1 ;
r.BasePassOutputsVelocity=1 ;
r.VirtualTexture=0 ;
r.AlsoUseSphereForFrustumCull=-1 ;
a.ParallelBlendPhysics=0 ;
r.Atmosphere=1 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=1 ;
r.DefaultFeature.AntiAliasing=1 ;
r.PostProcessAAQuality=1 ;
r.RenderTargetPoolMin=400 ;
r.SkeletalMeshLODBias=0 ;
r.SkeletalMeshLODRadiusScale=1.0 ;
r.StaticMeshLODDistanceScale=1 ;
r.ViewDistanceScale=0.4 ;
r.ForceLOD=-1 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1.0 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.TextureStreaming=1 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=2 ;
r.Streaming.Boost=1 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.PoolSize=2000 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.MaxAnisotropy=16 ;
r.SkyLightingQuality=1 ;
r.IndirectLightingCache=1 ;
r.LightFunctionQuality=1 ;
r.ShadowQuality=0 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.7 ;
r.Shadow.CSM.TransitionScale=1.0 ;
r.Shadow.PreShadowResolutionFactor=0.5 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.CSMDepthBias=30 ;
r.Shadow.CachePreshadow=1 ;
r.Shadow.CacheWholeSceneShadows=1 ;
r.AllowLandscapeShadows=1 ;
r.CapsuleShadows=0 ;
r.CapsuleShadowsFullResolution=0 ;
r.DistanceFieldShadowing=1 ;
r.AllowStaticLighting=1 ;
r.HighQualityLightMaps=1 ;
r.MultithreadedLightmapEncode=1 ;
r.MultithreadedShadowmapEncode=1 ;
r.DistanceFieldGI=1 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyVolumeBlur=0 ;
r.TranslucencyLightingVolumeDim=32 ;
r.TranslucencyLightingVolumeInnerDistance=1500 ;
r.TranslucencyLightingVolumeOuterDistance=5000 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=0 ;
r.SupportAtmosphericFog=0 ;
r.Fog=1 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.DefaultFeature.AmbientOcclusion=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0 ;
r.AmbientOcclusionMaxQuality=-100 ;
r.AmbientOcclusionLevels=2 ;
r.AmbientOcclusionRadiusScale=0.1 ;
r.AmbientOcclusion.FadeRadiusScale=1.0 ;
r.AmbientOcclusion.Compute=0 ;
r.AmbientOcclusion.AsyncComputeBudget=1 ;
r.GenerateMeshDistanceFields=0 ;
r.DistanceFieldAO=0 ;
r.LightMaxDrawDistanceScale=1.0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.GrainQuantization=1 ;
ShowFlag.Vignette=0 ;
ShowFlag.Grain=0 ;
r.BlurGBuffer=0 ;
r.DefaultFeature.MotionBlur=0 ;
r.MotionBlurQuality=0 ;
r.FastBlurThreshold=7 ;
r.SeparateTranslucency=1 ;
r.DepthOfFieldQuality=0 ;
r.DefaultFeature.LensFlare=1 ;
r.LensFlareQuality=2 ;
r.DefaultFeature.AutoExposure=1 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.Bloom=0 ;
r.BloomQuality=0 ;
r.Filter.SizeScale=1 ;
r.Upscale.Quality=3 ;
r.RefractionQuality=2 ;
r.SSR.Quality=1 ;
r.SSR.MaxRoughness=0.9 ;
r.SSR.Temporal=0 ;
r.GBufferFormat=1 ;
r.SceneColorFormat=3 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0.5 ;
r.DetailMode=2 ;
r.MaterialQualityLevel=1 ;
r.ClearCoatNormal=0 ;
r.SubsurfaceScattering=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.ParticleLightQuality=2 ;
r.ParticleMinTimeBetweenTicks=8 ;
r.MinTimeBetweenTicks=8 ;
r.EmitterSpawnRateScale=1.0 ;
foliage.DensityScale=0 ;
grass.DensityScale=0 ;
grass.MaxUpdateFrequency=10 ;
r.FoliageInteractionQuality=0 ;
r.RenderTargetViewportSize=1.0 ;
r.CustomDepth=0 ;
r.CustomDepth.Order=1 ;
r.DisableDistortion=1 ;
r.ForwardShading=0 ;
r.SupportSimpleForwardShading=0 ;
r.SimpleForwardShading=0 ;
r.TiledDeferredShading=1 ;
r.TiledDeferredShading.MinimumCount=80 ;
r.TiledReflectionEnvironmentMinimumCount=10 ;
r.DoTiledReflections=1 ;
r.NoTiledReflections=0 ;
r.HalfResReflections=0 ;
r.ReflectionEnvironment=1 ;
r.ReflectionCaptureGPUArrayCopy=1 ;
r.ReflectionCaptureResolution=128 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.DefaultFeature.PointLightUnits=0 ;
r.DefaultFeature.SpotLightUnits=0 ;

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

Max FPS for Squad* and Post Scriptum* paste this:

[Core.Log]
Global=all off
LogEasyAntiCheatServer=all off

[Audio]
MaxChannels=64

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
t.MaxFPS=300 ;
t.OverrideFPS=0 ;
r.FullScreenMode=0 ;
r.VSync=0 ;
r.HZBOcclusion=1 ;
r.ClearSceneMethod=1 ;
r.OneFrameThreadLag=1 ;
r.FinishCurrentFrame=0 ;
r.RHICmdBypass=0 ;
r.CompileShadersForDevelopment=0 ;
r.CreateShadersOnLoad=1 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.Cache.LimitQuerySize=1 ;
r.BasePassOutputsVelocity=1 ;
r.VirtualTexture=0 ;
r.AlsoUseSphereForFrustumCull=-1 ;
a.ParallelBlendPhysics=0 ;
r.Atmosphere=1 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.DefaultFeature.AntiAliasing=0 ;
r.PostProcessAAQuality=0 ;
r.RenderTargetPoolMin=200 ;
r.SkeletalMeshLODBias=1 ;
r.SkeletalMeshLODRadiusScale=1.0 ;
r.StaticMeshLODDistanceScale=0.25 ;
r.ViewDistanceScale=0.8 ;
r.ForceLOD=-1 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1.0 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.TextureStreaming=1 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=2 ;
r.Streaming.Boost=1 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.PoolSize=-1 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.MaxAnisotropy=0 ;
r.SkyLightingQuality=0 ;
r.IndirectLightingCache=1 ;
r.LightFunctionQuality=0 ;
r.ShadowQuality=0 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.7 ;
r.Shadow.CSM.TransitionScale=1.0 ;
r.Shadow.PreShadowResolutionFactor=0.5 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.CSMDepthBias=30 ;
r.Shadow.CachePreshadow=1 ;
r.Shadow.CacheWholeSceneShadows=1 ;
r.AllowLandscapeShadows=0 ;
r.CapsuleShadows=0 ;
r.CapsuleShadowsFullResolution=0 ;
r.DistanceFieldShadowing=0 ;
r.AllowStaticLighting=0 ;
r.HighQualityLightMaps=0 ;
r.MultithreadedLightmapEncode=1 ;
r.MultithreadedShadowmapEncode=1 ;
r.DistanceFieldGI=0 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyVolumeBlur=0 ;
r.TranslucencyLightingVolumeDim=16 ;
r.TranslucencyLightingVolumeInnerDistance=1500 ;
r.TranslucencyLightingVolumeOuterDistance=5000 ;
r.LightShaftQuality=0 ;
r.LightShaftDownSampleFactor=4 ;
r.SupportAtmosphericFog=0 ;
r.Fog=1 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.DefaultFeature.AmbientOcclusion=0 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0 ;
r.AmbientOcclusionMaxQuality=0 ;
r.AmbientOcclusionLevels=0 ;
r.AmbientOcclusionRadiusScale=0.1 ;
r.AmbientOcclusion.FadeRadiusScale=1.0 ;
r.AmbientOcclusion.Compute=0 ;
r.AmbientOcclusion.AsyncComputeBudget=1 ;
r.GenerateMeshDistanceFields=0 ;
r.DistanceFieldAO=0 ;
r.LightMaxDrawDistanceScale=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.GrainQuantization=1 ;
ShowFlag.Vignette=0 ;
ShowFlag.Grain=0 ;
r.BlurGBuffer=0 ;
r.DefaultFeature.MotionBlur=0 ;
r.MotionBlurQuality=0 ;
r.FastBlurThreshold=7 ;
r.SeparateTranslucency=1 ;
r.DepthOfFieldQuality=0 ;
r.DefaultFeature.LensFlare=0 ;
r.LensFlareQuality=0 ;
r.DefaultFeature.AutoExposure=1 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.Bloom=0 ;
r.BloomQuality=0 ;
r.Filter.SizeScale=1 ;
r.Upscale.Quality=0 ;
r.RefractionQuality=0 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=1 ;
r.SSR.Temporal=0 ;
r.GBufferFormat=0 ;
r.SceneColorFormat=3 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0.5 ;
r.DetailMode=0 ;
r.MaterialQualityLevel=0 ;
r.ClearCoatNormal=0 ;
r.SubsurfaceScattering=0 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.ParticleLightQuality=0 ;
r.ParticleMinTimeBetweenTicks=16 ;
r.MinTimeBetweenTicks=16 ;
r.EmitterSpawnRateScale=0.1 ;
foliage.DensityScale=0.6 ;
grass.DensityScale=0.6 ;
grass.MaxUpdateFrequency=10 ;
r.FoliageInteractionQuality=0 ;
r.RenderTargetViewportSize=1.0 ;
r.CustomDepth=3 ;
r.CustomDepth.Order=1 ;
r.DisableDistortion=1 ;
r.ForwardShading=0 ;
r.SupportSimpleForwardShading=0 ;
r.SimpleForwardShading=0 ;
r.TiledDeferredShading=0 ;
r.TiledDeferredShading.MinimumCount=80 ;
r.TiledReflectionEnvironmentMinimumCount=10 ;
r.DoTiledReflections=0 ;
r.NoTiledReflections=0 ;
r.HalfResReflections=0 ;
r.ReflectionEnvironment=0 ;
r.ReflectionCaptureGPUArrayCopy=1 ;
r.ReflectionCaptureResolution=128 ;
r.ReflectionEnvironmentBeginMixingRoughness=0.1 ;
r.ReflectionEnvironmentEndMixingRoughness=0.3 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.ReflectionEnvironmentLightmapMixLargestWeight=1000 ;
r.DefaultFeature.PointLightUnits=0 ;
r.DefaultFeature.SpotLightUnits=0 ;

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

My config for Squad* and Post Scriptum* paste this:

[Core.Log]
Global=all off
LogEasyAntiCheatServer=all off

[Audio]
MaxChannels=96 ;

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
r.VSync=0 ;
t.IdleWhenNotForeground=0 ;
t.OverrideFPS=0 ;
t.MaxFPS=300 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.RHICmdBypass=0 ;
r.HZBOcclusion=1 ;
r.OneFrameThreadLag=1 ;
r.FinishCurrentFrame=0 ;
r.CreateShadersOnLoad=1 ;
r.CompileShadersForDevelopment=0 ;
r.RenderTargetPoolMin=400 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.PoolSize=2000 ;
r.MaxAnisotropy=16 ;
r.CustomDepth=3 ;
r.SceneColorFormat=3 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.AlsoUseSphereForFrustumCull=-1 ;
r.GBufferFormat=0 ;
foliage.DensityScale=0.6 ;
grass.DensityScale=0.6 ;
r.ViewDistanceScale=0.8 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=1.0 ;
r.ReflectionEnvironment=0 ;
r.SSR.Quality=0 ;
r.LightShaftQuality=0 ;
r.DepthOfFieldQuality=0 ;
r.Streaming.MipBias=2 ;
r.SceneColorFringe.Max=0.3 ;
r.DistanceFieldAO=0 ;
r.VolumetricFog=0 ;
r.SubsurfaceScattering=0 ;
r.AllowLandscapeShadows=0 ;

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

Edit GameUserSettings.ini:

Bloom=1
BloomQuality=1
LensFlare=1
LensFlareQuality=2
EyeAdaptationQuality=2

sg.ViewDistanceQuality=3
sg.AntiAliasingQuality=3
sg.ShadowQuality=3
sg.PostProcessQuality=3
sg.TextureQuality=3
sg.EffectsQuality=4
sg.FoliageQuality=3

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

Extra:

For NVIDIA users in control panel change:

Maximum pre-rendered frames: 1  (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel: Single display performance mode
Power management mode: Prefer max performance
Preferred refresh rate: Highest available
Texture filtering anisotropic sample optimization: On
Texture filtering quality: High performance
Vertical sync: Off

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

Disable Insurgency Sandstorm intro vids add .bak after .mp4 e.g. (UE_Startup_Still_1080_30.mp4.bak)

Press:         Windows key + R    
Copy/Paste:    %SystemDrive%/Program Files (x86)/Steam/steamapps/common/sandstorm/Insurgency/Content/Movies
