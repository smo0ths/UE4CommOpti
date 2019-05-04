~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




*Updated 5/4/2019
*For Squad/Insurgency Sandstorm/PS or other UE4 games for reference customization and optimization 
*Always testing stuff contact me twitch.tv/smoothschannel or discord for help or whatever

Open Engine.ini and Copy/Paste commands/configs:

     Press:    Windows key + R      
Copy/Paste:    %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:    %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 
Copy/Paste:    %localappdata%/PostScriptum/Saved/Config/WindowsNoEditor/Engine.ini 




; end ;




SQUAD* Max FPS Copy/Paste this:

[Core.Log]
Global=all off ;

[Audio]
MaxChannels=64 ;

when i get around to it




; end ;




SQUAD/PS* My config Copy/Paste this:




[Audio]
MaxChannels=96 ;
UseAudioThread=false ;

[Core.Log]
Global=all off ;

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
r.FullScreenMode=0 ;
r.VSync=0 ;
t.OverrideFPS=0 ;
t.MaxFPS=250 ;
r.OneFrameThreadLag=1 ;
r.HZBOcclusion=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.FinishCurrentFrame=0 ;
r.ReflectionEnvironment=0 ;
r.DefaultFeature.LightUnits=0 ;
r.TonemapperFilm=1 ;
r.GBufferFormat=1 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.RenderTargetPoolMin=450 ;
r.SkeletalMeshLODRadiusScale=1 ;
r.SkeletalMeshLODBias=0 ;
r.ViewDistanceScale=0.8 ;
r.MipMapLODBias=-1 ;
r.LandscapeLODBias=0 ;
r.CustomDepthTemporalAAJitter=0 ;
r.TemporalAASamples=2 ;
r.TemporalAACurrentFrameWeight=0.3 ;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=1 ;
r.EyeAdaptation.PreExposureOverride=0 ;
r.UsePreExposure=0 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.SceneColorFringe.Max=-0.25 ;
r.AmbientOcclusionMaxQuality=-100 ;
r.AmbientOcclusionMipLevelFactor=0.3 ;
r.AmbientOcclusionMipLevelFactor=0 ;
r.AmbientOcclusionRadiusScale=0.3 ;
r.AmbientOcclusionRadiusScale=0 ;
r.LightFunctionQuality=1 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.01 ;
r.Shadow.DistanceScale=0.5 ;
r.Shadow.CSM.TransitionScale=1.0 ;
r.Shadow.PreShadowResolutionFactor=0 ;
r.AllowLandscapeShadows=1 ;
r.DistanceFieldShadowing=0 ;
r.DistanceFieldAO=0 ;
r.AllowStaticLighting=0 ;
r.AOQuality=0 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=8 ;
r.VolumetricFog.GridSizeZ=128 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.LightMaxDrawDistanceScale=1 ;
r.CapsuleShadows=0 ;
r.CapsuleShadowsCharacter=0 ;
r.ContactShadows=0 ;
r.MotionBlurQuality=0 ;
r.AmbientOcclusionLevels=0 ;
r.DepthOfFieldQuality=1 ;
r.LensFlareQuality=2 ;
r.SceneColorFringeQuality=1 ;
r.EyeAdaptationQuality=2 ;
r.BloomQuality=3 ;
r.FastBlurThreshold=7 ;
r.Upscale.Quality=0 ;
r.Tonemapper.GrainQuantization=1 ;
r.LightShaftQuality=1 ;
r.Filter.SizeScale=1 ;
r.Tonemapper.Quality=5 ;
r.Streaming.MipBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=0 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.Boost=1.0 ;
r.MaxAnisotropy=8 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.TranslucencyLightingVolumeDim=32 ;
r.RefractionQuality=0 ;
r.SSR.Quality=0 ;
r.SceneColorFormat=4 ;
r.DetailMode=0 ;
r.TranslucencyVolumeBlur=1 ;
r.MaterialQualityLevel=1 ;
r.SubsurfaceScattering=0 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=1 ;
r.SSS.HalfRes=0 ;
r.EmitterSpawnRateScale=1.0 ;
r.ParticleLightQuality=1 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.SeparateTranslucencyScreenPercentage=100 ;
foliage.DensityScale=0.6 ;
grass.DensityScale=0.6 ;




; end ;




INSURGENCY SANDSTORM* Max FPS Copy/Paste this:

[Core.Log]
Global=all off ;

