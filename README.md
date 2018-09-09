*Updated 9/9/2018 ~
*Insurgency Sandstorm configs added
*Post Scriptum and Squad configs 
*Always testing stuff contact me twitch.tv/smoothschannel or discord

\\\\\\\\\\\\\\\\\\\\\\\

Open Engine.ini and Copy/Paste commands/configs:

Press:    Windows key + R      

Copy/Paste:    %localappdata%/Squad/Saved/Config/WindowsNoEditor/Engine.ini 

Copy/Paste:    %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 

Copy/Paste:    %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 


\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\


Max FPS (for Insurgency Sandstorm)


Copy/Paste:  

[Core.Log]
Global=all off

[SystemSettings]
r.PostProcessAAQuality=0
r.SkeletalMeshLODBias=2
r.ViewDistanceScale=0.4
r.LightFunctionQuality=0
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=2
r.Shadow.MaxResolution=1024
r.Shadow.MaxCSMResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.6
r.Shadow.CSM.TransitionScale=1.0
r.Shadow.PreShadowResolutionFactor=0.5
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.VolumetricFog.GridPixelSize=16
r.VolumetricFog.GridSizeZ=64
r.VolumetricFog.HistoryMissSupersampleCount=4
r.LightMaxDrawDistanceScale=0
r.CapsuleShadows=1
r.MotionBlurQuality=0
r.AmbientOcclusionMipLevelFactor=0.5
r.AmbientOcclusionMaxQuality=100
r.AmbientOcclusionLevels=0
r.AmbientOcclusionRadiusScale=1.0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=300 ;
r.LensFlareQuality=0
r.SceneColorFringeQuality=0
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=7
r.Upscale.Quality=0
r.Tonemapper.GrainQuantization=0
r.LightShaftQuality=0
r.Filter.SizeScale=1
r.Tonemapper.Quality=0
r.Streaming.MipBias=2
r.MaxAnisotropy=0
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.PoolSize=400
r.Streaming.MaxEffectiveScreenSize=0
r.TranslucencyLightingVolumeDim=8
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=3 ;
r.DetailMode=0
r.TranslucencyVolumeBlur=0
r.MaterialQualityLevel=0
r.SSS.Scale=1
r.SSS.SampleSet=0
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=0.1
r.ParticleLightQuality=0
foliage.DensityScale=0
grass.DensityScale=0
r.FoliageInteractionQuality=0
r.HLOD.DistanceScale=0.6
r.RenderTargetViewportSize=1.0
r.TessellationAdaptivePixelsPerTriangle=9999999
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
bSmoothFrameRate=0
bUseFixedFrameRate=0
t.MaxFPS=200
r.ScreenPercentage=100
r.FullScreenMode=0
r.VSync=0
r.AllowStaticLighting=1 ;
r.AllowLandscapeShadows=0
r.GBufferFormat=0
r.CustomDepth=0 ;
r.CustomDepth.Order=0
r.TranslucentLightingVolume=1 ;
r.ParticleMinTimeBetweenTicks=16
r.MinTimeBetweenTicks=16
r.SubsurfaceScattering=0
r.CompileShadersForDevelopment=0
r.RHICmdBypass=0
r.SeparateTranslucency=0
r.TiledDeferredShading=0
r.DoTiledReflections=0
r.ReflectionEnvironment=0
r.LandscapeLODBias=0 ;
r.ParticleLODBias=0 ;
r.MipMapLODBias=0
ShowFlag.Decals=0 ; test


\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\


My High/FPS config paste this:  (for Insurgency Sandstorm)


[Core.Log]
Global=all off

