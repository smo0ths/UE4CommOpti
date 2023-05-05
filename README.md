
#### updated 5/4/2023 x3 :ramen:

###### for UE4 games for reference/customization/optimization/learning

###### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

###### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

###### def is pretty much reference to high scalablity group

###### Use Nvidia Image Scaling and turn down in game res for more fps (Enabled dlss quality with this for even more fps)

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
MaxChannels=32;
CommonAudioPoolSize=0;
UnfocusedVolumeMultiplier=1;
UseAudioThread=1;
EnableAudioMixer=0;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=64; ⚫️DEF 70 🟢texturepool cache 🟣TEST ⚪️EDITED

[ConsoleVariables]
a.ParallelBlendPhysics=1; ⚫️DEF 1
au.RenderThreadPriority=3; ⚫️DEF 0 or 3 who knows ⚪️EDITED 🟣TEST
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 🟣TEST ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE
foliage.MinLOD=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AllowCachedOverlaps=1; ⚫️DEF 1
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
p.BatchPhysXTasksSize=3; ⚫️DEF 3 🟣TEST
p.Cloth.MaxDeltaTimeTeleportMultiplier=1.5; ⚫️DEF 1.5
p.ClothPhysics.UseTaskThread=1; ⚫️DEF 1
p.ClothPhysics.WaitForParallelClothTask=0; ⚫️DEF 0
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED 🟣TEST
r.AllowDownsampledStandardTranslucency=0; ⚫️DEF 0 🟣TEST
r.AllowLandscapeShadows=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowPointLightCubemapShadows=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AllowSimpleLights=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionMipLevelFactor=1; ⚫️DEF 0.6 ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.Bloom.HalfResolutionFFT=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CookOutUnusedDetailModeComponents=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟣TEST
r.D3D11.UseAllowTearing=0; ⚫️DEF 0
r.D3D12.UseAllowTearing=0; ⚫️DEF 0
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED 🟣TEST
r.DefaultFeature.AmbientOcclusion=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultFeature.AmbientOcclusionStaticFraction=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DefaultFeature.AntiAliasing=2; 🟢1 FXAA 2 TAA 3 MSAA 0 OFF ⚪️EDITED
r.DeferSkeletalDynamicDataUpdateUntilGDME=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DepthOfFieldQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DFDistanceScale=1; ⚫️DEF 1
r.DFFullResolution=0; ⚫️DEF 0
r.DFShadowQuality=2; ⚫️DEF 2
r.DFShadowScatterTileCulling=1; ⚫️DEF 1
r.DFTwoSidedMeshDistanceBias=5; ⚫️DEF 5
r.DiscardUnusedQuality=0; ⚫️DEF 0 🟣TEST
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟣TEST
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟣TEST
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 for PERFORMANCE ⚪️EDITED
r.EnableAsyncComputeVolumetricFog=1; ⚫️DEF ❓ 🟣TEST
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.FreeSkeletalMeshBuffers=0; ⚫️DEF 0 🟣TEST
r.FullScreenMode=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟣TEST
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟢1 for DFSHADOWS DFAO 🟣TEST
r.GeometryCollectionTripleBufferUploads=1; ⚫️DEF 1
r.GPUCrash.CollectionEnable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=0; ⚫️DEF 0 🟣TEST
r.GTSyncType=1; ⚫️DEF 1 🟢1 for DX12 🟣TEST
r.HZBOcclusion=1; ⚫️DEF ❓ 🟣TEST
r.IrisNormal=0; ⚫️DEF 0 🟣TEST
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1
r.LandscapeLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.LightShaftDownSampleFactor=1; ⚫️DEF 2 🟢2 for PERFORMANCE ⚪️EDITED
r.LightShaftQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.LightShaftRenderToSeparateTranslucency=0; ⚫️DEF 0
r.LUT.Size=31; ⚫️DEF 32 🟣TEST
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaxAnisotropy=8; ⚫️DEF 4 ⚪️EDITED
r.MinScreenRadiusForLights=0.03; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.MSAACount=0; ⚫️DEF 4 ⚪️EDITED
r.NormalMapsForStaticLighting=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.OcclusionCullParallelPrimFetch=1; ⚫️DEF 0 ⚪️EDITED 🟣TEST
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RayTracing=0; ⚫️DEF 0
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.RefractionQuality=2; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.RHICmdAsyncRHIThreadDispatch=1; ⚫️DEF 1 🟣TEST 🔴experimental
r.RHICmdBypass=0; ⚫️DEF 0
r.RHICmdUseDeferredContexts=1; ⚫️DEF 1
r.RHICmdUseParallelAlgorithms=1; ⚫️DEF 1
r.SceneColorFormat=3; ⚫️DEF 3 🟣TEST
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.ScreenPercentage=70; ⚫️DEF 100 🟢60 70 80 for PERFORMANCE ⚪️EDITED 🟣TEST
r.SecondaryScreenPercentage.GameViewport=0; ⚫️DEF 0 🟢83.33 for PERFORMANCE 🟣TEST
r.SeparateTranslucency=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Shadow.CachedShadowsCastFromMovablePrimitives=1; ⚫️DEF 1 🟢0 for PERFORMANCE 🟣TEST
r.Shadow.CSM.MaxCascades=2; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE ⚪️EDITED
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=1.1; ⚫️DEF 0.85 🟢0.85 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxCSMResolution=4096; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=2048; ⚫️DEF 2048 🟢1024 for PERFORMANCE
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=0; ⚫️DEF 0 🟢1 for PERFORMANCE
r.SSGI.Quality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Quality=2; ⚫️DEF 2 🟢0 for PERFORMANCE
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=5; ⚫️DEF 0 🟢5 for PERFORMANCE ⚪️EDITED
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🟣TEST 🔴experimental
r.TemporalAA.Upsampling=1; ⚫️DEF 1 🟣TEST
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED 🟣TEST
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED 🟣TEST
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=3; ⚫️DEF 5 🟢0 for PERFORMANCE ⚪️EDITED
r.TranslucencyLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewMaxAngle=90; ⚫️DEF 90 🟣TEST
r.ViewDistanceScale.FieldOfViewMaxAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngle=45; ⚫️DEF 45 🟣TEST
r.ViewDistanceScale.FieldOfViewMinAngleScale=1; ⚫️DEF 1 🟣TEST
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.GridPixelSize=32; ⚫️DEF 16 ⚪️EDITED
r.VolumetricFog.HistoryMissSupersampleCount=1; ⚫️DEF 4 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
rhi.SyncInterval=0; ⚫️DEF 1 ⚪️EDITED
rhi.SyncSlackMS=0; ⚫️DEF 10 ⚪️EDITED
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

