#### updated 10/11/2023 🍝 :ramen:

##### for UE4 games for reference/customization/optimization/learning

##### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

##### my config is trying to be quality and perform well for any UE4 game, it might not be perfectly optimal for a specific game

##### def is reference to high scalablity group

##### use upscaling methods!

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
MaxChannels=128;
CommonAudioPoolSize=0;

[/Script/Engine.Engine]
bSmoothFrameRate=0;
bPauseOnLossOfFocus=0;
bUseFixedFrameRate=0;
DisplayGamma=2.2;

[TextureStreaming]
PoolSizeVRAMPercentage=50; ⚫️DEF 70 🟢texturepool cache ⚪️EDITED

[ConsoleVariables]
sg.ViewDistanceQuality=2;
sg.PostProcessQuality=2;
sg.ShadowQuality=2;
sg.TextureQuality=2;
sg.EffectsQuality=2;
sg.FoliageQuality=2;
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=1; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10; ⚫️DEF 30 ⚪️EDITED
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED
r.DFShadowQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED
r.LandscapeLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.MinScreenRadiusForLights=0.04; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.75; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Burley.BilateralFilterKernelFunctionType=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟢2500 for PERFORMANCE ⚪️EDITED
r.Streaming.PoolSize=1200; ⚫️DEF 2000 ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.Upscale.Quality=0; ⚫️DEF 2 ⚪️EDITED
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4; ⚫️DEF 4 🟢0 for PERFORMANCE
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldGI=0; ⚫️DEF ❓
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🔴experimental
r.EarlyZPass=2; ⚫️DEF ❓
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED
r.HZBOcclusion=0; ⚫️DEF ❓
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.NormalMapsForStaticLighting=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req some light shadows
r.SupportSkyAtmosphereAffectsHeightFog=0; ⚫️DEF ❓
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0 🟡for ScreenPercentage
r.VolumetricFog.LightFunctionSupersampleScale=1; ⚫️DEF ❓ ⚪️EDITED
```

---

<details><summary>Now the fun part open up Scalability.ini and add the config to the scalability groups eg [EffectsQuality@2] i'm not going threw all the commands and putting them perfectly into place this is the brute force method :D</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/Scalability.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/Scalability.ini
</p>
</details>

```python
[AntiAliasingQuality@2]
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=1; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10; ⚫️DEF 30 ⚪️EDITED
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED
r.DFShadowQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED
r.LandscapeLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.MinScreenRadiusForLights=0.04; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.75; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Burley.BilateralFilterKernelFunctionType=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟢2500 for PERFORMANCE ⚪️EDITED
r.Streaming.PoolSize=1200; ⚫️DEF 2000 ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.Upscale.Quality=0; ⚫️DEF 2 ⚪️EDITED
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4; ⚫️DEF 4 🟢0 for PERFORMANCE
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldGI=0; ⚫️DEF ❓
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🔴experimental
r.EarlyZPass=2; ⚫️DEF ❓
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED
r.HZBOcclusion=0; ⚫️DEF ❓
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.NormalMapsForStaticLighting=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req some light shadows
r.SupportSkyAtmosphereAffectsHeightFog=0; ⚫️DEF ❓
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0 🟡for ScreenPercentage
r.VolumetricFog.LightFunctionSupersampleScale=1; ⚫️DEF ❓ ⚪️EDITED

[ViewDistanceQuality@2]
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=1; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10; ⚫️DEF 30 ⚪️EDITED
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED
r.DFShadowQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED
r.LandscapeLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.MinScreenRadiusForLights=0.04; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.75; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Burley.BilateralFilterKernelFunctionType=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟢2500 for PERFORMANCE ⚪️EDITED
r.Streaming.PoolSize=1200; ⚫️DEF 2000 ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.Upscale.Quality=0; ⚫️DEF 2 ⚪️EDITED
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4; ⚫️DEF 4 🟢0 for PERFORMANCE
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldGI=0; ⚫️DEF ❓
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🔴experimental
r.EarlyZPass=2; ⚫️DEF ❓
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED
r.HZBOcclusion=0; ⚫️DEF ❓
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.NormalMapsForStaticLighting=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req some light shadows
r.SupportSkyAtmosphereAffectsHeightFog=0; ⚫️DEF ❓
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0 🟡for ScreenPercentage
r.VolumetricFog.LightFunctionSupersampleScale=1; ⚫️DEF ❓ ⚪️EDITED

