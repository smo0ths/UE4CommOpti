# SquadOpti

Updated 3/30

Always testing stuff contact me twitch.tv/smoothschannel or discord

\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////
\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////

Open Engine.ini and copy paste configs under code:

     Press:       Windows key + R       
Copy/Paste:       %localappdata%/Squad/Saved/Config/WindowsNoEditor/Engine.ini 

Max FPS: 

[Core.Log]
Global=off

[Audio]
MaxChannels=64

[/Script/Engine.RendererSettings]
r.SkeletalMeshLODBias=1
r.ViewDistanceScale=0.8 ; Lowest hardcoded
r.MipMapLODBias=0
r.LightFunctionQuality=0
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=1
r.Shadow.MaxResolution=512
r.Shadow.MaxCSMResolution=512
r.Shadow.RadiusThreshold=0.06
r.Shadow.DistanceScale=0.6
r.Shadow.CSM.TransitionScale=0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.VolumetricFog.GridPixelSize=0
r.VolumetricFog.GridSizeZ=0
r.AllowLandscapeShadows=0
r.LightMaxDrawDistanceScale=0
r.MotionBlurQuality=0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=300
r.LensFlareQuality=0
r.SceneColorFringeQuality=0
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=0
r.Upscale.Quality=0
r.Tonemapper.GrainQuantization=0
r.LightShaftQuality=0
r.Filter.SizeScale=1
r.Tonemapper.Quality=2
r.Streaming.MipBias=2
r.MaxAnisotropy=0
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=1000
r.Streaming.MaxEffectiveScreenSize=0
r.TranslucencyLightingVolumeDim=8
r.TranslucencyLightingVolumeInnerDistance=8
r.TranslucencyLightingVolumeOuterDistance=8
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=2 ; When using TXAA types you might see ghosting even with 4
r.DetailMode=0
r.TranslucencyVolumeBlur=0
r.MaterialQualityLevel=0
r.SSS.Scale=0
r.SSS.SampleSet=0
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=0
r.ParticleMinTimeBetweenTicks=16
r.ParticleLightQuality=0
foliage.DensityScale=0.6 ; Lowest hardcoded
grass.DensityScale=0.6 ; Lowest hardcoded
grass.MaxUpdateFrequency=10
t.MaxFPS=400
r.ReflectionEnvironment=0 ; When using TXAA types 0 causes black flickering 
r.TiledDeferredShading=0
r.TiledDeferredShading.MinimumCount=0
r.TiledReflectionEnvironmentMinimumCount=0
r.StaticMeshLODDistanceScale=0.25
r.VirtualTexture=0
r.EarlyZPass=0
r.HZBOcclusion=0
r.TranslucentLightingVolume=0
r.NoTiledReflections=1

\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////
\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////

My config: 

[SystemSettings]
r.TranslucentLightingVolume=0

[Core.Log]
Global=all off

