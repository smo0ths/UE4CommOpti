# SquadOpti
**This is my attempts at helping optimize the game. I'll update this thread as time goes on and i learn more about the engine. I just want everyone to have the best fps they can without messing with the game and helping devs out with the game, thanks.**
* 
* **Launch options:  -sm4 (same as -d3d10, results vary)**
* 
* **Download: UE4PakUnpacker.exe (941,568 bytes) (you need to find the download link from google)**
* **Unpack: pakchunk0-WindowsNoEditor.pak**
* **Found in:**
* **Windows key + R: %SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Content/Paks/**
* 
* 
* **Now you can open up DefaultEngine.ini:**
* **Windows key + R: %SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultEngine.ini**
* 
* Find and Edit these commands are already in the file:
* MaxChannels=64  (Faster cpu's use 96 or default 128)
* **Turn off logging:** **Find:** [Core.Log] **Remove:** LogAnalytics=log **Add this:** Global=off
* r.GBufferFormat=0 ;
* 
* 
* **Find: Steam\steamapps\common\Squad\Squad\Config\DefaultEngine.ini**
* **Windows key + R: %SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultEngine.ini**
* 
* **Copy and Paste under [systemSettings]**
* 
* ; VIEWDISTANCE
* r.SkeletalMeshLODBias=1.5
* r.ViewDistanceScale=0.4
* r.MipMapLODBias=0
* ; SHADOW  
* r.LightFunctionQuality=0
* r.ShadowQuality=0
* r.Shadow.CSM.MaxCascades=0
* r.Shadow.MaxResolution=0
* r.Shadow.RadiusThreshold=0
* r.Shadow.DistanceScale=0
* r.Shadow.CSM.TransitionScale=0
* r.DistanceFieldShadowing=0
* r.DistanceFieldAO=0
* r.AllowLandscapeShadows=0
* ; POSTPROCESS
* r.MotionBlurQuality=0
* r.AmbientOcclusionMipLevelFactor=0
* r.AmbientOcclusionMaxQuality=0
* r.AmbientOcclusionLevels=0
* r.AmbientOcclusionRadiusScale=0
* r.DepthOfFieldQuality=0
* r.RenderTargetPoolMin=300
* r.LensFlareQuality=0
* r.SceneColorFringeQuality=0
* r.EyeAdaptationQuality=0
* r.BloomQuality=0
* r.FastBlurThreshold=0
* r.Upscale.Quality=0
* r.Tonemapper.GrainQuantization=0
* r.LightShaftQuality=0
* r.Filter.SizeScale=0
* r.Tonemapper.Quality=2
* ; TEXTURE
* r.Streaming.MipBias=2  
* r.MaxAnisotropy=0
* ;r.Streaming.LimitPoolSizeToVRAM=0 ; nul
* ;r.Streaming.PoolSize=1024 ; nul
* ; EFFECTS
* r.TranslucencyLightingVolumeDim=16
* r.RefractionQuality=0
* r.SSR.Quality=0
* r.SceneColorFormat=2  
* r.DetailMode=0
* r.TranslucencyVolumeBlur=0
* r.MaterialQualityLevel=0
* r.SSS.Scale=0
* r.SSS.SampleSet=0
* r.SSS.Quality=0
* r.SSS.HalfRes=1
* r.EmitterSpawnRateScale=0
* r.DefaultFeature.AutoExposure=0
* r.ParticleMinTimeBetweenTicks=33
* r.ParticleLightQuality=0
; FOLIAGE
* foliage.DensityScale=0.6
* grass.DensityScale=0.6
* grass.MaxUpdateFrequency=10
* foliage.DiscardDataOnLoad=1
* grass.DiscardDataOnLoad=1
* ; EXTRA
* r.ReflectionEnvironment=0  
* r.TiledDeferredShading=0  
* r.Decal.FadeScreenSizeMult=0
* r.SkeletalMeshLODRadiusScale=0.25
* t.MaxFPS=400
* ; END
* 
* 
* **Set in-game graphics settings to medium to get FXAA/TXAA to work when you want to change them on or off.**
* **Updated for Squad v9~**
* **The above is for max fps, below for more configs and stuff.**
* 
* 
* **Skip intro video:**
* 
* **Windows key + R: %SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultGame.ini**
* **Add a ; in front of the command below:**
* ;+StartupMovies=squad_intro_movie


**My config:**

; VIEWDISTANCE
r.SkeletalMeshLODBias=0
r.ViewDistanceScale=0.4
r.MipMapLODBias=0
; SHADOW
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=4096
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.45
r.Shadow.CSM.TransitionScale=0.8
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0
; POSTPROCESS
r.MotionBlurQuality=0
;r.AmbientOcclusionMipLevelFactor=0
;r.AmbientOcclusionMaxQuality=0
;r.AmbientOcclusionLevels=0
;r.AmbientOcclusionRadiusScale=0
r.DepthOfFieldQuality=0
r.RenderTargetPoolMin=300
r.LensFlareQuality=2
r.SceneColorFringeQuality=1
r.EyeAdaptationQuality=0
r.BloomQuality=1
r.FastBlurThreshold=0
r.Upscale.Quality=0
r.Tonemapper.GrainQuantization=0
r.LightShaftQuality=1
r.Filter.SizeScale=1
r.Tonemapper.Quality=2
; TEXTURE
r.Streaming.MipBias=0
r.MaxAnisotropy=8
;r.Streaming.LimitPoolSizeToVRAM=1 ; nul
;r.Streaming.PoolSize=6144 ; nul
; EFFECTS
r.TranslucencyLightingVolumeDim=64
r.RefractionQuality=0
r.SSR.Quality=0
r.SceneColorFormat=3
r.DetailMode=0
r.TranslucencyVolumeBlur=0
r.MaterialQualityLevel=1
r.SSS.Scale=0
r.SSS.SampleSet=0
r.SSS.Quality=0
r.SSS.HalfRes=1
r.EmitterSpawnRateScale=1
r.DefaultFeature.AutoExposure=0
r.ParticleMinTimeBetweenTicks=8
r.ParticleLightQuality=2
; FOLIAGE
foliage.DensityScale=0.6
grass.DensityScale=0.6
grass.MaxUpdateFrequency=10
foliage.DiscardDataOnLoad=1
grass.DiscardDataOnLoad=1
; EXTRA
r.ReflectionEnvironment=0
;r.TiledDeferredShading=0
r.SceneColorFringe.Max=0.35
r.Decal.FadeScreenSizeMult=0
t.MaxFPS=400
; END

 

**For NVIDIA users in control panel change:**

Maximum pre-rendered frames: 1  (test 2 3 4 yourself, lowest is said to have less input lag)
Multi/mixed gpu accel: Single display performance mode
Power management mode: Prefer max performance
Preferred refresh rate: Highest available
Texture filtering anisotropic sample optimization: On
Texture filtering quality: High performance
Vertical sync: Off

 

 

**Change shadows in game:**

**Edit DefaultScalability.ini and BaseScalability.ini: ShadowQuality @ 0 @ 1 @ 2 @ 3 to whatever you like and you can change them in game**
**Windows key + R: %SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultScalability.ini**
**Windows key + R: %SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Engine/Config/BaseScalability.ini**

**i use this....**

**DefaultScalability.ini:**

[ShadowQuality@0]
r.LightFunctionQuality=0
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=0
r.Shadow.MaxResolution=512
r.Shadow.RadiusThreshold=0
r.Shadow.DistanceScale=0
r.Shadow.CSM.TransitionScale=0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0

[ShadowQuality@1]
r.LightFunctionQuality=1
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=0
r.Shadow.MaxResolution=512
r.Shadow.RadiusThreshold=0
r.Shadow.DistanceScale=0
r.Shadow.CSM.TransitionScale=0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0

[ShadowQuality@2]
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.45
r.Shadow.CSM.TransitionScale=0.8
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0

[ShadowQuality@3]
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=4096
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.45
r.Shadow.CSM.TransitionScale=0.8
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0

BaseScalability.ini:

[ShadowQuality@0]
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

[ShadowQuality@1]
r.LightFunctionQuality=1
r.ShadowQuality=0
r.Shadow.CSM.MaxCascades=0
r.Shadow.MaxResolution=0
r.Shadow.RadiusThreshold=0
r.Shadow.DistanceScale=0
r.Shadow.CSM.TransitionScale=0
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0

[ShadowQuality@2]
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=2048
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.45
r.Shadow.CSM.TransitionScale=0.8
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0

[ShadowQuality@3]
r.LightFunctionQuality=1
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=3
r.Shadow.MaxResolution=4096
r.Shadow.RadiusThreshold=0.03
r.Shadow.DistanceScale=0.45
r.Shadow.CSM.TransitionScale=0.8
r.DistanceFieldShadowing=0
r.DistanceFieldAO=0
r.AllowLandscapeShadows=0

**Load up any map to test:**

Windows key + R: %SystemDrive%/Program Files (x86)/Steam/steamapps/common/Squad/Squad/Config/DefaultGame.ini
Change: MainMenuMap=/Game/Maps/EntryMap
Example: MainMenuMap=/Game/Maps/Chora/Chora_AAS_v1
