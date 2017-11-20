# SquadOpti


Updated 11/20



Unpack Squad-Root.pak located here then edit the files: 

%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Content/Paks/




<<<<<<<<<<<<<=======================>>>>>>>>>>>>>






Got to unpak or use the Engine.ini method again

Updated 11/19

Always testing stuff contact me twitch.tv/smoothschannel or discord

shout out to the mod who deleted my forum post




<<<<<<<<<<<<<=======================>>>>>>>>>>>>>




Set in-game graphics settings to medium to get anti aliasing options to work* in game on/off after applying these configs commands in configs will still work.

Bloom has to be on in-game for lens flare to work b/c they have values in GameUserSettings.ini like other settings.

They need to fix the SSAO on/off resets settings to AmbientOcclusionLevels=2 and AmbientOcclusionRadiusScale=1.200000 default engine is levels=3 and radiusscale=1.2 is too much and looks bad.
You can leave SSAO on in-game and then set the settings AmbientOcclusionLevels=3 or 4 and AmbientOcclusionRadiusScale=0.100000 and restart to make SSAO look better but if you turn it off you need to do this again.




<<<<<<<<<<<<<=======================>>>>>>>>>>>>>



Open DefaultEngine.ini:

%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultEngine.ini



<<<<<<<<<<<<<=======================>>>>>>>>>>>>>




Disable-ish logs: 

[Core.Log] 
Global=off ; delete LogAnalytics=log and LogEasyAntiCheatServer=log




<<<<<<<<<<<<<=======================>>>>>>>>>>>>>




Lower audio channels: 

MaxChannels=96  ; find and edit lowest i would use is 64




<<<<<<<<<<<<<=======================>>>>>>>>>>>>>




Paste under [systemSettings] code 

;My Config

;ViewDistanceQuality

r.SkeletalMeshLODBias=0
r.ViewDistanceScale=0.8 ; Lowest hardcoded
r.MipMapLODBias=0 ; added 

;ShadowQuality ; Use shadow config to change them in game

;PostProcessQuality

r.MotionBlurQuality=0
r.AmbientOcclusionMipLevelFactor=0.4
r.AmbientOcclusionMaxQuality=100
r.AmbientOcclusionLevels=-1
r.AmbientOcclusionRadiusScale=0.2
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=1000
r.LensFlareQuality=3
r.SceneColorFringeQuality=1
r.EyeAdaptationQuality=0
r.BloomQuality=1
r.FastBlurThreshold=0
r.Upscale.Quality=3
r.Tonemapper.GrainQuantization=1
r.LightShaftQuality=1
r.Filter.SizeScale=1
r.Tonemapper.Quality=5

;TextureQuality

r.Streaming.MipBias=0
r.MaxAnisotropy=16 ; Set to 16
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=3000
r.Streaming.MaxEffectiveScreenSize=0

;EffectsQuality

r.TranslucencyLightingVolumeDim=64
r.RefractionQuality=1
r.SSR.Quality=1
r.SceneColorFormat=4
r.DetailMode=2
r.TranslucencyVolumeBlur=1
r.MaterialQualityLevel=1 ; High quality
r.SSS.Scale=0
r.SSS.SampleSet=0
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=1.0
r.ParticleLightQuality=2
r.MinTimeBetweenTicks=8
r.ParticleMinTimeBetweenTicks=16  ; set to 16

;FoliageQuality

foliage.DensityScale=0.6 ; Lowest hardcoded
grass.DensityScale=0.6 ; Lowest hardcoded
;foliage.DiscardDataOnLoad=0 ; void 
;grass.DiscardDataOnLoad=0 ; void
grass.MaxUpdateFrequency=30 ; added 

;Extra
t.MaxFPS=300
r.SceneColorFringe.Max=0.5
r.FinishCurrentFrame=0 
r.OneFrameThreadLag=1








<<<<<<<<<<<<<=======================>>>>>>>>>>>>>








