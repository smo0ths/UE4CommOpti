
#### updated 3/11/2022 :ramen:

###### for UE4 games for reference/customization/optimization/learning

###### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/vB8f4fZ7EH)

###### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

---

<details><summary>Open Engine.ini and copy paste under lines in the file</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Engine.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Engine.ini
</p>
</details>

```python
[Core.Log]
Global=off;

[Audio]
MaxChannels=64;------def 0------64 for PERFORMANCE
CommonAudioPoolSize=0;------def 0
UnfocusedVolumeMultiplier=1;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=70;------def 70 TEXTUREPOOL CACHE

[SystemSettings]
r.DefaultFeature.AntiAliasing=2;------def 2------1 FXAA 2 TAA 3 MSAA 0 OFF
r.PostProcessAAQuality=3;------def 3------1/2 FXAA 3/4/5/6 TAA 0 OFF
r.ScreenPercentage=100;------def 100 TAAU INPUT RESOLUTION
r.TemporalAA.Algorithm=0;------def 0
r.TemporalAA.AllowDownsampling=0;------def 1------changed to 0*------1 for PERFORMANCE
r.TemporalAA.HistoryScreenPercentage=100;------def 100
r.TemporalAA.R11G11B10History=0;------def 0------EXPERIMENTAL
r.TemporalAA.Upsampling=0;------def 0
r.TemporalAA.Upscaler=1;------def 1
r.TemporalAACatmullRom=0;------def 0
r.TemporalAACurrentFrameWeight=0;------def 0.2------changed to 0*
r.TemporalAAFilterSize=1;------def 1
r.TemporalAAPauseCorrect=1;------def 1
r.TemporalAASamples=2;------def 16------changed to 2*
r.TemporalAAUpsampleFiltered=1;------def 1
au.RenderThreadPriority=0;------def 0
AudioThread.BatchAsyncBatchSize=128;------def 128
AudioThread.EnableBatchProcessing=1;------def 1
Compat.UseDXT5NormalMaps=0;------def 0
foliage.DensityScale=0.6;------def 0.8------0.6 for PERFORMANCE
foliage.DitheredLOD=1;------def 1
foliage.LODDistanceScale=1;------def 1
foliage.MinimumScreenSize=0.0001;------def 0.0001
foliage.MinVertsToSplitNode=8192;------def 8192
foliage.OverestimateLOD=0;------def 0
FX.AllowAsyncTick=1;------def 1
FX.AllowGPUSorting=1;------def 1
FX.BatchAsync=0;------def 0
FX.BatchAsyncBatchSize=32;------def 0------changed to 32*
FX.FXAllowParticleMeshLODs=1;------def 0------changed to 1*
FX.MaxCPUParticlesPerEmitter=100;------def 1000------changed to 100*
FX.MaxGPUParticlesSpawnedPerFrame=104858;------def 1048576------changed to 104858*
FX.QualityLevelSpawnRateScaleReferenceLevel=2;------def 2
grass.DensityScale=0.6;------def 1------0.6 for PERFORMANCE
grass.DisableDynamicShadows=0;------def 0------1 for PERFORMANCE
grass.TickInterval=1;------def 1
p.AllowCachedOverlaps=1;------def 1
p.AnimDynamics=1;------def 1------0 for PERFORMANCE
p.AnimDynamicsLODThreshold=-1;------def -1
p.AnimDynamicsRestrictLOD=-1;------def -1
p.AnimDynamicsWind=1;------def 1
p.BatchPhysXTasksSize=3;------def 3
p.ClothPhysics.UseTaskThread=1;------def 1
p.ClothPhysics=1;------def 1------0 for PERFORMANCE
p.RigidBodyLODThreshold=-1;------def -1
p.RigidBodyNode=1;------def 1
r.AllowDownsampledStandardTranslucency=0;------def 0
r.AllowHDR=0;------def 0
r.AllowLandscapeShadows=1;------def 1------0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1;------def 1------0 for PERFORMANCE
r.AllowSimpleLights=1;------def 1------0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=0;------def 0
r.AmbientOcclusion.Compute.Smooth=1;------def 1
r.AmbientOcclusion.Compute=1;------def 0------1 for PERFORMANCE
r.AmbientOcclusionLevels=0;------def 3------0 for PERFORMANCE
r.AmbientOcclusionMaxQuality=100;------def 100
r.AmbientOcclusionMipLevelFactor=0.6;------def 0.6
r.AmbientOcclusionRadiusScale=0;------def 1------0 for PERFORMANCE
r.AmbientOcclusionStaticFraction=-1;------def -1
r.AnisotropicMaterials=0;------def 1
r.AOApplyToStaticIndirect=0;------def 0
r.AOComputeShaderNormalCalculation=0;------def 0
r.AOGlobalDFResolution=128;------def 128
r.AOHeightfieldOcclusion=0;------def 0
r.AOMaxViewDistance=1000;------def 20000------changed to 1000
r.AOOverwriteSceneColor=0;------def 0
r.AOQuality=1;------def 1
r.AOSampleSet=1;------def 1
r.AOViewFadeDistanceScale=0.7;------def 0.7
r.Atmosphere=1;------def 1
r.Bloom.Cross=0;------def 0-------Anamorphic 0.7777
r.Bloom.HalfResolutionFFT=0;------def 0------EXPERIMENTAL
r.BloomQuality=3;------def 4------changed to 3*
r.CapsuleShadows=0;------def 1------0 for PERFORMANCE
r.CapsuleShadowsFullResolution=0;------def 0
r.chaos.ReflectionCaptureStaticSceneOnly=1;------def 1
r.ClearCoatNormal=0;------def 0
r.CompileShadersForDevelopment=0;------def 1------0 for PERFORMANCE
r.ContactShadows=0;------def 1------0 for PERFORMANCE
r.CreateShadersOnLoad=1;------def 0------changed to 1*
r.D3D11.Depth24Bit=0;------def 0
r.D3D12.Depth24Bit=0;------def 0
r.DBuffer=1;------def 1------0 for PERFORMANCE
r.Decal.FadeDurationScale=1;------def 1------0.6 for PERFORMANCE
r.Decal.FadeScreenSizeMult=1;
r.Decal.StencilSizeThreshold=0.1;------def 0.1
r.DefaultBackBufferPixelFormat=4;------def 4
r.DefaultFeature.AmbientOcclusion=1;------def 1
r.DefaultFeature.AmbientOcclusionStaticFraction=0;------def 0
r.DefaultFeature.AutoExposure.Method=0------def 0
r.DefaultFeature.AutoExposure=0;------def 0
r.DefaultFeature.Bloom=1;------def 1
r.DefaultFeature.LensFlare=1;------def 1
r.DefaultFeature.LightUnits=1;------def 1
r.DefaultFeature.MotionBlur=0;------def 0
r.DeferSkeletalDynamicDataUpdateUntilGDME=0;------def 0------EXPERIMENTAL
r.DeferUniformBufferUpdatesUntilVisible=1;
r.DeferUniformExpressionCaching=1;------def 1
r.DepthOfFieldQuality=0;------def 2------0 for PERFORMANCE
r.DetailMode=1;------def 1------0 for PERFORMANCE
r.DFDistanceScale=1;------def 1
r.DFFullResolution=0;------def 0
r.DFShadowQuality=2;------def 3------1 or 2 for PERFORMANCE
r.DFShadowScatterTileCulling=1;------def 1
r.DFTwoSidedMeshDistanceBias=5;------def 4------changed to 5*
r.DiscardUnusedQuality=0;------def 0
r.DistanceFieldAO=1;------def 0------0 for PERFORMANCE
r.DistanceFieldShadowing=1;------def 1------0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0;------def 0------EXPERIMENTAL
r.DoLazyStaticMeshUpdate=0;------def 0------EXPERIMENTAL
r.DoPrepareDistanceFieldSceneAfterRHIFlush=1;------def 1
r.DoTiledReflections=1;------def 1
r.Downsample.Quality=1;------def 1
r.DrawRectangleOptimization=1;------def 1
r.DX11NVAfterMathEnabled=0;
r.EarlyZPass=2;------def 2
r.EarlyZPassMovable=1;------def 1
r.EarlyZPassOnlyMaterialMasking=1;------def 1
r.Emitter.FastPoolEnable=1;------def 0------changed to 1*
r.EmitterSpawnRateScale=0.5;------def 1------0.5 for PERFORMANCE
r.EnableAsyncComputeTranslucencyLightingVolumeClear=1;------def 1
r.EnableAsyncComputeVolumetricFog=1;
r.EyeAdaptationQuality=2;------def 2
r.FastBlurThreshold=3;------def 3
r.Filter.SizeScale=0.8;------def 0.8
r.FinishCurrentFrame=0;------def 0
r.Fog=1;------def 1
r.ForceSceneHasDecals=0;------def 0
r.FreeSkeletalMeshBuffers=0;------def 0
r.FullScreenMode=0;
r.GBufferFormat=1;------def 1
r.GenerateLandscapeGIData=1;------def 1------0 for PERFORMANCE
r.GenerateMeshDistanceFields=1;------def 1 required for DFSHADOWS and DFAO------0 for PERFORMANCE
r.GPUCrash.CollectionEnable=0;------def 1------changed to 0*
r.GPUCrashDebugging=0;------def 0
r.GPUSkin.Limit2BoneInfluences=0;------def 0
r.GTSyncType=0;------def 0
r.HDR.EnableHDROutput=0;------def 0
r.HeightFieldShadowing=0;------def 0
r.HFShadowQuality=2;------def 2
r.HighQualityLightMaps=1;------def 1
r.HZBOcclusion=0;------def 0
r.IrisNormal=0;------def 0
r.LandscapeLOD0DistributionScale=1;------def 1
r.LandscapeLODBias=0;------def 0
r.LandscapeLODDistributionScale=1;------def 1
r.LensFlareQuality=0;------def 2------0 for PERFORMANCE
r.LightFunctionQuality=1;------def 1
r.LightMaxDrawDistanceScale=1;------def 1------0.6 for PERFORMANCE
r.LightShaftQuality=0;------def 1------0 for PERFORMANCE
r.MaterialQualityLevel=1;------def 1------0 for PERFORMANCE
r.MaxAnisotropy=8;------def 4------changed to 8*
r.MaxCSMRadiusToAllowPerObjectShadows=300;------def 8000 changed to 300*
r.MinRoughnessOverride=0.1;------def 0------changed to 0.1*
r.MinScreenRadiusForCSMDepth=0.01;------def 0.01
r.MinScreenRadiusForDepthPrepass=0.03;------def 0.03
r.MinScreenRadiusForLights=0.04;------def 0.03------changed to 0.04*------0.2 for PERFORMANCE
r.MipMapLODBias=0;------def 0
r.MorphTarget.Mode=1;------def 1
r.MotionBlurQuality=0;
r.MSAA.CompositingSampleCount=1;------def 3------changed to 1*
r.MSAACount=1;------def 4------changed to 1*
r.NormalMapsForStaticLighting=1;------def 1------0 for PERFORMANCE
r.NumBufferedOcclusionQueries=1;------def 1
r.OneFrameThreadLag=1;------def 1
r.ParticleLightQuality=1;------def 1------0 for PERFORMANCE
r.ParticleLODBias=0;------def 0
r.ParticleMinTimeBetweenTicks=10;-----------changed to 10*
r.PostProcessAllowBlendModes=1;------def 1
r.RayTracing=0;------def 0
r.ReflectionCaptureSupersampleFactor=1;------def 1
r.ReflectionEnvironment=1;------def 1------0 for PERFORMANCE
r.RefractionQuality=1;------def 2------0 for PERFORMANCE
r.RenderTargetPool.AllowMultipleAliasingDiscardsPerFrame=0;------def 0
r.RenderTargetPool.TransientAliasingMode=2;------def 2
r.RenderTargetPoolMin=1000;------def 400------changed to 1000*
r.SceneColorFormat=3;------def 3
r.SceneColorFringe.Max=-1;------def -1
r.SceneColorFringeQuality=0;------def 1------changed to 0*
r.SceneRenderTargetResizeMethod=0;------def 0
r.SceneRenderTargetResizeMethodForceOverride=0;------def 0
r.SecondaryScreenPercentage.GameViewport=0;------def 0
r.SeparateTranslucency=0;------def 1------changed to 0*
r.ShaderDevelopmentMode=0;------def 0
r.Shaders.FastMath=1;------def 1
r.Shaders.Optimize=1;------def 1
r.Shadow.CachedShadowsCastFromMovablePrimitives=1;------def 1------0 for PERFORMANCE
r.Shadow.CacheWholeSceneShadows=1;------def 1
r.Shadow.CacheWPOPrimitives=0;------def 0
r.Shadow.CSM.MaxCascades=4;------def 3------0 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1;------def 0.8------changed to 1*
r.Shadow.CSMDepthBias=10;------def 10
r.Shadow.DistanceScale=0.6;------def 0.85------changed to 0.6*
r.Shadow.FilterMethod=0;------def 0
r.Shadow.MaxCSMResolution=2048;------def 2048------512 or 1024 for PERFORMANCE
r.Shadow.MaxNumFarShadowCascades=0;------def 10------0 for PERFORMANCE
r.Shadow.OcclusionCullCascadedShadowMaps=0;------def 0
r.Shadow.PointLightDepthBias=0.009;------def 0.02 changed to 0.009*
r.Shadow.PointLightSlopeScaleDepthBias=3;------def 3
r.Shadow.RadiusThreshold=0.01;------def 0.04------changed to 0.01*------0.1 or 0.04 for PERFORMANCE
r.Shadow.SpotLightTransitionScale=120;------def 60 changed to 120*
r.Shadow.TransitionScale=120;------def 60 changed to 120*
r.ShadowQuality=3;------def 4------3 for PERFORMANCE
r.SkeletalMeshLODBias=0;------def 0
r.SkeletalMeshLODRadiusScale=1;------def 1
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=1;------def 0------changed to 1*
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=1;------def 0------changed to 1*
r.SkylightIntensityMultiplier=1;------def 1
r.SSGI.Quality=0;------def 2------changed to 0*------0 for PERFORMANCE
r.SSR.HalfResSceneColor=1;------def 1
r.SSR.MaxRoughness=0.1;------def -1------changed to 0.1*
r.SSR.Quality=1;------def 2------changed to 1*------0 for PERFORMANCE
r.SSR.Temporal=0;------def 0
r.SSS.Checkerboard=1;------def 2------changed to 1
r.StaticMeshLODDistanceScale=0.75;------def 1------changed to 0.75*
r.Streaming.MipBias=0;------def 0------1 for PERFORMANCE
r.Streaming.PoolSize.VRAMPercentageClamp=1024;------def 1024
r.Streaming.PoolSize=1000;------def 800------changed to 1000*
r.Streaming.PoolSizeForMeshes=-1;------def -1
r.TessellationAdaptivePixelsPerTriangle=9999999;------def 48------9999999 for PERFORMANCE
r.TextureStreaming=1;------def 1
r.TiledDeferredShading=1;------def 1------0 for PERFORMANCE
r.Tonemapper.EmulateHDR=0;
r.Tonemapper.GrainQuantization=1;------def 1 0 for PERFORMANCE
r.Tonemapper.Quality=5;------def 5
r.Tonemapper.Sharpen=0;------def 1------changed to 0*
r.TonemapperGamma=0;
r.TranslucencyLightingVolume=1;------def 1------0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32;------def 48------32 for PERFORMANCE
r.UITextureLODBias=0;------def 0
r.UniformBufferPooling=1;------def 1
r.Upscale.Quality=0;------def 2------changed to 0*
r.UseClusteredDeferredShading=0;------def 0
r.UseFastIntersect=1;------def 1
r.UseParallelGetDynamicMeshElementsTasks=0;------def 0
r.ViewDistanceScale.ApplySecondaryScale=0;------def 0
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0;------def 0
r.ViewDistanceScale.FieldOfViewMaxAngle=90;------def 90
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1;------def 1
r.ViewDistanceScale.FieldOfViewMinAngle=45;------def 45
r.ViewDistanceScale.FieldOfViewMinAngleScale=1;------def 1
r.ViewDistanceScale.SecondaryScale=1;------def 1
r.ViewDistanceScale=1;------def 1------0.8 for PERFORMANCE
r.VolumetricCloud.ShadowMap=0;------def 1------changed to 0*
r.VolumetricCloud.SkyAO=0;------def 1------changed to 0*
r.VolumetricFog.GridPixelSize=32;------def 16------changed to 32*
r.VolumetricFog.HistoryMissSupersampleCount=1;------def 4------changed to 1*------0 for PERFORMANCE
r.VolumetricFog.InjectShadowedLightsSeparately=0;------def 1------0 for PERFORMANCE
r.VolumetricFog=1;------def 1------0 for PERFORMANCE
r.VSync=0;
r.Vulkan.Depth24Bit=0;------def 0
r.Water.EnableShallowWaterSimulation=0;------def 1------changed to 0*------0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=0;------def 1------changed to 0*------0 for PERFORMANCE
r.Water.ShallowWaterRenderTargetSize=512;------def 1024------changed to 512*
r.Water.SingleLayer.Reflection=1;------def 1------0 for PERFORMANCE
r.Water.SingleLayer.RefractionDownsampleFactor=4;------def 2------4 for PERFORMANCE
r.Water.SingleLayer.SSR=1;------def 1------0 for PERFORMANCE
r.Water.SingleLayer.SSRTAA=0;------def 1------changed to 0*
r.Water.SingleLayer.TiledComposite=1;------def 1
RHI.SyncInterval=0;------def 1------changed to 0*
RHI.SyncSlackMS=0;------def 10------changed to 0*
```