[/Script/Engine.RendererSettings]
r.LightFunctionQuality=1
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=1
r.Shadow.MaxResolution=512
r.Shadow.MaxCSMResolution=512
r.Shadow.RadiusThreshold=0.06
r.Shadow.DistanceScale=0.6
r.Shadow.CSM.TransitionScale=0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.VolumetricFog.GridPixelSize=0
r.VolumetricFog.GridSizeZ=0
r.AllowLandscapeShadows=0
r.LightMaxDrawDistanceScale=0
r.SkeletalMeshLODBias=0
r.ViewDistanceScale=0.8
r.MipMapLODBias=0
r.MotionBlurQuality=0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=1000
r.LensFlareQuality=0
r.SceneColorFringeQuality=0
r.SceneColorFringe.Max=0.5
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=0
r.Upscale.Quality=0
r.LightShaftQuality=1
r.LightShaftDownSampleFactor=0
r.Filter.SizeScale=1
r.Tonemapper.Quality=5
r.Tonemapper.GrainQuantization=0
r.Streaming.MipBias=0
r.MaxAnisotropy=0
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=4000
r.Streaming.MaxEffectiveScreenSize=0
r.TranslucencyLightingVolumeDim=64
r.TranslucencyVolumeBlur=0
r.TranslucencyLightingVolumeInnerDistance=1500
r.TranslucencyLightingVolumeOuterDistance=5000
r.SceneColorFormat=4
r.RefractionQuality=0
r.SSR.Quality=0
r.DetailMode=2
r.MaterialQualityLevel=1
r.SSS.Scale=0
r.SSS.SampleSet=0
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=1.0
r.MinTimeBetweenTicks=16
r.ParticleMinTimeBetweenTicks=16
r.ParticleLightQuality=2
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=10
r.Color.Max=1.0	   ; > move more colors towards white, < darken the highlights               Default: 1
r.Color.Mid=0.5    ; > darken the mid tones,           < brighten the mid tones              Default: 0.5
r.Color.Min=0      ; > more dark values become black,  < a gray scale is added to the darks  Default: 0
t.MaxFPS=400
r.OneFrameThreadLag=1 ; 0 lower fps for less input lag
r.VSync=0
r.EarlyZPass=0
r.EarlyZPassMovable=0
r.HZBOcclusion=0
r.HalfResReflections=1
r.OptimizeForUAVPerformance=1
r.CompileShadersForDevelopment=0
r.Atmosphere=0
r.TiledDeferredShading=1
r.TiledDeferredShading.MinimumCount=10
r.ReflectionEnvironment=1
r.DoTiledReflections=1
r.VirtualTexture=0
FX.AllowGPUSorting=1

\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////
\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////

For NVIDIA users in control panel change:

Maximum pre-rendered frames: 1  (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel: Single display performance mode
Power management mode: Prefer max performance
Preferred refresh rate: Highest available
Texture filtering anisotropic sample optimization: On
Texture filtering quality: High performance
Vertical sync: Off

\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////
\\\\\\\\\\\\\\\\\\\\\\\
///////////////////////

Max/Ultra raw settings for reference: 

;ViewDistanceQuality

r.SkeletalMeshLODBias=-1
r.ViewDistanceScale=10.0
r.MipMapLODBias=-1     

;ShadowQuality

r.LightFunctionQuality=1
r.ShadowQuality=5
r.Shadow.CSM.MaxCascades=10
r.Shadow.MaxResolution=4096
r.Shadow.MaxCSMResolution=4096
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=1.0
r.Shadow.CSM.TransitionScale=1.0
r.DistanceFieldShadowing=1
r.DistanceFieldAO=1
r.VolumetricFog=1
r.VolumetricFog.GridPixelSize=4
r.VolumetricFog.GridSizeZ=128
r.AllowLandscapeShadows=1        

;PostProcessQuality

r.MotionBlurQuality=4
r.AmbientOcclusionMipLevelFactor=0.4
r.AmbientOcclusionMaxQuality=100
r.AmbientOcclusionLevels=-1
r.AmbientOcclusionRadiusScale=1.0
r.DepthOfFieldQuality=4
r.RenderTargetPoolMin=1000
r.LensFlareQuality=3
r.SceneColorFringeQuality=1
r.EyeAdaptationQuality=2
r.BloomQuality=5
r.FastBlurThreshold=100
r.Upscale.Quality=3
r.Tonemapper.GrainQuantization=1
r.LightShaftQuality=1
r.Filter.SizeScale=1
r.Tonemapper.Quality=5

;TextureQuality

r.Streaming.MipBias=0
r.MaxAnisotropy=16        
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=3000
r.Streaming.MaxEffectiveScreenSize=0

;EffectsQuality

r.TranslucencyLightingVolumeDim=64
r.RefractionQuality=2
r.SSR.Quality=4
r.SceneColorFormat=4
r.DetailMode=2
r.TranslucencyVolumeBlur=1
r.MaterialQualityLevel=1      
r.SSS.Scale=1
r.SSS.SampleSet=2
r.SSS.Quality=1
r.SSS.HalfRes=0
r.EmitterSpawnRateScale=1.0
r.ParticleLightQuality=2
r.MinTimeBetweenTicks=8
r.ParticleMinTimeBetweenTicks=16        

;FoliageQuality

foliage.DensityScale=1.0
grass.DensityScale=1.0
grass.MaxUpdateFrequency=30       

;Extra
t.MaxFPS=400
