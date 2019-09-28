~~~~~~~~~~~~~~~~~~~~~~~~~

**Updated 9/28/2019
*For UE4 games for reference/customization/optimization/learning
*Always testing stuff contact me twitch.tv/smoothschannel or discord


-----------end-----------


Open Engine.ini and Copy/Paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 
Copy/Paste:  %localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Engine.ini 


-----------end-----------


Squad* Max fps Copy/Paste this: 

WIP ;


-----------end-----------


Squad* My config Copy/Paste this:

[Audio]
MaxChannels=96 ;

[TextureStreaming]
PoolSizeVRAMPercentage=30 ;

[SystemSettings]
r.HZBOcclusion=0 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.VSync=0 ;
r.AllowHDR=0 ;
r.FinishCurrentFrame=0 ;
r.OneFrameThreadLag=1 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.GPUCrashDebugging=0 ;
r.CreateShadersOnLoad=1 ;
r.GenerateMeshDistanceFields=1 ;
r.GenerateLandscapeGIData=0 ;
r.SceneColorFormat=3 ;
r.CompileShadersForDevelopment=0 ;
Compat.UseDXT5NormalMaps=0 ;
r.MaxAnisotropy=16 ;
r.VirtualTexture=0 ;
r.RenderTargetPoolMin=400 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.TextureStreaming=1 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.SkeletalMeshLODBias=0 ;
r.ParticleLODBias=0 ;
r.Streaming.LimitPoolSizeToVRAM=0 ;
r.Streaming.UseFixedPoolSize=1 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.UsePerTextureBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=0 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.ShadowQuality=3 ;
r.Shadow.PerObject=0 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=3 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=1 ;
r.AllowLandscapeShadows=0 ;
r.DistanceFieldShadowing=1 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=0 ;
r.IndirectLightingCache=1 ;
r.PostProcessAAQuality=3 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=2 ;
r.Upscale.Quality=0 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=0 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ;
r.Tonemapper.Sharpen=0.8 ;
r.DefaultFeature.AmbientOcclusion=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.5 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=1 ;
r.AmbientOcclusionRadiusScale=0.8 ;
r.AmbientOcclusion.FadeRadiusScale=1 ;
r.AmbientOcclusion.Compute=0 ;
r.AmbientOcclusion.AsyncComputeBudget=4 ;
r.AOSpecularOcclusionMode=0 ;
r.AOApplyToStaticIndirect=0 ;
r.DistanceFieldAO=1 ;
r.AOQuality=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.DepthOfFieldQuality=0 ;
r.DepthOfField.FarBlur=0 ;
r.DepthOfField.MaxSize=0 ;
r.ViewDistanceScale=1 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=1 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=10000 ;
r.LightFunctionQuality=1 ;
r.LightMaxDrawDistanceScale=1 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=0 ;
r.LightShaftRenderToSeparateTranslucency=1 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0 ;
r.SSR.Quality=0 ;
r.VolumetricFog=0 ;
r.MotionBlurQuality=0 ;
r.SubsurfaceScattering=1 ;
r.MaterialQualityLevel=1 ;
r.EyeAdaptation.MethodOveride=1 ;
grass.DensityScale=1 ;
foliage.DensityScale=1 ;


-----------end-----------


Sandstorm* Max FPS Copy/Paste this:

WIP ;


-----------end-----------


Sandstorm* My config Copy/Paste this: 

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=30 ;

[SystemSettings]
r.HZBOcclusion=0 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.VSync=0 ;
r.AllowHDR=0 ;
r.FinishCurrentFrame=0 ;
r.OneFrameThreadLag=1 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.GPUCrashDebugging=0 ;
r.CreateShadersOnLoad=1 ;
r.GenerateMeshDistanceFields=1 ;
r.GenerateLandscapeGIData=0 ;
r.SceneColorFormat=3 ;
r.CompileShadersForDevelopment=0 ;
Compat.UseDXT5NormalMaps=0 ;
r.MaxAnisotropy=16 ;
r.VirtualTexture=0 ;
r.RenderTargetPoolMin=400 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.TextureStreaming=1 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.SkeletalMeshLODBias=0 ;
r.ParticleLODBias=0 ;
r.Streaming.LimitPoolSizeToVRAM=0 ;
r.Streaming.UseFixedPoolSize=1 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.UsePerTextureBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=0 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.ShadowQuality=3 ;
r.Shadow.PerObject=0 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=3 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=1 ;
r.AllowLandscapeShadows=0 ;
r.DistanceFieldShadowing=0 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=1 ;
r.IndirectLightingCache=1 ;
r.PostProcessAAQuality=3 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=2 ;
r.Upscale.Quality=0 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=0 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ;
r.Tonemapper.Sharpen=0.8 ;
r.DefaultFeature.AmbientOcclusion=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.5 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=1 ;
r.AmbientOcclusionRadiusScale=0.8 ;
r.AmbientOcclusion.FadeRadiusScale=1 ;
r.AmbientOcclusion.Compute=0 ;
r.AmbientOcclusion.AsyncComputeBudget=4 ;
r.AOSpecularOcclusionMode=0 ;
r.AOApplyToStaticIndirect=0 ;
r.DistanceFieldAO=1 ;
r.AOQuality=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.DepthOfFieldQuality=0 ;
r.DepthOfField.FarBlur=0 ;
r.DepthOfField.MaxSize=0 ;
r.ViewDistanceScale=1 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=1 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=10000 ;
r.LightFunctionQuality=1 ;
r.LightMaxDrawDistanceScale=1 ;
r.LightShaftQuality=0 ;
r.LightShaftDownSampleFactor=0 ;
r.LightShaftRenderToSeparateTranslucency=1 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0 ;
r.SSR.Quality=0 ;
r.VolumetricFog=0 ;
r.MotionBlurQuality=0 ;
r.SubsurfaceScattering=1 ;
r.MaterialQualityLevel=1 ;
r.EyeAdaptation.MethodOveride=1 ;
grass.DensityScale=1 ;
foliage.DensityScale=1 ;