---

#### AA settings i use copy paste over or experiment

```python
TAA
r.DefaultFeature.AntiAliasing=2;------def 2------1 FXAA 2 TAA 3 MSAA 0 OFF
r.PostProcessAAQuality=3;------def 3------1/2 FXAA 3/4/5/6 TAA 0 OFF
r.ScreenPercentage=100;------def 100 TAAU INPUT RESOLUTION

TAAU for PERFORMANCE
r.DefaultFeature.AntiAliasing=2;------def 2------1 FXAA 2 TAA 3 MSAA 0 OFF
r.PostProcessAAQuality=3;------def 3------1/2 FXAA 3/4/5/6 TAA 0 OFF
r.ScreenPercentage=86.66;------def 100 TAAU INPUT RESOLUTION

FXAA
r.DefaultFeature.AntiAliasing=1;------def 2------1 FXAA 2 TAA 3 MSAA 0 OFF
r.PostProcessAAQuality=2;------def 3------1/2 FXAA 3/4/5/6 TAA 0 OFF
r.ScreenPercentage=100;------def 100 TAAU INPUT RESOLUTION

NONE
r.DefaultFeature.AntiAliasing=0;------def 2------1 FXAA 2 TAA 3 MSAA 0 OFF
r.PostProcessAAQuality=0;------def 3------1/2 FXAA 3/4/5/6 TAA 0 OFF
r.ScreenPercentage=100;------def 100 TAAU INPUT RESOLUTION
```