[PostProcessQuality@2]
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=1; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10; ⚫️DEF 30 ⚪️EDITED
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED
r.DFShadowQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED
r.LandscapeLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.MinScreenRadiusForLights=0.04; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.75; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Burley.BilateralFilterKernelFunctionType=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟢2500 for PERFORMANCE ⚪️EDITED
r.Streaming.PoolSize=1200; ⚫️DEF 2000 ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.Upscale.Quality=0; ⚫️DEF 2 ⚪️EDITED
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4; ⚫️DEF 4 🟢0 for PERFORMANCE
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldGI=0; ⚫️DEF ❓
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🔴experimental
r.EarlyZPass=2; ⚫️DEF ❓
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED
r.HZBOcclusion=0; ⚫️DEF ❓
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.NormalMapsForStaticLighting=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req some light shadows
r.SupportSkyAtmosphereAffectsHeightFog=0; ⚫️DEF ❓
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0 🟡for ScreenPercentage
r.VolumetricFog.LightFunctionSupersampleScale=1; ⚫️DEF ❓ ⚪️EDITED

[TextureQuality@2]
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=1; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10; ⚫️DEF 30 ⚪️EDITED
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED
r.DFShadowQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED
r.LandscapeLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.MinScreenRadiusForLights=0.04; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.75; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Burley.BilateralFilterKernelFunctionType=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟢2500 for PERFORMANCE ⚪️EDITED
r.Streaming.PoolSize=1200; ⚫️DEF 2000 ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.Upscale.Quality=0; ⚫️DEF 2 ⚪️EDITED
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4; ⚫️DEF 4 🟢0 for PERFORMANCE
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldGI=0; ⚫️DEF ❓
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🔴experimental
r.EarlyZPass=2; ⚫️DEF ❓
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED
r.HZBOcclusion=0; ⚫️DEF ❓
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.NormalMapsForStaticLighting=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req some light shadows
r.SupportSkyAtmosphereAffectsHeightFog=0; ⚫️DEF ❓
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0 🟡for ScreenPercentage
r.VolumetricFog.LightFunctionSupersampleScale=1; ⚫️DEF ❓ ⚪️EDITED

[EffectsQuality@2]
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=1; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10; ⚫️DEF 30 ⚪️EDITED
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED
r.DFShadowQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED
r.LandscapeLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.MinScreenRadiusForLights=0.04; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.75; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Burley.BilateralFilterKernelFunctionType=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟢2500 for PERFORMANCE ⚪️EDITED
r.Streaming.PoolSize=1200; ⚫️DEF 2000 ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.Upscale.Quality=0; ⚫️DEF 2 ⚪️EDITED
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4; ⚫️DEF 4 🟢0 for PERFORMANCE
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldGI=0; ⚫️DEF ❓
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🔴experimental
r.EarlyZPass=2; ⚫️DEF ❓
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED
r.HZBOcclusion=0; ⚫️DEF ❓
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.NormalMapsForStaticLighting=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req some light shadows
r.SupportSkyAtmosphereAffectsHeightFog=0; ⚫️DEF ❓
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0 🟡for ScreenPercentage
r.VolumetricFog.LightFunctionSupersampleScale=1; ⚫️DEF ❓ ⚪️EDITED

