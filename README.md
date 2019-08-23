~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

****Updated 8/23/2019
*For Squad/Insurgency Sandstorm/PS or other UE4 games for reference customization and optimization 
*Always testing stuff contact me twitch.tv/smoothschannel or discord for help or whatever


; end ;


Open Engine.ini and Copy/Paste commands/configs:

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini 
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsClient/Engine.ini 


; end ;


************WIP************ 
SQUAD* Max FPS Copy/Paste this: 


; end ;


SQUAD* My config Copy/Paste this:

[Audio]
MaxChannels=96 ;

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=20 ;

[SystemSettings]
ShowFlag.Vignette=0 ;
ShowFlag.Tessellation=0 ;
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
bUseDynamicResolution=0 ;
t.OverrideFPS=0 ;
t.MaxFPS=200 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.VSync=0 ;
r.OneFrameThreadLag=1 ;
r.CreateShadersOnLoad=1 ;
r.HZBOcclusion=1 ;
r.RHICmdBypass=0 ;
r.FinishCurrentFrame=0 ;
r.AllowHDR=0 ;
r.VirtualTexture=1 ;
r.VirtualTextureReducedMemory=0 ;
r.VirtualTexturedLightmaps=1 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.SceneColorFormat=4 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.GPUCrashDebugging=0 ;
r.GpuSkin.Pool=1 ;
r.D3D11.NVAutoFlushUAV=1 ;
r.RenderTargetPoolMin=400 ;
r.GBufferFormat=1 ;
r.DefaultBackBufferPixelFormat=0 ;
r.MaxAnisotropy=8 ;
r.TextureStreaming=1 ;
Compat.UseDXT5NormalMaps=0 ;
r.Streaming.LimitPoolSizeToVRAM=0 ;
r.Streaming.UseFixedPoolSize=1 ;
r.Streaming.PoolSize=600 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.SkeletalMeshLODBias=-1 ;
r.ParticleLODBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=0 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.UsePerTextureBias=0 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.Streaming.HiddenPrimitiveScale=0 ;
r.Streaming.DefragDynamicBounds=1 ;
r.Streaming.UseNewMetrics=1 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=0 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.7 ;
r.Shadow.CSM.TransitionScale=1 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.15 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=1 ;
r.TemporalAACatmullRom=1 ;
r.TemporalAAPauseCorrect=1 ;
r.AmbientOcclusionMipLevelFactor=0.4 ;
r.AmbientOcclusionMaxQuality=-100 ;
r.AmbientOcclusionLevels=2 ;
r.AmbientOcclusionRadiusScale=0.5 ;
r.AmbientOcclusion.FadeRadiusScale=0.5 ;
r.AmbientOcclusionStaticFraction=0 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AllowStaticLighting=0 ;
r.AllowLandscapeShadows=1 ;
r.LightMaxDrawDistanceScale=1 ;
r.LightFunctionQuality=1 ;
r.LightShaftQuality=1 ;
r.LightShaftDownSampleFactor=1 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ;
r.Tonemapper.Quality=2 ;
r.Tonemapper.Sharpen=0.5 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.VolumetricFog.InjectShadowedLightsSeparately=0 ;
r.ViewDistanceScale=0.8 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=5000 ;
r.Filter.SizeScale=1 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyLightingVolumeDim=64 ;
r.TranslucencyVolumeBlur=1 ;
r.SeparateTranslucency=1 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.SSR.Temporal=1 ;
r.SSR.Stencil=0 ;
r.SubsurfaceScattering=1 ;
r.SSS.Checkerboard=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=1 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.Emitter.FastPoolEnable=1 ;
r.EmitterSpawnRateScale=0.5 ;
r.ParticleLightQuality=1 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0 ;
grass.DensityScale=0.6 ;
grass.DisableDynamicShadows=1 ;
foliage.DensityScale=0.6 ;
r.GenerateMeshDistanceFields=1 ;
r.GenerateLandscapeGIData=0 ;
r.DistanceFieldGI=0 ;
r.DistanceFieldShadowing=1 ;
r.DFFullResolution=1 ;
r.DFShadowQuality=1 ;
r.DFTwoSidedMeshDistanceBias=1 ;
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1 ;
r.SkeletalMeshLODRadiusScale=1 ;
r.StaticMeshLODDistanceScale=1 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.AOQuality=0 ;
r.DistanceFieldAO=0 ;
r.AOApplyToStaticIndirect=0 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.DefaultFeature.LightUnits=1 ;
r.DisableDistortion=0 ;
r.RefractionQuality=2 ;
r.DoTiledReflections=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.DetailMode=1 ;
r.MaterialQualityLevel=1 ;
r.MotionBlurQuality=0 ;
r.BlurGBuffer=0 ;
r.FastBlurThreshold=15 ;
r.DepthOfFieldQuality=0 ;
r.DepthOfField.FarBlur=0 ;
r.LensFlareQuality=2 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0 ;
r.BloomQuality=0 ;
r.Upscale.Quality=0 ;
r.MinTimeBetweenTicks=8 ;
r.ParticleMinTimeBetweenTicks=8 ;
r.Decal.StencilSizeThreshold=0.1 ;
r.Decal.FadeDurationScale=0.5 ;
r.Decal.FadeScreenSizeMult=0.5 ;


