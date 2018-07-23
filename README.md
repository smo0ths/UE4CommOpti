Updated 7/23/2018

*Post Scriptum works with this aswell

Always testing stuff contact me twitch.tv/smoothschannel or discord

r.OneFrameThreadLag=0 ; lowers input delay test yourself default is 1 

Open Engine.ini and copy paste configs under code:

Press: Windows key + R       
Copy/Paste: %localappdata%/Squad/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste: %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 


\\\\\\\\\\\\\\\\\\\\\\\


Max FPS paste this: 

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


My squad and post scriptum high/fps config paste this: 

[Core.Log]
Global=all off
LogEasyAntiCheatServer=all off

[Audio]
MaxChannels=96

[SystemSettings]
t.MaxFPS=400
bSmoothFrameRate=0
bUseFixedFrameRate=0
r.VSync=0
s.AsyncLoadingThreadEnabled=1
Compat.UseDXT5NormalMaps=0
r.OneFrameThreadLag=0
r.GBufferFormat=0
r.CompileShadersForDevelopment=0
r.SeparateTranslucency=0
r.CustomDepth=3
r.CustomDepth.Order=0
r.HZBOcclusion=0
r.EarlyZPass=0
r.EarlyZPassMovable=0
r.EarlyZPassOnlyMaterialMasking=0
r.ViewDistanceScale=0.8
r.SkeletalMeshLODBias=0
r.MipMapLODBias=0
r.TextureStreaming=1
r.Streaming.MipBias=0
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=3000
r.Streaming.MaxEffectiveScreenSize=0
r.MaxAnisotropy=16
r.RenderTargetPoolMin=1000
r.AmbientOcclusionMipLevelFactor=0.5
r.AmbientOcclusionMaxQuality=100
r.AmbientOcclusionLevels=3
r.AmbientOcclusionRadiusScale=0.5
r.AmbientOcclusion.FadeRadiusScale=1.0
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
r.DistanceFieldShadowing=0
r.AllowLandscapeShadows=0
r.LightMaxDrawDistanceScale=0
r.VolumetricFog=0
r.TranslucentLightingVolume=1
r.TranslucencyLightingVolumeDim=8
r.TranslucencyVolumeBlur=0
r.Upscale.Quality=0
r.MotionBlurQuality=0
r.DepthOfFieldQuality=0
r.LensFlareQuality=0
r.SceneColorFormat=3
r.SceneColorFringeQuality=0
r.SceneColorFringe.Max=0.45
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=0
r.Tonemapper.Quality=2
r.Tonemapper.GrainQuantization=1
r.Tonemapper.Sharpen=0
r.LightShaftQuality=1
r.LightShaftDownSampleFactor=4
r.Filter.SizeScale=1
r.RefractionQuality=0
r.SSR.Quality=0
r.SSR.MaxRoughness=0.1
r.DetailMode=2
r.MaterialQualityLevel=1
r.SubsurfaceScattering=0
r.ParticleLightQuality=1
r.ParticleMinTimeBetweenTicks=16
r.EmitterSpawnRateScale=1.0
r.MinTimeBetweenTicks=16
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=10
r.TiledDeferredShading=1
r.TiledDeferredShading.MinimumCount=10
r.DoTiledReflections=1                                 ; test
r.ReflectionCaptureResolution=128
r.ReflectionEnvironment=1
r.ReflectionEnvironmentBeginMixingRoughness=0.1        ; def 0.1
r.ReflectionEnvironmentEndMixingRoughness=0.3          ; def 0.3
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=0   ; def 1
r.ReflectionEnvironmentLightmapMixing=1                ; def idk
r.ReflectionEnvironmentLightmapMixLargestWeight=1000   ; def 1000


\\\\\\\\\\\\\\\\\\\\\\\


For NVIDIA users in control panel change:

Maximum pre-rendered frames: 1  (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel: Single display performance mode
Power management mode: Prefer max performance
Preferred refresh rate: Highest available
Texture filtering anisotropic sample optimization: On
Texture filtering quality: High performance
Vertical sync: Off