[SystemSettings]
r.PostProcessAAQuality=1 ; 1/2=FXAA 3/4/5/6=TAA
r.SkeletalMeshLODBias=0
r.ViewDistanceScale=0.4
r.LightFunctionQuality=1
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=2
r.Shadow.MaxResolution=1024
r.Shadow.MaxCSMResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.6
r.Shadow.CSM.TransitionScale=1.0
r.Shadow.PreShadowResolutionFactor=1.0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.VolumetricFog.GridPixelSize=16
r.VolumetricFog.GridSizeZ=64
r.VolumetricFog.HistoryMissSupersampleCount=4
r.LightMaxDrawDistanceScale=0.5
r.CapsuleShadows=1
r.MotionBlurQuality=0
r.AmbientOcclusionMipLevelFactor=0.5
r.AmbientOcclusionMaxQuality=100
r.AmbientOcclusionLevels=0
r.AmbientOcclusionRadiusScale=1.0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=400
r.LensFlareQuality=2
r.SceneColorFringeQuality=0
r.EyeAdaptationQuality=2 ; test
r.BloomQuality=0
r.FastBlurThreshold=7
r.Upscale.Quality=3
r.Tonemapper.GrainQuantization=1
r.LightShaftQuality=0
r.Filter.SizeScale=1
r.Tonemapper.Quality=5
r.Streaming.MipBias=2
r.MaxAnisotropy=8
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=3000 ; test
r.Streaming.MaxEffectiveScreenSize=0
r.TranslucencyLightingVolumeDim=16
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=3
r.DetailMode=1
r.TranslucencyVolumeBlur=0
r.MaterialQualityLevel=1
r.SSS.Scale=1
r.SSS.SampleSet=2
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=0.1
r.ParticleLightQuality=1
foliage.DensityScale=0 ;
grass.DensityScale=0 ;
r.FoliageInteractionQuality=0
r.HLOD.DistanceScale=1.0
r.RenderTargetViewportSize=1.0
r.TessellationAdaptivePixelsPerTriangle=9999999
r.Shadow.ForceSingleSampleShadowingFromStationary=0 ; test
bSmoothFrameRate=0
bUseFixedFrameRate=0
t.MaxFPS=200
r.ScreenPercentage=100
r.FullScreenMode=0
r.VSync=0
r.AllowStaticLighting=1 ;
r.AllowLandscapeShadows=0
r.HZBOcclusion=0 ;
r.GBufferFormat=1 ;
r.CustomDepth=3
r.CustomDepth.Order=0 ; test
r.OneFrameThreadLag=1
r.TranslucentLightingVolume=1 ;
r.ParticleMinTimeBetweenTicks=16
r.MinTimeBetweenTicks=16
r.SubsurfaceScattering=1 ;
r.CompileShadersForDevelopment=0
r.RHICmdBypass=0
r.SeparateTranslucency=1
r.TiledDeferredShading=1 ;
r.DoTiledReflections=1 ;
r.ReflectionEnvironment=1 ;
r.LandscapeLODBias=0 ;
r.ParticleLODBias=0 ;
r.MipMapLODBias=0
r.AmbientOcclusionStaticFraction=0 ;
ShowFlag.Vignette=0
ShowFlag.Grain=0 ;
r.ToneMapperFilm=1


\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\


Max FPS paste this:  (for Squad and Post Scriptum)


[Core.Log]
Global=all off
LogEasyAntiCheatServer=all off

[Audio]
MaxChannels=64

[SystemSettings]
t.MaxFPS=400
bSmoothFrameRate=0
bUseFixedFrameRate=0
r.EarlyZPass=0
r.EarlyZPassMovable=0
r.EarlyZPassOnlyMaterialMasking=0
r.HZBOcclusion=0
r.CustomDepth=3
r.CustomDepth.Order=0
Compat.UseDXT5NormalMaps=0
r.CompileShadersForDevelopment=0
r.SeparateTranslucency=0
r.DoTiledReflections=0
r.ReflectionEnvironment=0
r.ReflectionCaptureResolution=0
r.TiledDeferredShading=0
r.TranslucencyVolumeBlur=0
r.TranslucentLightingVolume=0
r.TranslucencyLightingVolumeDim=8
r.EmitterSpawnRateScale=0
r.ParticleMinTimeBetweenTicks=16
r.ParticleLightQuality=0
r.MinTimeBetweenTicks=16
r.ViewDistanceScale=0.8
r.StaticMeshLODDistanceScale=0.25
r.SkeletalMeshLODBias=1
r.MipMapLODBias=0
r.MaxAnisotropy=0
r.Streaming.MipBias=2
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=1000
r.Streaming.MaxEffectiveScreenSize=0
r.LightFunctionQuality=0
r.AllowStaticLighting=0
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=1
r.Shadow.MaxResolution=512
r.Shadow.MaxCSMResolution=512
r.Shadow.RadiusThreshold=0.06
r.Shadow.DistanceScale=0.6
r.Shadow.CSM.TransitionScale=0
r.DistanceFieldShadowing=0
r.AllowLandscapeShadows=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.LightMaxDrawDistanceScale=0
r.RenderTargetPoolMin=200
r.Tonemapper.Quality=2
r.Tonemapper.GrainQuantization=0
r.Filter.SizeScale=0
r.MotionBlurQuality=0
r.DepthOfFieldQuality=0
r.LensFlareQuality=0
r.SceneColorFringeQuality=0
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=0
r.Upscale.Quality=0
r.LightShaftQuality=0
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=2
r.DetailMode=0
r.MaterialQualityLevel=0
r.SubsurfaceScattering=0
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=10