[FoliageQuality@2]
D3D12.AdjustTexturePoolSizeBasedOnBudget=1; ⚫️DEF 0 ⚪️EDITED
foliage.DensityScale=0.6; ⚫️DEF 0.8 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
foliage.LODDistanceScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
foliage.MinLOD=0; ⚫️DEF 0 🟢1 2 or 3 for PERFORMANCE ⚪️EDITED
FX.MaxCPUParticlesPerEmitter=1; ⚫️DEF 1000 ⚪️EDITED
FX.MaxGPUParticlesSpawnedPerFrame=20972; ⚫️DEF 1048576 ⚪️EDITED
grass.DensityScale=0.6; ⚫️DEF 1 🟢0.6 for PERFORMANCE ⚪️EDITED
grass.DisableDynamicShadows=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.DiscardDataOnLoad=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
grass.MaxUpdateFrequency=10; ⚫️DEF 30 ⚪️EDITED
grass.TickInterval=10; ⚫️DEF 1 🟢10 for PERFORMANCE ⚪️EDITED
p.AnimDynamics=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.RigidBodyNode=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AllowDownsampledStandardTranslucency=1; ⚫️DEF 0 ⚪️EDITED
r.AllowLandscapeShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AlsoUseSphereForFrustumCull=1; ⚫️DEF 0 ⚪️EDITED
r.AmbientOcclusionLevels=2; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED
r.AmbientOcclusionStaticFraction=1; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.AnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.AOViewFadeDistanceScale=0.1; ⚫️DEF 0.7 ⚪️EDITED
r.CapsuleShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.CompileShadersForDevelopment=0; ⚫️DEF 1 ⚪️EDITED
r.ContactShadows=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.DefaultBackBufferPixelFormat=0; ⚫️DEF 4 ⚪️EDITED
r.DepthOfFieldQuality=0; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.DFDistanceScale=0.3; ⚫️DEF 1 🟢0.3 for PERFORMANCE ⚪️EDITED
r.DFShadowQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.DFTwoSidedMeshDistanceBias=1; ⚫️DEF 5 ⚪️EDITED
r.DistanceFields.ForceMaxAtlasSize=1; ⚫️DEF 0 ⚪️EDITED
r.DistanceFields.RuntimeDownsamplingFactor=0.5; ⚫️DEF 0 ⚪️EDITED
r.DOF.TemporalAAQuality=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.EmitterSpawnRateScale=0.5; ⚫️DEF 1 🟢0.125 or 0.5 PERFORMANCE ⚪️EDITED
r.EyeAdaptationQuality=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.gpucrash.collectionenable=0; ⚫️DEF 1 ⚪️EDITED
r.GPUSkin.Limit2BoneInfluences=1; ⚫️DEF 0 ⚪️EDITED
r.LandscapeLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.LightShaftAllowTAA=0; ⚫️DEF 1 ⚪️EDITED
r.MinScreenRadiusForLights=0.04; ⚫️DEF 0.03 🟢0.06 for PERFORMANCE ⚪️EDITED
r.MinTimeBetweenTicks=12; ⚫️DEF 8 or 16 ⚪️EDITED
r.MipMapLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.MotionBlurQuality=0; ⚫️DEF 3 ⚪️EDITED
r.PostProcessAAQuality=5; 🟢1 or 2 FXAA 3 or 4 5 6 TAA 0 OFF ⚪️EDITED
r.RefractionQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SceneColorFringeQuality=0; ⚫️DEF 1 ⚪️EDITED
r.Shadow.CSM.MaxCascades=3; ⚫️DEF 3 🟢1 or 2 for PERFORMANCE
r.Shadow.CSM.TransitionScale=1; ⚫️DEF 0.8 ⚪️EDITED
r.Shadow.DistanceScale=0.75; ⚫️DEF 0.85 ⚪️EDITED
r.Shadow.MaxCSMResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.MaxResolution=1024; ⚫️DEF 2048 🟢1024 for PERFORMANCE ⚪️EDITED
r.Shadow.RadiusThreshold=0.03; ⚫️DEF 0.04 🟢0.08 for PERFORMANCE ⚪️EDITED
r.ShadowQuality=3; ⚫️DEF 4 🟢3 for PERFORMANCE ⚪️EDITED
r.SkeletalMeshLODBias=1; ⚫️DEF 0 🟢1 for PERFORMANCE ⚪️EDITED
r.SSR.MaxRoughness=0.7; ⚫️DEF -1 ⚪️EDITED
r.SSR.Quality=1; ⚫️DEF 2 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Burley.BilateralFilterKernelFunctionType=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.Checkerboard=1; ⚫️DEF 2 🟢1 for PERFORMANCE ⚪️EDITED
r.SSS.Quality=0; ⚫️DEF -1 🟢0 for PERFORMANCE ⚪️EDITED
r.SSS.SampleSet=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Streaming.AmortizeCPUToGPUCopy=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxEffectiveScreenSize=0; ⚫️DEF 1 ⚪️EDITED
r.Streaming.MaxNumTexturesToStreamPerFrame=1; ⚫️DEF 0 ⚪️EDITED
r.Streaming.MaxTextureUVDensity=2500; ⚫️DEF 0 🟢2500 for PERFORMANCE ⚪️EDITED
r.Streaming.PoolSize=1200; ⚫️DEF 2000 ⚪️EDITED
r.SupportAnisotropicMaterials=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.SupportMaterialLayers=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAA.Algorithm=1; ⚫️DEF 0 🟢0 for PERFORMANCE ⚪️EDITED
r.TemporalAACurrentFrameWeight=0.03; ⚫️DEF 0.05 ⚪️EDITED
r.TemporalAAFilterSize=0.1; ⚫️DEF 1 ⚪️EDITED
r.TemporalAASamples=2; ⚫️DEF 8 ⚪️EDITED
r.TessellationAdaptivePixelsPerTriangle=9999999; ⚫️DEF 48 🟢9999999 for PERFORMANCE ⚪️EDITED
r.Tonemapper.Sharpen=0; ⚫️DEF 2 ⚪️EDITED
r.TonemapperGamma=2.2; ⚫️DEF 0 ⚪️EDITED
r.TranslucencyLightingVolumeDim=32; ⚫️DEF 48 🟢32 for PERFORMANCE ⚪️EDITED
r.Upscale.Quality=0; ⚫️DEF 2 ⚪️EDITED
r.ViewDistanceScale=0.8; ⚫️DEF 1 🟢0.8 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.ShadowMap=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud.SkyAO=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricCloud=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.InjectShadowedLightsSeparately=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.VolumetricFog.TemporalReprojection=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.EnableShallowWaterSimulation=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSR=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
r.Water.SingleLayer.SSRTAA=0; ⚫️DEF 1 🟢0 for PERFORMANCE ⚪️EDITED
p.ClothPhysics=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Bloom.Cross=0; ⚫️DEF 0 🟢0.7777 for anamorphic
r.BloomQuality=4; ⚫️DEF 4 🟢0 for PERFORMANCE
r.DBuffer=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.DetailMode=2; ⚫️DEF 2 🟢1 or 0 for PERFORMANCE
r.DoTiledReflections=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.GBufferFormat=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LandscapeLOD0DistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LandscapeLODDistributionScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.LensFlareQuality=1; ⚫️DEF 2 🟢0 for PERFORMANCE
r.LightFunctionQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.LightMaxDrawDistanceScale=1; ⚫️DEF 1 🟢0.6 for PERFORMANCE
r.LightShaftQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.MaterialQualityLevel=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ParticleLightQuality=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ReflectionEnvironment=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SeparateTranslucency=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SSGI.Enable=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.SSR.HalfResSceneColor=1; ⚫️DEF 1 🟢1 for PERFORMANCE
r.SSR.Temporal=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.StaticMeshLODDistanceScale=1; ⚫️DEF 1 🟢test for PERFORMANCE
r.SubsurfaceScattering=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.SupportAtmosphericFog=0; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TiledDeferredShading=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.GrainQuantization=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Tonemapper.Quality=5; ⚫️DEF 5 🟢0 for PERFORMANCE
r.TranslucencyVolumeBlur=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.TranslucentLightingVolume=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.ViewDistanceScale.FieldOfViewAffectsHLOD=0; ⚫️DEF 0 🟢0 for PERFORMANCE
r.VolumetricFog=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.EnableUnderwaterPostProcess=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.Water.SingleLayer.Reflection=1; ⚫️DEF 1 🟢0 for PERFORMANCE
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AOHeightfieldOcclusion=0; ⚫️DEF ❓
r.AOQuality=2; ⚫️DEF ❓ 🟢1 for PERFORMANCE
r.DistanceFieldAO=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldGI=0; ⚫️DEF ❓
r.DistanceFieldShadowing=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.DoInitViewsLightingAfterPrepass=0; ⚫️DEF 0 🔴experimental
r.DoLazyStaticMeshUpdate=0; ⚫️DEF 0 🔴experimental
r.EarlyZPass=2; ⚫️DEF ❓
r.EarlyZPassOnlyMaterialMasking=1; ⚫️DEF ❓
r.FinishCurrentFrame=0; ⚫️DEF 0 🟢0 for PERFORMANCE 🔵1 for best latency
r.GenerateLandscapeGIData=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req MeshDF for GI
r.GenerateMeshDistanceFields=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req for DF things ⚪️EDITED
r.HZBOcclusion=0; ⚫️DEF ❓
r.MaxAnisotropy=8; ⚫️DEF ❓ ⚪️EDITED
r.NormalMapsForStaticLighting=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE
r.Shadow.CachedShadowsCastFromMovablePrimitives=0; ⚫️DEF ❓ 🟢0 for PERFORMANCE 🟡req some light shadows
r.SupportSkyAtmosphereAffectsHeightFog=0; ⚫️DEF ❓
r.TemporalAA.R11G11B10History=0; ⚫️DEF 0 🔴experimental
r.TemporalAA.Upsampling=0; ⚫️DEF 0 🟡for ScreenPercentage
r.VolumetricFog.LightFunctionSupersampleScale=1; ⚫️DEF ❓ ⚪️EDITED
```

---

<details><summary>Open GameUserSettings.ini these commands will overwrite your config so make sure they are correct check for new stuff after updates, good luck</summary>
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
bDepthOfField=
bMotionBlur=
bBounceLightEnabled=
bFlashlightShadowsEnabled=
AmbientOcclusion=(Value=1)
AntiAliasingMode=(Value=2)
AudioQualityLevel=3
bRTXAmbientOcclusionEnabled=
bRTXEnabled=
bRTXReflectionsEnabled=
bRTXShadowsEnabled=
bTelemetryEnabled=0
bUseDynamicResolution=0
bUseVSync=0
ContactShadows=(Value=0)
ContactShadows=0
DetailMode=(Value=)
DFAO=
DistanceFieldShadows=1
DlssQualitySetting=
DoubleKeyPressTime=0.1
FoliageMinLOD=(Value=0)
FullscreenMode=0
Gamma=2.2
GlobalSensitivity=0.183
GraphicsQuality=0
GraphicsPresetIndex=0
HDRDisplayOutputNits=
HZBOcclusion=(Value=)
MaxAnisotropy=(Value=)
MaxAnisotropy=8
bFrameLimitEnabled=
FrameRateLimit=
MaxFPS=
MenuFrameRateLimit=
OceanQuality=(Value=0)
OverrideOptions=(("r.9000FPS",(Value=1,bModified=True)),("r.OPTIMIZE",(Value=1,bModified=False)));
PostFX_Saturation=1.2
PostFX_Sharpness=0.25;      <- needed for squid to set tonemappersharp correctly
ResolutionScaleModifier=
ScreenPercentage=(Value=70)
SkeletalMeshLODBias=(Value=0)
TAASampleStorage=2
LastSavedAASamples=2
TemporalAASamples=(Value=2);   <- needed for squid to set to 2
Tessellation=(Value=0)
TessellationMode=(Value=9999999)
TextureStreamPoolSizeStorage=(Value=)
WakeSim=(Value=0)
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
InitialButtonRepeatDelay=0.2; ⚫️DEF 0.2
ButtonRepeatDelay=0.1; ⚫️DEF 0.1
DoubleClickTime=0.1; ⚫️DEF 0.25
```

