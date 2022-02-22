~~~~~~~~~~~~~~~~~~~~~~~~~


*updated 2/22/2022

*for UE4 games for reference/customization/optimization/learning

*always testing stuff contact me twitch.tv/smoothschannel or discord (discord.gg/vB8f4fZ7EH)

*my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game


-----------------------------------------------------------------
-------------------------Open Engine.ini-------------------------
-----------------------------------------------------------------


Press:       Windows key + R
Copy/Paste:  %localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Engine.ini
Copy/Paste:  %localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Engine.ini


*copy and paste this in engine.ini under lines in the file


[Core.Log]
Global=off;

[Audio]
MaxChannels=0;------default 0
CommonAudioPoolSize=0;------default 0
UnfocusedVolumeMultiplier=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=70;------default 70 TEXTUREPOOL CACHE

[SystemSettings]
r.DefaultFeature.AntiAliasing=2;------default 2 set 1 for FXAA 2 for TAA 3 for MSAA 0 for none
r.PostProcessAAQuality=3;------default 3 set to 1 or 2 FXAA 3 or 4 TAA
r.ScreenPercentage=100;------default 100 TAAU INPUT RESOLUTION
r.TemporalAA.Upsampling=1;------default 0 changed to 1*
r.TemporalAAUpsampleFiltered=1;------default 1
r.TemporalAAFilterSize=0.5;------default 1 changed to 0.5*
r.TemporalAASamples=4;------default 16 changed to 4*
r.TemporalAACurrentFrameWeight=0.1;------default 0.2 changed to 0.1*
r.TemporalAA.Algorithm=0;------default 0
r.TemporalAA.R11G11B10History=0;------default 0 EXPERIMENTAL
au.RenderThreadPriority=0;------default 0
AudioThread.EnableBatchProcessing=1;------TEST
Compat.UseDXT5NormalMaps=0;------default 0
foliage.DensityScale=0.6;------default 0.8 set to 0.6 for PERFORMANCE
foliage.DitheredLOD=1;------default 1
foliage.LODDistanceScale=1;------default 1
foliage.MinimumScreenSize=0.0001;------default 0.0001
foliage.MinVertsToSplitNode=8192;------default 8192
foliage.OverestimateLOD=1;------default 0 set to 1 for PERFORMANCE
FX.AllowAsyncTick=1;------default 1
FX.BatchAsync=0;------default 0
FX.FXAllowParticleMeshLODs=0;------default 0
FX.MaxCPUParticlesPerEmitter=500;------default 1000 changed to 500*
FX.MaxGPUParticlesSpawnedPerFrame=25000;------default 1048576 changed to 25000*
FX.QualityLevelSpawnRateScaleReferenceLevel=2;------default 2 set to 0 for PERFORMANCE
grass.DensityScale=0.6;------default 1 set to 0.6 for PERFORMANCE
grass.DisableDynamicShadows=0;------default 0 set to 1 for PERFORMANCE
grass.TickInterval=1;------default 1
p.AnimDynamics=1;------default 1 set to 0 for PERFORMANCE
p.AnimDynamicsLODThreshold=-1;------default -1
p.AnimDynamicsRestrictLOD=-1;------default -1
p.AnimDynamicsWind=1;------default 1
p.BatchPhysXTasksSize=3;------default 3
p.ClothPhysics.UseTaskThread=1;------default 1
p.ClothPhysics=1;------default 1 set to 0 for PERFORMANCE
p.RigidBodyLODThreshold=-1;------default -1
p.RigidBodyNode=1;------default 1
r.AllowDownsampledStandardTranslucency=0;------default 0
r.AllowHDR=0;------default 0
r.AllowLandscapeShadows=1;------default 1 set to 0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;------default 1 set to 0 for PERFORMANCE
r.AllowSimpleLights=1;------default 1 set to 0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=0;------default 0
r.AmbientOcclusion.Compute.Smooth=1;------default 1
r.AmbientOcclusion.Compute=1;------default 0 set to 1 for PERFORMANCE
r.AmbientOcclusionLevels=0;------default 3 set to 0 for PERFORMANCE
r.AmbientOcclusionMaxQuality=100;------default 100
r.AmbientOcclusionMipLevelFactor=0.6;------default 0.6
r.AmbientOcclusionRadiusScale=0;------default 1 set to 0 for PERFORMANCE
r.AmbientOcclusionStaticFraction=-1;------default -1
r.AnisotropicMaterials=1;------default 1
r.AOGlobalDFResolution=128;------default 128
r.AOHeightfieldOcclusion=0;------default 0
r.AOQuality=1;------default 1
r.Atmosphere=1;------default 1
r.Bloom.Cross=0;------default 0 set to -0.7777 for ANAMORPHIC BLOOM
r.Bloom.HalfResolutionFFT=0;------default 0 EXPERIMENTAL
r.BloomQuality=3;------default 4 changed to 3*
r.CapsuleShadows=0;------default 1 set to 0 for PERFORMANCE
r.CapsuleShadowsFullResolution=0;------default 0
r.chaos.ReflectionCaptureStaticSceneOnly=1;------default 1
r.ClearCoatNormal=0;------default 0
r.CompileShadersForDevelopment=0;------default 1 set to 0 for PERFORMANCE
r.ContactShadows=0;------default 1 set to 0 for PERFORMANCE
r.CreateShadersOnLoad=0;------default 0
r.D3D11.Depth24Bit=0;------default 0
r.D3D12.Depth24Bit=0;------default 0
r.DBuffer=1;------default 1 set to 0 for PERFORMANCE
r.Decal.FadeDurationScale=1;------default 1 set to 0.6 for PERFORMANCE
r.Decal.FadeScreenSizeMult=1;
r.Decal.StencilSizeThreshold=0.1;------default 0.1
r.DefaultBackBufferPixelFormat=4;------default 4
r.DefaultFeature.AmbientOcclusion=1;------default 1
r.DefaultFeature.AmbientOcclusionStaticFraction=0;------default 0
r.DefaultFeature.AutoExposure.Method=0------default 0
r.DefaultFeature.AutoExposure=0;------default 0
r.DefaultFeature.Bloom=1;------default 1
r.DefaultFeature.LensFlare=1;------default 1
r.DefaultFeature.LightUnits=1;------default 1
r.DefaultFeature.MotionBlur=0;------default 0
r.DeferSkeletalDynamicDataUpdateUntilGDME=0;------default 0 EXPERIMENTAL
r.DeferUniformBufferUpdatesUntilVisible=1;
r.DeferUniformExpressionCaching=1;------default 1
r.DepthOfFieldQuality=1;------default 2 set to 1 or 0 for PERFORMANCE
r.DetailMode=1;------default 1 set to 0 for PERFORMANCE
r.DFDistanceScale=1;------default 1
r.DFFullResolution=0;------default 0
r.DFShadowQuality=3;------default 3 set to 1 for PERFORMANCE
r.DFShadowScatterTileCulling=1;------default 1
r.DFTwoSidedMeshDistanceBias=5;------default 4 changed to 5*
r.DiscardUnusedQuality=0;------default 0
r.DistanceFieldAO=1;------default 0 set to 0 for PERFORMANCE
r.DistanceFieldShadowing=1;------default 1 set to 0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0;------default 0 EXPERIMENTAL
r.DoLazyStaticMeshUpdate=0;------default 0 EXPERIMENTAL
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1;------default 1
r.DoTiledReflections=1;------default 1
r.DrawRectangleOptimization=1;------default 1
r.DX11NVAfterMathEnabled=0;
r.EarlyZPass=2;------default 2
r.EarlyZPassMovable=1;------default 1
r.EarlyZPassOnlyMaterialMasking=1;------default 1
r.Emitter.FastPoolEnable=1;------default 0 changed to 1*
r.EmitterSpawnRateScale=0.5;------default 1 set to 0.5 for PERFORMANCE
r.EnableAsyncComputeTranslucencyLightingVolumeClear=1;------default 1
r.EnableAsyncComputeVolumetricFog=1;
r.EyeAdaptationQuality=2;------default 2
r.FastBlurThreshold=3;------default 3
r.Filter.SizeScale=0.8;------default 0.8
r.FinishCurrentFrame=0;------default 0
r.Fog=1;------default 1
r.ForceSceneHasDecals=0;------default 0
r.FreeSkeletalMeshBuffers=0;------default 0
r.FullScreenMode=0;
r.GBufferFormat=1;------default 1
r.GenerateLandscapeGIData=1;------default 1 set to 0 for PERFORMANCE
r.GenerateMeshDistanceFields=1;------default 1 required for DFSHADOWS and DFAO set to 0 for PERFORMANCE
r.GPUCrash.CollectionEnable=0;------default 1 changed to 0*
r.GPUCrashDebugging=0;------default 0
r.GPUSkin.Limit2BoneInfluences=0;------default 0
r.GTSyncType=0;------default 0
r.HDR.EnableHDROutput=0;------default 0
r.HeightFieldShadowing=0;------default 0
r.HFShadowQuality=2;------default 2
r.HighQualityLightMaps=1;------default 1
r.HZBOcclusion=0;------default 0
r.IrisNormal=0;------default 0
r.LandscapeLOD0DistributionScale=1;------default 1
r.LandscapeLODBias=0;------default 0
r.LandscapeLODDistributionScale=1;------default 1
r.LensFlareQuality=0;------default 2 set to 0 for PERFORMANCE
r.LightFunctionQuality=1;------default 1
r.LightMaxDrawDistanceScale=1;------default 1 set to 0.6 for PERFORMANCE
r.LightShaftQuality=0;------default 1 set to 0 for PERFORMANCE
r.MaterialQualityLevel=1;------default 1 set to 0 for PERFORMANCE
r.MaxAnisotropy=8;------default 4 changed to 8*
r.MinRoughnessOverride=0;------default 0
r.MinScreenRadiusForCSMDepth=0.01;------default 0.01
r.MinScreenRadiusForDepthPrepass=0.03;------default 0.03
r.MinScreenRadiusForLights=0.04;------default 0.03 set to 0.2 for PERFORMANCE
r.MipMapLODBias=0;------default 0
r.MorphTarget.Mode=1;------default 1
r.MotionBlurQuality=0;
r.MSAA.CompositingSampleCount=1;------default 3 changed to 1*
r.MSAACount=1;------default 4 changed to 1*
r.NormalMapsForStaticLighting=1;------default 1 set to 0 for PERFORMANCE
r.NumBufferedOcclusionQueries=1;------default 1
r.OneFrameThreadLag=1;------default 1
r.ParticleLightQuality=1;------default 1 set to 0 for PERFORMANCE
r.ParticleLODBias=0;------default 0
r.ParticleMinTimeBetweenTicks=10;------changed to 10*
r.RayTracing=0;------default 0
r.ReflectionCaptureResolution=128;------default 128 set to 64 for PERFORMANCE
r.ReflectionCaptureSupersampleFactor=1;------default 1
r.ReflectionEnvironment=1;------default 1 set to 0 for PERFORMANCE
r.RefractionQuality=1;------default 2 set to 0 for PERFORMANCE
r.RenderTargetPool.AllowMultipleAliasingDiscardsPerFrame=0;------default 0
r.RenderTargetPool.TransientAliasingMode=2;------default 2
r.RenderTargetPoolMin=400;------default 400
r.SceneColorFormat=3;------default 3
r.SceneColorFringe.Max=-1;------default -1
r.SceneColorFringeQuality=0;------default 1 changed to 0*
r.SceneRenderTargetResizeMethod=0;------default 0
r.SceneRenderTargetResizeMethodForceOverride=0;------default 0
r.SecondaryScreenPercentage.GameViewport=0;------default 0
r.ShaderDevelopmentMode=0;------default 0
r.Shaders.FastMath=1;------default 1
r.Shaders.Optimize=1;------default 1
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;------default 1 set to 0 for PERFORMANCE
r.Shadow.CacheWholeSceneShadows=1;------default 1
r.Shadow.CacheWPOPrimitives=0;------default 0
r.Shadow.CSM.MaxCascades=3;------default 3
r.Shadow.CSM.TransitionScale=1.5;------default 0.8 changed to 1.5*
r.Shadow.CSMDepthBias=5;------default 10 changed to 5*
r.Shadow.DistanceScale=0.85;------default 0.85 set to 0.6 for PERFORMANCE
r.Shadow.FilterMethod=0;------default 0
r.Shadow.MaxCSMResolution=2048;------default 2048
r.Shadow.MaxNumFarShadowCascades=0;------default 10 changed to 0*
r.Shadow.MaxResolution=2048;------default 1024 set to 1024 for PERFORMANCE
r.Shadow.OcclusionCullCascadedShadowMaps=0;------default 0
r.Shadow.PointLightDepthBias=0.007;------default 0.02 changed to 0.007*
r.Shadow.PointLightSlopeScaleDepthBias=5;------default 3 changed to 5*
r.Shadow.RadiusThreshold=0.03;------default 0.04 set to 0.03 for PERFORMANCE
r.Shadow.SpotLightTransitionScale=256;------default 60 changed to 256*
r.Shadow.TransitionScale=120;------default 60 changed to 120*
r.ShadowQuality=3;------default 4 set to 3 for PERFORMANCE
r.SkeletalMeshLODBias=0;------default 0
r.SkeletalMeshLODRadiusScale=1;------default 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=1;------default 0 changed to 1*
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=1;------default 0 changed to 1*
r.SkylightIntensityMultiplier=0.8;------default 1 changed to 0.8
r.SSGI.Enable=0;------default 0
r.SSR.Quality=0;------default 2 set to 0 for PERFORMANCE
r.SSS.Checkerboard=1;------default 2 changed to 1
r.StaticMeshLODDistanceScale=1;------default 1
r.Streaming.MipBias=0;------default 0 set to 1 for PERFORMANCE
r.Streaming.PoolSize.VRAMPercentageClamp=1024;------default 1024
r.Streaming.PoolSize=1000;------default 800 changed to 1000*
r.Streaming.PoolSizeForMeshes=-1;------default -1
r.TessellationAdaptivePixelsPerTriangle=9999999;------default 48 set to 9999999 for PERFORMANCE
r.TextureStreaming=1;------default 1
r.TiledDeferredShading=1;------default 1 set to 0 for PERFORMANCE
r.Tonemapper.EmulateHDR=0;
r.Tonemapper.GrainQuantization=1;------default 1 0 for PERFORMANCE
r.Tonemapper.Quality=0;------default 5 changed to 0*
r.Tonemapper.Sharpen=0;------default 1 changed to 0*
r.TonemapperGamma=0;
r.TranslucencyLightingVolume=1;------default 1 set to 0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;------default 48 set to 32 for PERFORMANCE
r.ViewDistanceScale=1;------default 1 set to 0.8 for PERFORMANCE
r.VolumetricCloud.ShadowMap=0;------default 1 changed to 0*
r.VolumetricCloud.SkyAO=0;------default 1 changed to 0*
r.VolumetricFog.GridPixelSize=32;------default 16 changed to 32*
r.VolumetricFog.HistoryMissSupersampleCount=1;------default 4 set to 0 for PERFORMANCE
r.VolumetricFog.InjectShadowedLightsSeparately=0;------default 1 set to 0 for PERFORMANCE
r.VolumetricFog=1;------default 1 set to 0 for PERFORMANCE
r.VSync=0;
r.Vulkan.Depth24Bit=0;------default 0
RHI.SyncInterval=0;------default 1 changed to 0*
RHI.SyncSlackMS=0;------default 10 changed to 0*