;Extra Add what you want   
r.TranslucencyLightingVolumeInnerDistance=64
r.TranslucencyLightingVolumeOuterDistance=64
t.MaxFPS=300
r.VirtualTexture=0
r.RHICmdBypass=0
r.FinishCurrentFrame=0
r.OneFrameThreadLag=1
r.EarlyZPass=0
r.BlurGBuffer=0
r.SkeletalMeshLODRadiusScale=1.0 ; low 0.25
r.StaticMeshLODDistanceScale=1.0 ; low 0.25
r.LightShaftDownSampleFactor=0
r.SceneColorFringe.Max=0.5
r.SeparateTranslucency=0
r.Decal.FadeScreenSizeMult=0
r.ReflectionEnvironment=0 ; Use 1 if you want to use TXAA/MIX to prevent flickering      
r.TiledDeferredShading=0  
r.TiledDeferredShading.MinimumCount=0
r.TiledReflectionEnvironmentMinimumCount=0
r.Decal.FadeScreenSizeMult=0
r.Atmosphere=0 ; why did i put this here?
r.GBufferFormat=0
r.TextureStreaming=1
r.DefaultFeature.AmbientOcclusion=0
r.DefaultFeature.AmbientOcclusionStaticFraction=0
r.DefaultFeature.AntiAliasing=0
r.DefaultFeature.AutoExposure=0
r.DefaultFeature.Bloom=0
r.DefaultFeature.LensFlare=0
r.DefaultFeature.MotionBlur=0








<<<<<<<<<<<<<=======================>>>>>>>>>>>>>









Change shadows in game:

Edit DefaultScalability.ini and BaseScalability.ini: ShadowQuality @ 0 @ 1 @ 2 @ 3 to whatever you like and you can change them in game
%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultScalability.ini
%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Engine/Config/BaseScalability.ini

i use this....

[ShadowQuality@0]
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
r.AllowLandscapeShadows=0 ; Added
r.LightMaxDrawDistanceScale=0 ; Added

[ShadowQuality@1]
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=2048
r.Shadow.MaxCSMResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=1.0
r.Shadow.CSM.TransitionScale=1.0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.VolumetricFog.GridPixelSize=0
r.VolumetricFog.GridSizeZ=0
r.AllowLandscapeShadows=0 ; Added
r.LightMaxDrawDistanceScale=1.0 ; Added

[ShadowQuality@2]
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=2048
r.Shadow.MaxCSMResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.4
r.Shadow.CSM.TransitionScale=1.0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.VolumetricFog.GridPixelSize=0
r.VolumetricFog.GridSizeZ=0
r.AllowLandscapeShadows=0 ; Added
r.LightMaxDrawDistanceScale=1.0 ; Added

[ShadowQuality@3]
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=4096
r.Shadow.MaxCSMResolution=4096
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.4
r.Shadow.CSM.TransitionScale=1.0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.VolumetricFog=0
r.VolumetricFog.GridPixelSize=0
r.VolumetricFog.GridSizeZ=0
r.AllowLandscapeShadows=0 ; Added
r.LightMaxDrawDistanceScale=1.0 ; Added









<<<<<<<<<<<<<=======================>>>>>>>>>>>>>







Skip intro video:

%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultGame.ini
Add a ; in front of the command below:
;+StartupMovies=squad_intro_movie









<<<<<<<<<<<<<=======================>>>>>>>>>>>>>







Max fps config soon or you can scroll down and make one real quick using my other lowest settings configs 







<<<<<<<<<<<<<=======================>>>>>>>>>>>>>











Max raw settings: 

;ViewDistanceQuality

r.SkeletalMeshLODBias=-1
r.ViewDistanceScale=10.0
r.MipMapLODBias=-1 ; added 

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
r.AllowLandscapeShadows=1 ; Added

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
r.MaxAnisotropy=16 ; Set to 16
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
r.MaterialQualityLevel=1 ; High quality
r.SSS.Scale=1
r.SSS.SampleSet=2
r.SSS.Quality=1
r.SSS.HalfRes=0
r.EmitterSpawnRateScale=1.0
r.ParticleLightQuality=2
r.MinTimeBetweenTicks=8
r.ParticleMinTimeBetweenTicks=16  ; set to 16

;FoliageQuality

foliage.DensityScale=1.0
grass.DensityScale=1.0
;foliage.DiscardDataOnLoad=0 ; void 
;grass.DiscardDataOnLoad=0 ; void
grass.MaxUpdateFrequency=30 ; added 

;Extra
t.MaxFPS=300













Latest stuff is ABOVE this^















<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