<details><summary>Open GameUserSettings.ini these commands will overwrite your config so make sure they are correct also set your scalability groups 0 low 1 med  2 high 3 epic 4 cinematic, check for new stuff after updates</summary>
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
ScreenPercentage=(Value=69)
TextureStreamPoolSizeStorage=(Value=)
MaxAnisotropy=(Value=)
FoliageMinLOD=(Value=)
HZBOcclusion=(Value=)
ContactShadows=(Value=)
DetailMode=(Value=)
AudioQualityLevel=3
MaxAnisotropy=8
bUseVSync=0
GlobalSensitivity=0.183
MaxFPS=
FrameRateLimit=
MenuFrameRateLimit=
HDRDisplayOutputNits=
DoubleKeyPressTime=0.1
DistanceFieldShadows=1;
Gamma=2.2
TAASampleStorage=4
bRTXEnabled=0
bRTXReflectionsEnabled=0
bRTXShadowsEnabled=0
bRTXAmbientOcclusionEnabled=0
DlssQualitySetting=
ResolutionScaleModifier=
DFAO=
Tessellation=(Value=)
TessellationMode=(Value=)
bTelemetryEnabled=0
bUseDynamicResolution=0
FullscreenMode=0
PreferredFullscreenMode=0
ContactShadows=0
PostFX_Saturation=1.2
PostFX_Sharpness=0
OverrideOptions=(("r.PlaceHolder1", (Value=0,bModified=True)),("r.PlaceHolder2", (Value=1,bModified=False)));------works like engineini but in gameusersettingsini
OverrideOptions=(("r.Streaming.PoolSize", (Value=69,bModified=True)));------another example