---

#### AO options

```python
dfao:
r.AmbientOcclusionLevels=0; ⚫️DEF 3 🟢0 for PERFORMANCE ⚪️EDITED
r.DistanceFieldAO=1; ⚫️DEF ❓ 🟢0 for PERFORMANCE ⚪️EDITED

ssao med:
r.AmbientOcclusion.Compute=0; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels
r.AmbientOcclusionRadiusScale=0.3; ⚫️DEF 1 ⚪️EDITED

ssao low:
r.AmbientOcclusion.Compute=1; ⚫️DEF 0 🟢1 for PERFORMANCE 🟡req 0 for AO levels ⚪️EDITED
r.AmbientOcclusionRadiusScale=0.1; ⚫️DEF 1 ⚪️EDITED

or both
```

---

<details><summary>Open DeviceProfiles.ini for textures lods, skip this and just use the games texture settings imo</summary>
<p>
press <kbd>⊞ Win+R</kbd> then copy paste
<br>
%localappdata%/SquadGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/GroundBranch/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/ReadyOrNot/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/SessionGame/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
<br>
%localappdata%/Chivalry 2/Saved/Config/WindowsNoEditor/DeviceProfiles.ini
</p>
</details>

```python
[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Character,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Effects,MinLODSize=128,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,MinLODSize=128,MaxLODSize=1024,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=aniso,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_UI,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,MinLODSize=512,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,MinLODSize=512,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=3,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,MinLODSize=1,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,MinLODSize=256,MaxLODSize=2048,LODBias=0,MinMagFilter=linear,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,MinLODSize=1,MaxLODSize=1024,LODBias=0,MinMagFilter=point,MipFilter=point,NumStreamedMips=-1,MipGenSettings=TMGS_SimpleAverage)
```