------------------------------------------------------------------------------------------------------
-------------------------AA settings i use Copy/Paste over or experiment------------------------------
------------------------------------------------------------------------------------------------------


TAA
r.DefaultFeature.AntiAliasing=2;------default 2 set 1 for FXAA 2 for TAA 3 for MSAA 0 for none
r.PostProcessAAQuality=3;------default 3 set to 1 or 2 FXAA 3 or 4 TAA
r.ScreenPercentage=100;------default 100 TAAU INPUT RESOLUTION

TAAU for PERFORMANCE
r.DefaultFeature.AntiAliasing=2;------default 2 set 1 for FXAA 2 for TAA 3 for MSAA 0 for none
r.PostProcessAAQuality=3;------default 3 set to 1 or 2 FXAA 3 or 4 TAA
r.ScreenPercentage=86.66;------default 100 TAAU INPUT RESOLUTION

FXAA
r.DefaultFeature.AntiAliasing=1;------default 2 set 1 for FXAA 2 for TAA 3 for MSAA 0 for none
r.PostProcessAAQuality=2;------default 3 set to 1 or 2 FXAA 3 or 4 TAA
r.ScreenPercentage=100;------default 100 TAAU INPUT RESOLUTION

NONE
r.DefaultFeature.AntiAliasing=0;------default 2 set 1 for FXAA 2 for TAA 3 for MSAA 0 for none
r.PostProcessAAQuality=0;------default 3 set to 1 or 2 FXAA 3 or 4 TAA
r.ScreenPercentage=100;------default 100 TAAU INPUT RESOLUTION