[ScalabilityGroups]
sg.ResolutionQuality=100
sg.ViewDistanceQuality=2
sg.AntiAliasingQuality=2
sg.PostProcessQuality=2
sg.ShadowQuality=2
sg.TextureQuality=2
sg.EffectsQuality=2
sg.FoliageQuality=2
sg.ShadingQuality=2
sg.AnimationQuality=2
```

---

<details><summary>Open DeviceProfiles.ini and textures lods, skip this and just use the games texture settings imo</summary>
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
[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Cinematic,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=linear,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=1,MaxLODSize=1024,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_NoMipmaps)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=3)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_MobileFlattened,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,MinLODSize=1,MaxLODSize=4096,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,MinLODSize=1,MaxLODSize=4096,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Bokeh,MinLODSize=1,MaxLODSize=256,OptionalMaxLODSize=128,OptionalLODBias=1,MaxLODSize_Smaller=128,MaxLODSize_Smallest=64,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=linear,MipFilter=linear)
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=point,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Impostor,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_ImpostorNormalDepth,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_HierarchicalLOD,MinLODSize=1,MaxLODSize=4096,OptionalMaxLODSize=1024,OptionalLODBias=1,MaxLODSize_Smaller=512,MaxLODSize_Smallest=256,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project01,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,HighPriorityLoad=true)
TextureLODGroups=(Group=TEXTUREGROUP_Project02,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project03,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project04,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point,MipGenSettings=TMGS_NoMipmaps)
TextureLODGroups=(Group=TEXTUREGROUP_Project05,MinLODSize=1,MaxLODSize=512,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=0,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project06,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=1,LODBias_Smaller=1,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project07,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project08,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project09,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project10,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project11,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project12,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
TextureLODGroups=(Group=TEXTUREGROUP_Project13,MinLODSize=1,MaxLODSize=512,OptionalMaxLODSize=256,OptionalLODBias=1,MaxLODSize_Smaller=256,MaxLODSize_Smallest=128,LODBias=0,LODBias_Smaller=0,LODBias_Smallest=1,MinMagFilter=aniso,MipFilter=point)
```

---

#### in nvidia control panel

##### 1. 3D settings -> adjust image settings with preview -> use my preference emphasizing performance apply.

##### 2. click on use the advanced 3D image settings and apply then click "take me there"

##### 3. Anisotropic filtering:  set Application-controlled (you can force the setting in here if you can't notice it working in certain games)

##### 4. Antialiasing - mode: set Application-controlled

##### 5. Low latency mode (Only works with dx11 and lower api):

###### Off and ~85% gpu usage for multiple frame buffers sacrificing latency (cap fps til gpu usage is ~85%) (for visual fluidity of frames)

###### On forces 1 frame buffer (for lower latency than off) (for visual fluidity of frames)

###### Ultra and/or nvidia relfex (in-game dx12 only) and ~97% gpu usage for lowest latency (could be less fluid frames at low fps)

##### 6. Power management mode:  prefer max performance  (this is the "+ boost" in reflex + boost)

##### 7. Preferred refresh rate:  Highest available

##### 8. Texture filtering - anisotropic sample optimization:  on  (off will look better if this even works in your game) (you may need to reapply because NVCP will reset when you change other settings)

##### 9. Texture filtering - negative LOD bias:  allow (allows -1,-2 ect bias) clamp (0 mipmap bias) + integers give more performance at cost of bland textures, most game devs make their HQ textures with a -1 clamp so might want to just leave this on allow and change textures in game (you may need to re-apply because NVCP will reset when you change other settings)

##### 10. Texture filtering quality:  high performance

##### 11. Texture filtering - trilinear optimization:  on

#####  12. Vertical sync:  Off

#####  13. Display -> Adjust desktop size and position -> set no scaling and Perform scaling on: Display

<details><summary>14. Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method) click for how to</summary>
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