---

<details><summary>Open Input.ini and edit input commands or add them</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Input.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Input.ini
</p>
</details>

```python
[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bF11TogglesFullscreen=0; 
bEnableMouseSmoothing=0;
bViewAccelerationEnabled=0;
InitialButtonRepeatDelay=0.2;------def 0.2
ButtonRepeatDelay=0.1;------def 0.1
DoubleClickTime=0.1;------def 0.25
```

---

<details><summary>Open GameUserSettings.ini these commands will overwrite your config so make sure they are correct also set your scalability groups 0 low 1 med  2 high 3 epic 4 cinematic</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/GameUserSettings.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/GameUserSettings.ini
</p>
</details>

```python
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
DFAO=
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
```

---

<details><summary>Open DeviceProfiles.ini and textures lods experiment for performance</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
</p>
</details>

```python
(wip)
```

---

#### in nvidia control panel

##### 1. 3D settings -> adjust image settings with preview -> use my preference emphasizing performance apply.

##### 2. click on use the advanced 3D image settings and apply then click "take me there"

##### 3. Anisotropic filtering:  Off for performance App-controlled or force your own setting for quality (8x is nice)

##### 4. Low latency mode:

###### Off and ~85% gpu usage for most med-lower end systems (assuming you cap fps correctly)

###### On feels consistent (i use this and reflex in games that support it)

###### Ultra and relfex (in-game) feels good when gpu usage is ~97%

##### 5. Power management mode:  Prefer max performance  (this is the "+ boost" in reflex + boost)

##### 6. Preferred refresh rate:  Highest available

##### 7. Texture filtering - anisotropic sample optimization:  on  (off will look better if this even works)

##### 8. Texture filtering - Negative LOD bias:  Allow

##### 9. Texture filtering quality:  High performance

#####  10. Vertical sync:  Off

<details><summary>11. Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method) click for how to</summary>
<p>
1. NVCleanstall enabling it in advanced settings before installing or
<br>
2. use Wtools enable it and restart or
<br>
3. find ID: open device manager right click your GPU properties and click on events tab
<br>
looks like this:
<br>
HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Enum\PCI\VEN_10DE&DEV_1E84&SUBSYS_139E10DE&REV_A1\4&3aaa5e18&0&0008\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties
<br>
find in regedit and set MSISupported to 1 then restart
</p>
</details>