----------------------------------------------------------------
-------------------------Open Input.ini-------------------------
----------------------------------------------------------------


%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Input.ini
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Input.ini


*edit input commands or add them


[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.2;------default 0.2
ButtonRepeatDelay=0.1;------default 0.1
DoubleClickTime=0.1;------default 0.25
ConsoleKeys=Tilde;


---------------------------------------------------------------------------
-------------------------Open GameUserSettings.ini-------------------------
---------------------------------------------------------------------------

 
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/GameUserSettings.ini


*these will overwrite your config so make sure any setting GameUserSettings.ini is set the way you want


AudioQualityLevel=3
MaxAnisotropy=8
bUseVSync=0
MaxFPS=163
FrameRateLimit=163
MenuFrameRateLimit=163
HDRDisplayOutputNits=300;------set your monitors nits if using hdr
DoubleKeyPressTime=0.1
TextureStreamPoolSizeStorage=1000;------only way to change r.Streaming.PoolSize in squad
DistanceFieldShadows=1;
Gamma=2.2
TAASampleStorage=4
bRTXEnabled=1
bRTXReflectionsEnabled=0
bRTXShadowsEnabled=0
bRTXAmbientOcclusionEnabled=0
DlssQualitySetting=1
ResolutionScaleModifier=1
DFAO=1
Tessellation=0
TessellationMode=48
bTelemetryEnabled=0
bUseDynamicResolution=0
FullscreenMode=0
PreferredFullscreenMode=0
ContactShadows=0
PostFX_Saturation=1.2
PostFX_Sharpness=0
OverrideOptions=(("r.PlaceHolder1", (Value=0,bModified=True)),("r.PlaceHolder2", (Value=1,bModified=False)));------works like engineini but in gameusersettingsini


*set your scalability groups, 0=low/1=medium/2=high/3=epic/4=cinematic (4 gets clamped)


[ScalabilityGroups]
sg.ResolutionQuality=100;
sg.ViewDistanceQuality=2;
sg.AntiAliasingQuality=2;
sg.PostProcessQuality=2;
sg.ShadowQuality=2;
sg.TextureQuality=2;
sg.EffectsQuality=2;
sg.FoliageQuality=2;
sg.ShadingQuality=2;
sg.AnimationQuality=2;
sg.ViewDistanceQuality.NumLevels=5;
sg.AntiAliasingQuality.NumLevels=5;
sg.PostProcessQuality.NumLevels=5;
sg.ShadowQuality.NumLevels=5;
sg.TextureQuality.NumLevels=5;
sg.EffectsQuality.NumLevels=5;
sg.FoliageQuality.NumLevels=5;
sg.ShadingQuality.NumLevels=5;
sg.AnimationQuality.NumLevels=5;


-------------------------------------------------------------------------
-------------------------Open DeviceProfiles.ini-------------------------
-------------------------------------------------------------------------

   
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/DeviceProfiles.ini


*textures lods experiment for performance (wip)


-------------------------------------------------------------------
-------------------------for NVIDIA users--------------------------
-------------------------------------------------------------------


Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method)