when i get around to it




; end ;




INSURGENCY SANDSTORM* My config Copy/Paste this: 

[Core.Log]
Global=all off ;

[SystemSettings]
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
r.FullScreenMode=0 ;
r.VSync=0 ;
t.OverrideFPS=0 ;
t.MaxFPS=250 ;
r.OneFrameThreadLag=1 ;
r.HZBOcclusion=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.ReflectionEnvironment=1 ;
r.DefaultFeature.LightUnits=0 ;
r.TonemapperFilm=1 ;
r.GBufferFormat=1 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.RenderTargetPoolMin=450 ;
r.PostProcessAAQuality=2 ;
r.SkeletalMeshLODRadiusScale=1 ;
r.SkeletalMeshLODBias=0 ;
r.ViewDistanceScale=0.8 ;
r.MipMapLODBias=-1 ;
r.LandscapeLODBias=0 ;
r.TemporalAASamples=2 ;
r.TemporalAACurrentFrameWeight=0.3 ;
r.EyeAdaptation.PreExposureOverride=1 ;
r.UsePreExposure=1 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.LightFunctionQuality=1 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=1024 ;
r.Shadow.RadiusThreshold=0.01 ;
r.Shadow.DistanceScale=0.5 ;
r.Shadow.CSM.TransitionScale=1.0 ;
r.Shadow.PreShadowResolutionFactor=0 ;
r.AllowLandscapeShadows=1 ;
r.DistanceFieldShadowing=0 ;
r.DistanceFieldAO=0 ;
r.AllowStaticLighting=1 ;
r.AOQuality=0 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=8 ;
r.VolumetricFog.GridSizeZ=128 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.LightMaxDrawDistanceScale=1 ;
r.CapsuleShadows=0 ;
r.CapsuleShadowsCharacter=0 ;
r.ContactShadows=0 ;
r.MotionBlurQuality=0 ;
r.AmbientOcclusionMipLevelFactor=0 ;
r.AmbientOcclusionMaxQuality=0 ;
r.AmbientOcclusionLevels=0 ;
r.AmbientOcclusionRadiusScale=0 ;
r.DepthOfFieldQuality=1 ;
r.LensFlareQuality=2 ;
r.SceneColorFringeQuality=1 ;
r.EyeAdaptationQuality=2 ;
r.BloomQuality=3 ;
r.FastBlurThreshold=7 ;
r.Upscale.Quality=0 ;
r.Tonemapper.GrainQuantization=1 ;
r.LightShaftQuality=1 ;
r.Filter.SizeScale=1 ;
r.Tonemapper.Quality=5 ;
r.Streaming.MipBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=0 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.Boost=1.0 ;
r.MaxAnisotropy=8 ;
r.Streaming.LimitPoolSizeToVRAM=1 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.TranslucencyLightingVolumeDim=32 ;
r.RefractionQuality=0 ;
r.SSR.Quality=0 ;
r.SceneColorFormat=4 ;
r.DetailMode=0 ;
r.TranslucencyVolumeBlur=1 ;
r.MaterialQualityLevel=1 ;
r.SubsurfaceScattering=0 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=2 ;
r.SSS.Quality=1 ;
r.SSS.HalfRes=0 ;
r.HLOD.DistanceScale=1.0 ;
r.EmitterSpawnRateScale=1.0 ;
r.RenderTargetViewportSize=1.0 ;
r.ParticleLightQuality=0 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.SurfReac.Particles.PoolSize=60 ;
r.ScopeRenderMode=0 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.RagdollMaximum=4 ;
r.Dismemberment=1 ;
r.FoliageInteractionQuality=0 ;
foliage.DensityScale=0.6 ;
grass.DensityScale=0.6 ;




; end ;




EXTRA* For NVIDIA users in control panel change:

Maximum pre-rendered frames: 1  (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel: Single display performance mode
Power management mode: Prefer max performance
Preferred refresh rate: Highest available
Texture filtering anisotropic sample optimization: On
Texture filtering quality: High performance
Vertical sync: Off




; end ;




Disable INSURGENCY SANDSTORM* intro vids add .bak after .mp4 e.g. (UE_Startup_Still_1080_30.mp4.bak)

     Press:    Windows key + R    
Copy/Paste:    %SystemDrive%/Program Files (x86)/Steam/steamapps/common/sandstorm/Insurgency/Content/Movies




~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