; end ;


************WIP************
INSURGENCY SANDSTORM* Max FPS Copy/Paste this:


; end ;


INSURGENCY SANDSTORM* My config Copy/Paste this: 

[Core.Log]
Global=all off ;

[TextureStreaming]
PoolSizeVRAMPercentage=20 ;

[SystemSettings]
ShowFlag.Vignette=0 ;
ShowFlag.Tessellation=0 ;
bSmoothFrameRate=0 ;
bUseFixedFrameRate=0 ;
bEnableMouseSmoothing=0 ;
bDisablePhysXHardwareSupport=0 ;
bPauseOnLossOfFocus=0 ;
bUseDynamicResolution=0 ;
t.OverrideFPS=0 ;
t.MaxFPS=200 ;
r.FullScreenMode=0 ;
r.GTSyncType=0 ;
r.VSync=0 ;
r.OneFrameThreadLag=1 ;
r.CreateShadersOnLoad=1 ;
r.HZBOcclusion=1 ;
r.RHICmdBypass=0 ;
r.FinishCurrentFrame=0 ;
r.AllowHDR=0 ;
r.VirtualTexture=1 ;
r.VirtualTextureReducedMemory=0 ;
r.VirtualTexturedLightmaps=0 ;
r.EarlyZPass=2 ;
r.EarlyZPassMovable=1 ;
r.EarlyZPassOnlyMaterialMasking=1 ;
r.SceneColorFormat=4 ;
r.ScreenPercentage=100 ;
r.SceneRenderTargetResizeMethod=0 ;
r.GPUCrashDebugging=0 ;
r.GpuSkin.Pool=1 ;
r.D3D11.NVAutoFlushUAV=1 ;
r.RenderTargetPoolMin=400 ;
r.GBufferFormat=1 ;
r.DefaultBackBufferPixelFormat=0 ;
r.MaxAnisotropy=8 ;
r.TextureStreaming=1 ;
Compat.UseDXT5NormalMaps=0 ;
r.Streaming.LimitPoolSizeToVRAM=0 ;
r.Streaming.UseFixedPoolSize=1 ;
r.Streaming.PoolSize=600 ;
r.Streaming.HLODStrategy=0 ;
r.Streaming.MipBias=0 ;
r.MipMapLODBias=0 ;
r.LandscapeLODBias=0 ;
r.SkeletalMeshLODBias=-1 ;
r.ParticleLODBias=0 ;
r.Streaming.AmortizeCPUToGPUCopy=0 ;
r.Streaming.MaxNumTexturesToStreamPerFrame=0 ;
r.Streaming.UsePerTextureBias=0 ;
r.Streaming.Boost=1 ;
r.Streaming.FullyLoadUsedTextures=0 ;
r.Streaming.MaxEffectiveScreenSize=0 ;
r.Streaming.HiddenPrimitiveScale=0 ;
r.Streaming.DefragDynamicBounds=1 ;
r.Streaming.UseNewMetrics=1 ;
r.ShadowQuality=3 ;
r.Shadow.CSM.MaxCascades=2 ;
r.Shadow.ForceSingleSampleShadowingFromStationary=0 ;
r.Shadow.MaxResolution=1024 ;
r.Shadow.MaxCSMResolution=2048 ;
r.Shadow.RadiusThreshold=0.03 ;
r.Shadow.DistanceScale=0.7 ;
r.Shadow.CSM.TransitionScale=1 ;
r.TemporalAASamples=4 ;
r.TemporalAACurrentFrameWeight=0.15 ;
r.TemporalAA.Upsampling=0 ;
r.TemporalAAUpsampleFiltered=1 ;
r.TemporalAACatmullRom=1 ;
r.TemporalAAPauseCorrect=1 ;
r.AmbientOcclusionMipLevelFactor=0.4 ;
r.AmbientOcclusionMaxQuality=-100 ;
r.AmbientOcclusionLevels=2 ;
r.AmbientOcclusionRadiusScale=0.5 ;
r.AmbientOcclusion.FadeRadiusScale=0.5 ;
r.AmbientOcclusionStaticFraction=0 ;
r.DefaultFeature.AmbientOcclusionStaticFraction=0 ;
r.AllowStaticLighting=1 ;
r.AllowLandscapeShadows=1 ;
r.LightMaxDrawDistanceScale=1 ;
r.LightFunctionQuality=1 ;
r.LightShaftQuality=0 ;
r.LightShaftDownSampleFactor=1 ;
r.TonemapperFilm=1 ;
r.Tonemapper.GrainQuantization=1 ;
r.Tonemapper.Quality=2 ;
r.Tonemapper.Sharpen=0.5 ;
r.VolumetricFog=0 ;
r.VolumetricFog.GridPixelSize=16 ;
r.VolumetricFog.GridSizeZ=64 ;
r.VolumetricFog.HistoryMissSupersampleCount=4 ;
r.VolumetricFog.InjectShadowedLightsSeparately=0 ;
r.ViewDistanceScale=0.8 ;
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0 ;
r.HLOD=1 ;
r.HLOD.MaximumLevel=-1 ;
r.HLOD.DistanceScale=1 ;
r.HLOD.DistanceOverride=5000 ;
r.Filter.SizeScale=1 ;
r.TranslucentLightingVolume=1 ;
r.TranslucencyLightingVolumeDim=64 ;
r.TranslucencyVolumeBlur=1 ;
r.SeparateTranslucency=1 ;
r.SeparateTranslucencyScreenPercentage=100 ;
r.SSR.Quality=0 ;
r.SSR.MaxRoughness=0.8 ;
r.SSR.Temporal=1 ;
r.SSR.Stencil=0 ;
r.SubsurfaceScattering=1 ;
r.SSS.Checkerboard=1 ;
r.SSS.Scale=1 ;
r.SSS.SampleSet=1 ;
r.SSS.Quality=0 ;
r.SSS.HalfRes=1 ;
r.Emitter.FastPoolEnable=1 ;
r.EmitterSpawnRateScale=0.5 ;
r.ParticleLightQuality=1 ;
r.EyeAdaptationQuality=2 ;
r.DefaultFeature.AutoExposure.Method=0 ;
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=0 ;
grass.DensityScale=1 ;
grass.DisableDynamicShadows=1 ;
foliage.DensityScale=1 ;
r.GenerateMeshDistanceFields=1 ;
r.GenerateLandscapeGIData=0 ;
r.DistanceFieldGI=0 ;
r.DistanceFieldShadowing=1 ;
r.DFFullResolution=1 ;
r.DFShadowQuality=1 ;
r.DFTwoSidedMeshDistanceBias=1 ;
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1 ;
r.SkeletalMeshLODRadiusScale=1 ;
r.StaticMeshLODDistanceScale=1 ;
r.TessellationAdaptivePixelsPerTriangle=9999999 ;
r.AOQuality=0 ;
r.DistanceFieldAO=0 ;
r.AOApplyToStaticIndirect=0 ;
r.ContactShadows=0 ;
r.CapsuleShadows=0 ;
r.DefaultFeature.LightUnits=1 ;
r.DisableDistortion=0 ;
r.RefractionQuality=2 ;
r.DoTiledReflections=1 ;
r.ReflectionEnvironment=1 ;
r.ReflectionEnvironmentLightmapMixBasedOnRoughness=1 ;
r.DetailMode=1 ;
r.MaterialQualityLevel=1 ;
r.MotionBlurQuality=0 ;
r.BlurGBuffer=0 ;
r.FastBlurThreshold=15 ;
r.DepthOfFieldQuality=0 ;
r.DepthOfField.FarBlur=0 ;
r.LensFlareQuality=2 ;
r.SceneColorFringeQuality=0 ;
r.SceneColorFringe.Max=0 ;
r.BloomQuality=0 ;
r.Upscale.Quality=0 ;
r.MinTimeBetweenTicks=8 ;
r.ParticleMinTimeBetweenTicks=8 ;
r.Decal.StencilSizeThreshold=0.1 ;
r.Decal.FadeDurationScale=0.5 ;
r.Decal.FadeScreenSizeMult=0.5 ;
r.SurfReac.Particles.PoolSize=5 ;
r.FoliageInteractionQuality=0 ;
r.CapsuleShadowsCharacter=0 ;
r.Dismemberment=1 ;


; end ;


Open GameUserSettings.ini

Press:       Windows key + R      
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
Copy/Paste:  %localappdata%/Insurgency/Saved/Config/WindowsNoEditor/GameUserSettings.ini 

Make sure these are set to 0

[ScalabilityGroups]
sg.ViewDistanceQuality=0
sg.ShadowQuality=0
sg.PostProcessQuality=0
sg.TextureQuality=0
sg.EffectsQuality=0
sg.FoliageQuality=0

In sandstorms GameUserSettings.ini set value to 400 or what you want

("r.Streaming.PoolSize", (Value=400,bModified=True)

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