Adjust image settings set to Performance and apply then Select Use the advanced 3D image settings and apply

In manage 3D settings:

Anisotropic filtering:  Off for perf. App-controlled or force your own setting for quality (8x is nice)

Low latency mode:  
1. Off and ~85% gpu usage for most med-lower end systems (assuming you cap fps correctly)
2. On feels consistent (i use this and reflex in games that support it)
3. Ultra and relfex (in-game) feels good when gpu usage is ~97%

Power management mode:  Prefer max performance  (this is the "+ boost" in reflex + boost)

Preferred refresh rate:  Highest available

Texture filtering - anisotropic sample optimization:  on  (off will look better if this even works)

Texture filtering - Negative LOD bias:  Allow

Texture filtering quality:  High performance

Vertical sync:  Off


---------------------------------------------------------------------------------------------------
-------------------------How to enable Message-signaled interrupts (MSIs)--------------------------
---------------------------------------------------------------------------------------------------


use Wtools v1.0.2.0.exe (Wagnardsoft Tools) enable it and restart

or

when you make your driver setup.exe using NVCleanstall enabling it in advanced settings

or

find ID: open device manager right click your GPU properties and click on events tab

looks like this:

HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties

find in regedit and set MSISupported to 1 then restart


~~~~~~~~~~~~~~~~~~~~~~~~~