New simple method no need to unpak :) 
Works with any unreal game.
Paste under code in Engine.ini
Always testing stuff contact me twitch.tv/smoothschannel or discord

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

MY CONFIG:

%localappdata%/Squad/Saved/Config/WindowsNoEditor/Engine.ini 

[Core.Log]
Global=off

[Audio]
MaxChannels=96
UseAudioThread=True

[/Script/Engine.RendererSettings]
r.SkeletalMeshLODBias=-1
r.ViewDistanceScale=0.8
r.MipMapLODBias=-1
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=4096
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.4
r.Shadow.CSM.TransitionScale=1
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=1
r.MotionBlurQuality=0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=2048
r.LensFlareQuality=2
r.SceneColorFringeQuality=1
r.EyeAdaptationQuality=0
r.BloomQuality=1
r.FastBlurThreshold=0
r.Upscale.Quality=3
r.Tonemapper.GrainQuantization=1
r.LightShaftQuality=0
r.Filter.SizeScale=1
r.Tonemapper.Quality=5
r.Streaming.MipBias=0
r.MaxAnisotropy=16
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=6144
r.TranslucencyLightingVolumeDim=64
r.TranslucencyLightingVolumeInnerDistance=64
r.TranslucencyLightingVolumeOuterDistance=64
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=4
r.DetailMode=2
r.TranslucencyVolumeBlur=1
r.MaterialQualityLevel=1
r.SSS.Scale=0
r.SSS.SampleSet=0
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=0.5
r.ParticleMinTimeBetweenTicks=16
r.ParticleLightQuality=2
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=30
t.MaxFPS=300
r.VirtualTexture=0
r.RHICmdBypass=0
r.FinishCurrentFrame=0
r.OneFrameThreadLag=1
r.EarlyZPass=0
r.BlurGBuffer=0
r.SkeletalMeshLODRadiusScale=1.0
r.StaticMeshLODDistanceScale=1.0
r.LightShaftDownSampleFactor=0
r.SceneColorFringe.Max=0.5
r.SeparateTranslucency=0

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

MY MAX FPS CONFIG:

%localappdata%/Squad/Saved/Config/WindowsNoEditor/Engine.ini 
 
[Core.Log]
Global=off

[Audio]
MaxChannels=64

[/Script/Engine.RendererSettings]
r.SkeletalMeshLODBias=1
r.ViewDistanceScale=0.8
r.MipMapLODBias=0
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=2
r.Shadow.MaxResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.35
r.Shadow.CSM.TransitionScale=1
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0
r.MotionBlurQuality=0
r.AmbientOcclusionMipLevelFactor=0
r.AmbientOcclusionMaxQuality=0
r.AmbientOcclusionLevels=0
r.AmbientOcclusionRadiusScale=0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=300
r.LensFlareQuality=0
r.SceneColorFringeQuality=0
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=0
r.Upscale.Quality=0
r.Tonemapper.GrainQuantization=1
r.LightShaftQuality=0
r.Filter.SizeScale=0
r.Tonemapper.Quality=2
r.Streaming.MipBias=1
r.MaxAnisotropy=0
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=3000
r.TranslucencyLightingVolumeDim=24
r.TranslucencyLightingVolumeInnerDistance=24
r.TranslucencyLightingVolumeOuterDistance=24
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=4
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
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=10
r.TiledDeferredShading=0
r.TiledDeferredShading.MinimumCount=0
r.TiledReflectionEnvironmentMinimumCount=0
r.Decal.FadeScreenSizeMult=0
r.SkeletalMeshLODRadiusScale=1
r.StaticMeshLODDistanceScale=0.25
r.VirtualTexture=0
r.RHICmdBypass=0
t.MaxFPS=400
r.Atmosphere=0
r.GBufferFormat=0
r.SeparateTranslucency=0
r.EarlyZPass=0
r.TextureStreaming=1
r.DefaultFeature.AmbientOcclusion=0
r.DefaultFeature.AmbientOcclusionStaticFraction=0
r.DefaultFeature.AntiAliasing=0
r.DefaultFeature.AutoExposure=0
r.DefaultFeature.Bloom=0
r.DefaultFeature.LensFlare=0
r.DefaultFeature.MotionBlur=0

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

MAX FPS CONFIG:

%localappdata%/Squad/Saved/Config/WindowsNoEditor/Engine.ini 

[Core.Log]
Global=off