---

#### in nvidia control panel (make sure all the settings stuck cause the NVCP is old as shit)

##### 1. 3D settings -> adjust image settings with preview -> use my preference emphasizing performance apply.

##### 2. click on use the advanced 3D image settings and apply then click "take me there"

##### 3. Anisotropic filtering:  set Application-controlled (you can force the setting in here if you can't notice it working in certain games)

##### 4. Low latency mode (Only works with dx11 and lower api):

###### Off and ~85% gpu usage for multiple frame buffers sacrificing latency (cap fps til gpu usage is ~85%) (for visual fluidity of frames)

###### On forces 1 frame buffer (for lower latency than off) (for visual fluidity of frames and less latency)

###### Ultra and high gpu usage for lowest latency

###### Nvidia relfex is in-game and dx12 only and you should use it just like Ultra low latency mode with high gpu usage

##### 5. Power management mode:  prefer max performance  (this is the "+ boost" in reflex + boost)

##### 6. Preferred refresh rate:  Highest available

##### 7. Texture filtering - anisotropic sample optimization:  on  (off will look better if this even works in your game)

##### 8. Texture filtering - negative LOD bias:  allow (allows a negative bias) clamp (0 mipmap bias) test yourself devs usually set slight negative clamps

##### 9. Texture filtering quality:  high performance

##### 10. Texture filtering - trilinear optimization:  on

#####  11. Vertical sync:  Off

#####  12. Display -> Adjust desktop size and position -> set no scaling and Perform scaling on: Display

<details><summary>13. Turn on Message-signaled interrupts (MSIs) (better than line based interrupt method) click for how to</summary>
<p>
1. NVCleanstall enabling it in advanced settings before installing or
<br>
2. use Wtools enable it and restart or
<br>
3. find ID: open device manager right click your GPU properties and click on events tab
<br>
looks like this:
<br>
HKLM\SYSTEM\ControlSet001\Enum\PCI\THESENUMBERSCHANGE\THESENUMBERSCHANGE\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties
<br>
find in regedit and set MSISupported to 1 then restart
<br>
in device manager/view/resorces by connection/GPU name should have a negative number in parentheses if MSIs is enabled
</p>
</details>

#### Disable HPET (High Precision event timer) in device manager/system devices and/or in your bios to get lower latency and more fps