-----------end-----------


Session* My config Copy/Paste this: 

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=30 ;

[SystemSettings]
r.HZBOcclusion=0 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.VSync=0 ;
r.AllowHDR=0 ;
r.FinishCurrentFrame=0 ;
r.OneFrameThreadLag=1 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.RHICmdBypass=0 ;
r.GPUCrashDebugging=0 ;
r.CreateShadersOnLoad=1 ;
r.GenerateMeshDistanceFields=1 ;
r.GenerateLandscapeGIData=0 ;
r.SceneColorFormat=3 ;
r.CompileShadersForDevelopment=0 ;
Compat.UseDXT5NormalMaps=0 ;
r.MaxAnisotropy=16 ;
r.VirtualTexture=0 ;
r.RenderTargetPoolMin=400 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.TextureStreaming=1 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.SkeletalMeshLODBias=0 ;
r.ParticleLODBias=0 ;
r.Streaming.LimitPoolSizeToVRAM=0 ;
r.Streaming.UseFixedPoolSize=1 ;
r.Streaming.PoolSize=1000 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.Streaming.UsePerTextureBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=0 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.ShadowQuality=3 ;
r.Shadow.PerObject=0 ;
r.Shadow.FilterMethod=0 ;
r.Shadow.CSM.MaxCascades=3 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=1 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.6 ;
r.Shadow.CSM.TransitionScale=1 ;
r.AllowLandscapeShadows=0 ;
r.DistanceFieldShadowing=0 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.AllowStaticLighting=0 ;
r.IndirectLightingCache=1 ;
r.PostProcessAAQuality=3 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=2 ;
r.Upscale.Quality=0 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.2 ;
r.TemporalAA.AllowDownsampling=0 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=0 ;
r.Tonemapper.Quality=5 ;
r.Tonemapper.MergeWithUpscale.Mode=0 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ;
r.tonemapper.sharpen=0.8 ;
r.DefaultFeature.AmbientOcclusion=1 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AmbientOcclusionMipLevelFactor=0.5 ;
r.AmbientOcclusionMaxQuality=100 ;
r.AmbientOcclusionLevels=1 ;
r.AmbientOcclusionRadiusScale=0.8 ;
r.AmbientOcclusion.FadeRadiusScale=1 ;
r.AmbientOcclusion.Compute=0 ;
r.AmbientOcclusion.AsyncComputeBudget=4 ;
r.AOSpecularOcclusionMode=0 ;
r.AOApplyToStaticIndirect=0 ;
r.DistanceFieldAO=1 ;
r.AOQuality=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.ReflectionEnvironmentLightmapMixing=1 ;
r.DepthOfFieldQuality=0 ;
r.DepthOfField.FarBlur=0 ;
r.DepthOfField.MaxSize=0 ;
r.ViewDistanceScale=1 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=10000 ;
r.LightFunctionQuality=1 ;
r.LightMaxDrawDistanceScale=1 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=0 ;
r.LightShaftRenderToSeparateTranslucency=1 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0 ;
r.SSR.Quality=0 ;
r.VolumetricFog=0 ;
r.MotionBlurQuality=0 ;
r.SubsurfaceScattering=1 ;
r.MaterialQualityLevel=1 ;
r.EyeAdaptation.MethodOveride=1 ;
grass.DensityScale=1 ;
foliage.DensityScale=1 ;


-----------end-----------


Open GameUserSettings.ini:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/GameUserSettings.ini 
Copy/Paste:  %localappdata%/SessionGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini 


Set these to what you want:

[ScalabilityGroups]
sg.ViewDistanceQuality=0
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
FrameRateLimit=145.000000
FrameLimit=145


In sandstorm r.Streaming.PoolSize needs to be changed here:

("r.Streaming.PoolSize", (Value=1000,bModified=True)


-----------end-----------


EXTRA* For NVIDIA users in control panel change:

Maximum pre-rendered frames:  Off* with lower gpu usage and stable/locked 100-150 fps actually has lower input lag.
Multi/mixed gpu accel:  Single display performance mode
Power management mode:  Prefer max performance
Preferred refresh rate:  Highest available
Texture filtering anisotropic sample optimization:  On
Texture filtering quality:  High performance
Vertical sync:  Off


~~~~~~~~~~~~~~~~~~~~~~~~~