[Audio]
MaxChannels=64

[/Script/Engine.RendererSettings]
r.SkeletalMeshLODBias=1.5
r.ViewDistanceScale=0.8
r.MipMapLODBias=0
r.LightFunctionQuality=0
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=0
r.Shadow.MaxResolution=0
r.Shadow.RadiusThreshold=0
r.Shadow.DistanceScale=0
r.Shadow.CSM.TransitionScale=0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0
r.MotionBlurQuality=0
r.AmbientOcclusionMipLevelFactor=0
r.AmbientOcclusionMaxQuality=0
r.AmbientOcclusionLevels=0
r.AmbientOcclusionRadiusScale=0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=300
r.LensFlareQuality=0
r.SceneColorFringeQuality=0
r.EyeAdaptationQuality=0
r.BloomQuality=0
r.FastBlurThreshold=0
r.Upscale.Quality=0
r.Tonemapper.GrainQuantization=1
r.LightShaftQuality=0
r.Filter.SizeScale=0
r.Tonemapper.Quality=2
r.Streaming.MipBias=2  
r.MaxAnisotropy=0
r.Streaming.LimitPoolSizeToVRAM=0
r.Streaming.PoolSize=1000
r.TranslucencyLightingVolumeDim=16 
r.TranslucencyLightingVolumeInnerDistance=16  
r.TranslucencyLightingVolumeOuterDistance=16 
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=2          ; Use 4 if you use TXAA/MIX to prevent TXAA ghosting      
r.DetailMode=0
r.TranslucencyVolumeBlur=0
r.MaterialQualityLevel=0
r.SSS.Scale=0
r.SSS.SampleSet=0
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=0
r.ParticleMinTimeBetweenTicks=24
r.ParticleLightQuality=0
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=10
r.ReflectionEnvironment=0          ; Use 1 if you want to use TXAA/MIX to prevent flickering      
r.TiledDeferredShading=0  
r.TiledDeferredShading.MinimumCount=0
r.TiledReflectionEnvironmentMinimumCount=0
r.Decal.FadeScreenSizeMult=0
r.SkeletalMeshLODRadiusScale=0.25
r.StaticMeshLODDistanceScale=0.25
r.VirtualTexture=0
r.RHICmdBypass=0
t.MaxFPS=400       
r.Atmosphere=0
r.GBufferFormat=0
r.SeparateTranslucency=0
r.EarlyZPass=0
r.TextureStreaming=1
r.DefaultFeature.AmbientOcclusion=0
r.DefaultFeature.AmbientOcclusionStaticFraction=0
r.DefaultFeature.AntiAliasing=0
r.DefaultFeature.AutoExposure=0
r.DefaultFeature.Bloom=0
r.DefaultFeature.LensFlare=0
r.DefaultFeature.MotionBlur=0

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

Unpack method below (not needed anymore)

Download: UE4PakUnpacker.exe (941,568 bytes) (you need to find the download link from google)
Unpack: pakchunk0-WindowsNoEditor.pak
Found in:
%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Content/Paks/

Now you can open up DefaultEngine.ini:
%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultEngine.ini

Find and Edit these commands are already in the file:

MaxChannels=64  (Faster cpu use 96 or default 128)
Turn off logging: Find: [Core.Log] Add this: Global=off (remove all blahblah=log stuff)
r.GBufferFormat=0
r.SeparateTranslucency=0
r.EarlyZPass=0

Paste under [systemSettings] code 

( SCROLL UP FOR THE CONFIGS )

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

Skip intro video:

%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultGame.ini
Add a ; in front of the command below:
;+StartupMovies=squad_intro_movie

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

Load up any map to test:

%SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultGame.ini
Change: MainMenuMap=/Game/Maps/EntryMap
Example: MainMenuMap=/Game/Maps/BASRAH_CITY/Albasrah_invasion_v1

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

Launch options:  
-sm4 (same as -d3d10, test yourself)

<<<<<<<<<<<<<=======================>>>>>>>>>>>>>

For NVIDIA users in control panel change:

Maximum pre-rendered frames: 1  (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel: Single display performance mode
Power management mode: Prefer max performance
Preferred refresh rate: Highest available
Texture filtering anisotropic sample optimization: On
Texture filtering quality: High performance
Vertical sync: Off