\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\


My High/FPS config paste this:  (for Squad and Post Scriptum)


[Core.Log]
Global=all off
LogEasyAntiCheatServer=all off

[Audio]
MaxChannels=96

[SystemSettings]
r.ViewDistanceScale=0.8
r.SkeletalMeshLODBias=0
r.MipMapLODBias=0
r.Streaming.MipBias=2
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=3000
r.Streaming.MaxEffectiveScreenSize=0
r.MaxAnisotropy=16
r.RenderTargetPoolMin=1000
r.DefaultFeature.AmbientOcclusionStaticFraction=0
r.DistanceFieldAO=0
r.LightFunctionQuality=1
r.AllowStaticLighting=0
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=2
r.Shadow.MaxResolution=1024
r.Shadow.MaxCSMResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.4
r.Shadow.CSM.TransitionScale=1.0
r.Shadow.PreShadowResolutionFactor=1.0
r.DistanceFieldShadowing=0
r.AllowLandscapeShadows=0
r.LightMaxDrawDistanceScale=0
r.VolumetricFog=0
r.TranslucencyLightingVolumeDim=16
r.TranslucencyVolumeBlur=0
r.Upscale.Quality=0
r.MotionBlurQuality=0
r.DepthOfFieldQuality=0
r.LensFlareQuality=0
r.SceneColorFormat=3
r.SceneColorFringeQuality=1
r.SceneColorFringe.Max=0.4
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=0
r.Tonemapper.Quality=2
r.Tonemapper.GrainQuantization=0
r.LightShaftQuality=0
r.Filter.SizeScale=0
r.RefractionQuality=0
r.SSR.Quality=0
r.DetailMode=0
r.MaterialQualityLevel=1
r.ParticleLightQuality=1
r.EmitterSpawnRateScale=0.1
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=10
bSmoothFrameRate=0
bUseFixedFrameRate=0
r.FullScreenMode=0
r.VSync=0
r.GBufferFormat=0
r.CustomDepth=3
r.CustomDepth.Order=0
r.OneFrameThreadLag=1 ; test
r.TranslucentLightingVolume=1
r.ParticleMinTimeBetweenTicks=16
r.MinTimeBetweenTicks=16
r.SubsurfaceScattering=0
r.ParticleLODBias=0 ; test
r.CompileShadersForDevelopment=0
r.RHICmdBypass=0
r.SeparateTranslucency=1
r.EarlyZPass=0
r.EarlyZPassMovable=0
r.EarlyZPassOnlyMaterialMasking=0
r.HZBOcclusion=0


\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\


Extra:


For NVIDIA users in control panel change:

Maximum pre-rendered frames: 1  (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel: Single display performance mode
Power management mode: Prefer max performance
Preferred refresh rate: Highest available
Texture filtering anisotropic sample optimization: On
Texture filtering quality: High performance
Vertical sync: Off

\\\\\\\\\\\\\\\\\\\\\\\

Disable Insurgency Sandstorm intro vids add .bak after .mp4 e.g. (UE_Startup_Still_1080_30.mp4.bak)

Press:    Windows key + R    

Copy/Paste:    %SystemDrive%/Program Files (x86)/Steam/steamapps/common/sandstorm/Insurgency/Content/Movies
