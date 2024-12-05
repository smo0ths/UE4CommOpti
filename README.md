## updated 12/5/2024 ✂ 📋 🌀 :ramen: v0.201.33

### for UE4 and UE5* games for reference/customization/optimization/learning

#### always testing stuff contact me [smoothschannel](https://twitch.tv/smoothschannel) or [discord](https://discord.gg/tDZT7QSx8m)

#### my config is trying to be quality and perform well for any UE4/5 game, it might not be perfectly optimal for a specific game

#### [Installing and optimizing nvidia drivers here](https://github.com/smo0ths/Installing-and-optimizing-new-nvidia-drivers-on-windows-11-gaming-PC)

#### check 🔴 options for more fps (left to right, performance to quality)

#### 2560x1440 use 🔴 58%,67%,70% for PERFORMANCE (higher when cpu bound) (DLSS/TAAU/TSR/CAS/FSR/XeSS/PSSR/NIS/IS)

#### 3328x1872 use 🔴 50%,58%,67% for PERFORMANCE (higher when cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR/NIS/IS)

#### 3840x2160 use 🔴 33%,50%,67% for PERFORMANCE (higher when cpu bound) (DLSS123/TAAU/TSR/CAS/FSR123/XeSS/PSSR/NIS/IS)

#### negative LOD bias 0,-0.6,-1 for PERFORMANCE (0 is best on proper mipmaps/textures) (set by nvidiaProfileInspector)

## Open Engine.ini and copy pasta %localappdata%

#### or Repak.bat method (zzz_ENGINE_INI\Engine\Config\Windows\WindowsEngine.ini)

#### High config (works with UE5*)

```python
[Core.Log]
Global=off;

[/Script/Engine.Engine]
bPauseOnLossOfFocus=0;
bSmoothFrameRate=0;
bUseFixedFrameRate=0;

[TextureStreaming]
PoolSizeVRAMPercentage=70; 🔴 50 to lower vram usage ⚪ def 70 🔵 texturepool cache

[ConsoleVariables]
D3D12.InsertOuterOcclusionQuery=0; 🔴 1 for PERFORMANCE ⚪ def 0
D3D12.MaximumFrameLatency=1; ⚫ EDITED ⚪ def 3 🔵 frame latency
demo.LoadCheckpointGarbageCollect=0; ⚫ EDITED ⚪ def 1
foliage.DensityScale=0.8; 🔴 0.6,0.8 for PERFORMANCE ⚪ def 1
foliage.MinimumScreenSize=0.0001; ⚫ EDITED ⚪ def 0.000005
fx.EnableCircularAnimTrailDump=0; ⚫ EDITED ⚪ def 2
fx.Niagara.Collision.CPUEnabled=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
fx.Niagara.QualityLevel=2; 🔴 0,1,2 for PERFORMANCE ⚪ def 3
fx.ParticlePerfStats.Enabled=0; ⚫ EDITED ⚪ def 1
grass.DensityScale=0.8; 🔴 0.6,0.8 for PERFORMANCE ⚫ EDITED ⚪ def 1
grass.DisableDynamicShadows=0; 🔴 1 for PERFORMANCE ⚪ def 0
memory.logGenericPlatformMemoryStats=0; ⚫ EDITED ⚪ def 1
p.AnimDynamics=1; 🔴 0 for PERFORMANCE ⚪ def 1
p.AnimDynamicsWind=1; 🔴 0 for PERFORMANCE ⚪ def 1
p.RigidBodyNode=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.AllowLandscapeShadows=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.AllowSimpleLights=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.AmbientOcclusionLevels=-1; 🔴 0,1 for PERFORMANCE ⚪ def -1
r.AmbientOcclusionStaticFraction=-1; 🔴 0 for PERFORMANCE ⚪ def -1
r.AnisotropicMaterials=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.AOGlobalDistanceField.MipFactor=4; 🔴 8 for PERFORMANCE ⚪ def 4
r.AOQuality=2; 🔴 0,1 for PERFORMANCE ⚪ def 2
r.Bloom.ScreenPercentage=50; ⚪ def 50
r.BloomQuality=4; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 5
r.BlurGBuffer=0; ⚫ EDITED ⚪ def -1
r.CapsuleShadows=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.ContactShadows=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.DefaultFeature.MotionBlur=0; ⚫ EDITED ⚪ def 1
r.DepthOfFieldQuality=1; 🔴 0,1 for PERFORMANCE ⚫ EDITED ⚪ def 2
r.DetailMode=2; 🔴 0,1,2 for PERFORMANCE ⚫ EDITED ⚪ def 3
r.DFShadowQuality=1; 🔴 1,2 for PERFORMANCE ⚫ EDITED ⚪ def 3
r.DistanceFields.MaxPerMeshResolution=128; 🔴 128 for PERFORMANCE ⚫ EDITED ⚪ def 256
r.DOF.Gather.AccumulatorQuality=0; ⚫ EDITED ⚪ def 1
r.DOF.Gather.EnableBokehSettings=0; ⚫ EDITED ⚪ def 1
r.DOF.Gather.PostfilterMethod=0; ⚫ EDITED ⚪ def 1
r.DOF.Gather.RingCount=3; ⚫ EDITED ⚪ def 5
r.DOF.Kernel.MaxBackgroundRadius=0.012; ⚫ EDITED ⚪ def 0.025
r.DOF.Kernel.MaxForegroundRadius=0.012; ⚫ EDITED ⚪ def 0.025
r.DOF.Recombine.Quality=0; ⚫ EDITED ⚪ def 2
r.DOF.Scatter.BackgroundCompositing=1; ⚫ EDITED ⚪ def 2
r.DOF.Scatter.EnableBokehSettings=0; ⚫ EDITED ⚪ def 1
r.DOF.Scatter.ForegroundCompositing=1; ⚪ def 1
r.DOF.Scatter.MaxSpriteRatio=0.04; ⚪ def 0.1
r.DynamicRes.FrameTimeBudget=33.3; ⚪ def 33.3 
r.DynamicRes.MinScreenPercentage=50; ⚪ def 50
r.DynamicRes.OperationMode=0; ⚪ def 0
r.DynamicRes.TargetedGPUHeadRoomPercentage=10; ⚪ def 10
r.EmitterSpawnRateScale=1; 🔴 0.125,0.25,0.5 for PERFORMANCE ⚪ def 1
r.EnableDebugSpam_GetObjectPositionAndScale=0; ⚫ EDITED ⚪ def 1 🔵 debug
r.EyeAdaptationQuality=2; 🔴 1 for PERFORMANCE ⚪ def 2 🔵 eyeadaptation,autoexposure
r.FilmGrain=0; ⚫ EDITED ⚪ def 1
r.Filter.SizeScale=1; ⚪ def 1
r.Fog=1; ⚪ def 1 🔵 render fog
r.FXAA.Quality=4; ⚪ def 4
r.GBufferDiffuseSampleOcclusion=1; ⚫ EDITED ⚪ def 0 🔵 bent normal maps
r.gpucrash.collectionenable=0; ⚫ EDITED ⚪ def 1 🔵 debug
r.GTSyncType=2; ⚫ EDITED ⚪ def 0
r.HairStrands.Enable=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.HairStrands.MinLOD=1; 🔴 2 for PERFORMANCE ⚪ def 1
r.HairStrands.SkyAO=0; 🔴 0 for PERFORMANCE ⚪ def 1
r.HairStrands.UseCardsInsteadOfStrands=1; 🔴 1 for PERFORMANCE ⚫ EDITED ⚪ def 0
r.HairStrands.Visibility.MSAA.SamplePerPixel=2; 🔴 2 for PERFORMANCE ⚫ EDITED ⚪ def 4
r.HairStrands.Voxelization=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1 🔵 voxelization
r.HeightFieldShadowing=0; ⚪ def 0 🔵 height field shadowing
r.LandscapeLODBias=0; 🔴 1 for PERFORMANCE ⚪ def 0
r.LensFlareQuality=2; 🔴 1 for PERFORMANCE ⚪ def 2
r.LightMaxDrawDistanceScale=1; 🔴 0.5,0.6 for PERFORMANCE ⚪ def 1
r.LightShaftBlurPasses=2; ⚫ EDITED ⚪ def 3
r.LightShaftFirstPassDistance=0.08; ⚫ EDITED ⚪ def 0.1
r.LightShaftQuality=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.Lumen.DiffuseIndirect.SSAO=0; ⚪ def 0
r.Lumen.RadianceCache.NumFramesToKeepCachedProbes=8; ⚪ def 8
r.Lumen.Reflections.BilateralFilter.NumSamples=4; ⚪ def 4
r.Lumen.Reflections.BilateralFilter.SpatialKernelRadius=0.002; ⚪ def 0.002
r.Lumen.Reflections.DownsampleFactor=1; 🔴 2 for PERFORMANCE ⚪ def 1
r.Lumen.Reflections.MaxRoughnessToTrace=-1; ⚪ def -1
r.Lumen.Reflections.SampleSceneColorAtHit=1; ⚪ def 1
r.Lumen.Reflections.ScreenSpaceReconstruction=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.Lumen.Reflections.ScreenTraces=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.Lumen.Reflections.SmoothBias=0; ⚪ def 0 🔵 override roughness
r.Lumen.Reflections.TraceMeshSDFs=1; ⚪ def 1
r.Lumen.ScreenProbeGather.DownsampleFactor=32; 🔴 32 for PERFORMANCE ⚪ def 16
r.Lumen.ScreenProbeGather.FullResolutionJitterWidth=1; ⚪ def 1
r.Lumen.ScreenProbeGather.IrradianceFormat=1; 🔴 1 for PERFORMANCE ⚪ def 0
r.Lumen.ScreenProbeGather.MaterialAO=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.Lumen.ScreenProbeGather.RadianceCache.GridResolution=48; ⚪ def  48
r.Lumen.ScreenProbeGather.RadianceCache.NumProbesToTraceBudget=300; ⚪ def 300
r.Lumen.ScreenProbeGather.RadianceCache.ProbeAtlasResolutionInProbes=128; ⚪ def 128
r.Lumen.ScreenProbeGather.RadianceCache.ProbeResolution=16; 🔴 16 for PERFORMANCE ⚪ def 32
r.Lumen.ScreenProbeGather.ScreenSpaceBentNormal=1; ⚪ def 1 🔵 bent normal maps
r.Lumen.ScreenProbeGather.ShortRangeAO.ApplyDuringIntegration=0; ⚪ def 0
r.Lumen.ScreenProbeGather.ShortRangeAO.HairScreenTrace=0; ⚪ def 0
r.Lumen.ScreenProbeGather.ShortRangeAO=1; ⚪ def 1 🔵 lumen contact shadows
r.Lumen.ScreenProbeGather.StochasticInterpolation=1; 🔴 1 for PERFORMANCE ⚫ EDITED ⚪ def 0
r.Lumen.ScreenProbeGather.TracingOctahedronResolution=8; ⚪ def 8
r.Lumen.ScreenProbeGather.TwoSidedFoliageBackfaceDiffuse=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.Lumen.ScreenProbeGather=1; ⚪ def 1
r.Lumen.TraceMeshSDFs.TraceDistance=180; ⚪ def 180
r.Lumen.TraceMeshSDFs=0; 🔴 0 for PERFORMANCE ⚪ def 1
r.Lumen.TranslucencyReflections.FrontLayer.Allow=0; 🔴 0 for PERFORMANCE ⚪ def 1
r.Lumen.TranslucencyReflections.FrontLayer.Enable=0; 🔴 0 for PERFORMANCE ⚪ def 0
r.Lumen.TranslucencyReflections.FrontLayer.EnableForProject=0; 🔴 0 for PERFORMANCE ⚪ def 0
r.Lumen.TranslucencyVolume.Enable=1; ⚪ def 1
r.Lumen.TranslucencyVolume.GridPixelSize=64; 🔴 64,32 for PERFORMANCE ⚫ EDITED ⚪ def 32
r.Lumen.TranslucencyVolume.RadianceCache.NumProbesToTraceBudget=200; ⚪ def 200
r.Lumen.TranslucencyVolume.RadianceCache.ProbeResolution=8; ⚪ def 8
r.Lumen.TranslucencyVolume.RadianceCache=1; 🔴 1 for PERFORMANCE ⚪ def 1
r.Lumen.TranslucencyVolume.TraceFromVolume=0; 🔴 0 for PERFORMANCE ⚪ def 1
r.Lumen.TranslucencyVolume.TracingOctahedronResolution=3; ⚪ def 3
r.LumenScene.DirectLighting.OffscreenShadowing.TraceMeshSDFs=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.LumenScene.FarField=0; ⚪ def 0 🔵 extend lumen
r.LumenScene.GlobalSDF.Resolution=252; ⚪ def 252
r.LumenScene.Radiosity.HemisphereProbeResolution=3; 🔴 3 for PERFORMANCE ⚪ def 4
r.LumenScene.Radiosity.ProbeSpacing=8; 🔴 8 for PERFORMANCE ⚪ def 4
r.LumenScene.Radiosity=1 ⚪ def 1
r.LumenScene.SurfaceCache.AtlasSize=1024; 🔴 1024 for PERFORMANCE ⚫ EDITED ⚪ def 4096
r.LumenScene.SurfaceCache.CardCaptureRefreshFraction=0.125; ⚪ def 0.125
r.LumenScene.SurfaceCache.CardMinResolution=4; ⚪ def 4
r.LumenScene.SurfaceCache.FarField.CardDistance=40000; ⚪ def 40000
r.LumenScene.SurfaceCache.MeshCardsMinSize=10; ⚪ def 10
r.LumenScene.SurfaceCache.NaniteMultiView=0; ⚫ EDITED ⚪ def 1
r.MaterialQualityLevel=1; 🔴 0,2 for PERFORMANCE ⚪ def 1
r.MaxAnisotropy=8; 🔴 0,4 for PERFORMANCE ⚪ def 8
r.MinScreenRadiusForLights=0.03; 🔴 0.06,0.04 for PERFORMANCE ⚪ def 0.03
r.MipMapLODBias=0; ⚪ def 0
r.MotionBlurQuality=0; ⚫ EDITED ⚪ def 4
r.NGX.DLSS.DilateMotionVectors=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.NGX.DLSS.PreferNISSharpen=0; ⚫ EDITED ⚪ def 1
r.NGX.DLSS.Quality.Auto=0; ⚫ EDITED ⚪ def 1
r.NGX.DLSS.Quality=1; 🔴 -2,-1,0,1 for PERFORMANCE ⚫ EDITED ⚪ def -1 🔵 DLSS
r.NGX.LogLevel=0; ⚫ EDITED ⚪ def 1 🔵 debug
r.ParallelShadows=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.ParticleLightQuality=1; 🔴 0,1 for PERFORMANCE ⚪ def 2
r.RayTracing=0; ⚪ def 0
r.RefractionQuality=1; 🔴 0,1 for PERFORMANCE ⚫ EDITED ⚪ def 2
r.RenderTargetPoolMin=400; ⚪ def 400
r.SceneColorFormat=3; 🔴 2,3 for PERFORMANCE ⚫ EDITED ⚪ def 4
r.SceneColorFringe.Max=0; ⚫ EDITED ⚪ def -1
r.Shadow.CachedShadowsCastFromMovablePrimitives=1; 🔴 0 for PERFORMANCE ⚪ def 1 🔵 movable light shadows
r.Shadow.CSM.MaxCascades=2; 🔴 1,2,4 for PERFORMANCE ⚫ EDITED ⚪ def 10
r.Shadow.CSMShadowDistanceFadeoutMultiplier=1; ⚪ def 1
r.Shadow.DistanceScale=1; 🔴 0.7 for PERFORMANCE ⚪ def 1
r.Shadow.FilterMethod=0; 🔴 0 for PERFORMANCE ⚪ def 0 🔵 pcss shadows
r.Shadow.ForceSingleSampleShadowingFromStationary=0; 🔴 1 for PERFORMANCE ⚪ def 0
r.Shadow.MaxCSMResolution=2048; 🔴 512,1024 for PERFORMANCE ⚪ def 2048
r.Shadow.MaxResolution=512; 🔴 512,1024 for PERFORMANCE ⚫ EDITED ⚪ def 2048
r.Shadow.Nanite=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.Shadow.NaniteLODBias=1; 🔴 1 for PERFORMANCE ⚪ def 1
r.Shadow.PreShadowResolutionFactor=0.5; ⚪ def 0.5
r.Shadow.RadiusThreshold=0.04; 🔴 0.06,0.05,0.04,0.03 for PERFORMANCE ⚫ EDITED ⚪ def 0.01
r.Shadow.Virtual.Cache.StaticSeparate=1; ⚪ def 1
r.Shadow.Virtual.Clipmap.FirstLevel=6; ⚪ def 6
r.Shadow.Virtual.Enable=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.Shadow.Virtual.ForceOnlyVirtualShadowMaps=1; 🔴 1 for PERFORMANCE ⚪ def 1
r.Shadow.Virtual.MaxPhysicalPages=2048; 🔴 512,2048 to lower vram usage ⚫ EDITED ⚪ def 4096
r.Shadow.Virtual.OnePassProjection.MaxLightsPerPixel=8; 🔴 8 for PERFORMANCE ⚫ EDITED ⚪ def 16
r.Shadow.Virtual.OnePassProjection=1; 🔴 1 for PERFORMANCE ⚪ def 1
r.Shadow.Virtual.ResolutionLodBiasDirectional=-0.5; 🔴 0,-0.5,-1 for PERFORMANCE ⚫ EDITED ⚪ def -1.5
r.Shadow.Virtual.ResolutionLodBiasDirectionalMoving=-0.5; 🔴 0,-0.5,-1 for PERFORMANCE ⚫ EDITED ⚪ def -1.5
r.Shadow.Virtual.ResolutionLodBiasLocal=1; 🔴 1 for PERFORMANCE ⚫ EDITED ⚪ def 0
r.Shadow.Virtual.SMRT.MaxRayAngleFromLight=0.03; ⚪ def 0.03
r.Shadow.Virtual.SMRT.RayCountDirectional=4; 🔴 0,4 for PERFORMANCE ⚫ EDITED ⚪ def 8
r.Shadow.Virtual.SMRT.RayCountLocal=4; 🔴 0,4 for PERFORMANCE ⚫ EDITED ⚪ def 8
r.Shadow.Virtual.SMRT.RayLengthScaleDirectional=1; ⚫ EDITED ⚪ def 1.5
r.Shadow.Virtual.SMRT.SamplesPerRayDirectional=2; 🔴 2 for PERFORMANCE ⚫ EDITED ⚪ def 4
r.Shadow.Virtual.SMRT.SamplesPerRayLocal=2; 🔴 2 for PERFORMANCE ⚫ EDITED ⚪ def 4
r.Shadow.Virtual.SMRT.TexelDitherScaleDirectional=2; ⚪ def 2
r.Shadow.Virtual.TranslucentQuality=0; 🔴 0 for PERFORMANCE ⚪ def 0
r.ShadowQuality=5; 🔴 3,4 for PERFORMANCE ⚪ def 5
r.SkeletalMeshLODBias=0; 🔴 2,1 for PERFORMANCE ⚪ def 0 🔵 skeletal mesh bias if supported
r.SkyAtmosphere.AerialPerspectiveLUT.DepthResolution=8; 🔴 8 for PERFORMANCE ⚫ EDITED ⚪ def 16
r.SkyAtmosphere.AerialPerspectiveLUT.FastApplyOnOpaque=1; 🔴 1 for PERFORMANCE ⚪ def 1
r.SkyAtmosphere.AerialPerspectiveLUT.SampleCountMaxPerSlice=2; 🔴 2 for PERFORMANCE ⚫ EDITED ⚪ def 4
r.SkyAtmosphere.FastSkyLUT.SampleCountMax=32; 🔴 16,32,64 for PERFORMANCE ⚫ EDITED ⚪ def 128
r.SkyAtmosphere.FastSkyLUT.SampleCountMin=4; 🔴 1 for PERFORMANCE ⚪ def 4
r.SkyAtmosphere.LUT32=0; 🔴 0 for PERFORMANCE ⚪ def 0
r.SkyAtmosphere.MultiScatteringLUT.HighQuality=0; 🔴 0 for PERFORMANCE ⚪ def 0
r.SkyAtmosphere.SampleCountMax=32; 🔴 16,32,64 for PERFORMANCE ⚫ EDITED ⚪ def 128
r.SkyAtmosphere.SampleCountMin=4; 🔴 1 for PERFORMANCE ⚪ def 4
r.SkyAtmosphere.SampleLightShadowmap=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1 🔵 volumetric shadows
r.SkyAtmosphere.TransmittanceLUT.SampleCount=10; ⚪ def 10
r.SkyAtmosphere.TransmittanceLUT.UseSmallFormat=0; 🔴 1 for PERFORMANCE ⚪ def 0
r.SkyLight.RealTimeReflectionCapture.TimeSlice.SkyCloudCubeFacePerFrame=6; ⚪ def 6
r.SSGI.Enable=0; 🔴 0 for PERFORMANCE ⚪ def 0
r.SSR.HalfResSceneColor=1; 🔴 1 for PERFORMANCE ⚫ EDITED ⚪ def 0
r.SSR.Quality=3; 🔴 0,2 for PERFORMANCE ⚪ def 3
r.SSS.Burley.Quality=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.SSS.Checkerboard=1; 🔴 1 for PERFORMANCE ⚫ EDITED ⚪ def 2
r.SSS.HalfRes=1; 🔴 1 for PERFORMANCE ⚫ EDITED ⚪ def 0
r.Streaming.AmortizeCPUToGPUCopy=0; ⚪ def 0
r.Streaming.Boost=1; ⚪ def 1
r.Streaming.DropMips=0; ⚪ def 0 🔵 debug
r.Streaming.FramesForFullUpdate=5; ⚪ def 5
r.Streaming.HiddenPrimitiveScale=0.5; 🔴 0.5 for PERFORMANCE ⚪ def 0.5
r.Streaming.LimitPoolSizeToVRAM=1; ⚫ EDITED ⚪ def 0
r.Streaming.MaxEffectiveScreenSize=0; ⚪ def 0
r.Streaming.MaxNumTexturesToStreamPerFrame=0; ⚪ def 0
r.Streaming.MipBias=0; 🔴 1 for PERFORMANCE ⚪ def 0
r.Streaming.NumStaticComponentsProcessedPerFrame=50; ⚪ def 50
r.Streaming.PoolSize.VRAMPercentageClamp=1024; ⚪ def 1024
r.Streaming.PoolSize=3000; 🔴 1000 to lower vram usage ⚫ EDITED ⚪ def 1000 🔵 texture pool size
r.Streaming.UseFixedPoolSize=0; ⚪ def 0 🔵 change poolsize at run time
r.SubsurfaceScattering=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.SupportMaterialLayers=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.TemporalAA.Quality=2; 🔴 1 for PERFORMANCE ⚪ def 2
r.TemporalAA.Upsampling=1; 🔴 0 for PERFORMANCE ⚪ def 1 🔵 TAAU
r.TessellationAdaptivePixelsPerTriangle=999999; 🔴 999999 for PERFORMANCE ⚫ EDITED ⚪ def 48
r.Tonemapper.Quality=2; ⚫ EDITED ⚪ def 5
r.Translucency.DynamicRes.TimeBudget=0; ⚪ def 0
r.TranslucencyLightingVolumeDim=48; 🔴 32,48 for PERFORMANCE ⚫ EDITED ⚪ def 64
r.TranslucencyVolumeBlur=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.TSR.History.GrandReprojection=0; ⚪ def 0
r.TSR.History.R11G11B10=1; ⚪ def 1
r.TSR.History.ScreenPercentage=100; ⚫ EDITED ⚪ def 200
r.TSR.History.SeparateTranslucency=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.TSR.History.UpdateQuality=3; ⚪ def 3
r.TSR.RejectionAntiAliasingQuality=2; ⚪ def 2
r.TSR.Resurrection=0; 🔵 experimental
r.TSR.ShadingRejection.Flickering.Period=2; ⚪ def 2
r.TSR.ShadingRejection.Flickering=1; ⚪ def 1
r.TSR.Velocity.Extrapolation=0; 🔵 experimental
r.TSR.Velocity.HoleFill=0; 🔵 dummy variable
r.Upscale.Quality=3; 🔴 1,2 for PERFORMANCE ⚪ def 3
r.ViewDistanceScale=1; 🔴 0.8 for PERFORMANCE ⚪ def 1
r.VolumetricCloud.DistanceToSampleMaxCount=15; ⚪ def 15
r.VolumetricCloud.EnableAtmosphericLightsSampling=1; ⚪ def 1
r.VolumetricCloud.EnableDistantSkyLightSampling=1; ⚪ def 1
r.VolumetricCloud.EnableLocalLightsSampling=0; 🔴 0 for PERFORMANCE ⚪ def 0 🔵 experimental
r.VolumetricCloud.HzbCulling=0; 🔵 cloud hzb culling
r.VolumetricCloud.ReflectionRaySampleMaxCount=1; 🔵 reflection ray sample max
r.VolumetricCloud.SampleMinCount=2; ⚪ def 2
r.VolumetricCloud.Shadow.ReflectionRaySampleMaxCount=24; ⚪ def 24
r.VolumetricCloud.Shadow.SampleAtmosphericLightShadowmap=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.VolumetricCloud.Shadow.ViewRaySampleMaxCount=1; 🔵 shadow ray sample max
r.VolumetricCloud.ShadowMap.MaxResolution=2048; ⚪ def 2048
r.VolumetricCloud.ShadowMap.SpatialFiltering=1; ⚪ def 1
r.VolumetricCloud.ShadowMap.TemporalFiltering.NewFrameWeight=1; ⚪ def 1 🔵 experimental
r.VolumetricCloud.ShadowMap=1; 🔴 0 for PERFORMANCE ⚪ def 1 🔵 cloud shadows
r.VolumetricCloud.SkyAO.MaxResolution=2048; ⚫ EDITED ⚪ def 2048
r.VolumetricCloud.SkyAO=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.VolumetricCloud.ViewRaySampleMaxCount=768; ⚪ def 768
r.VolumetricCloud=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.VolumetricFog.GridPixelSize=16; ⚪ def 16
r.VolumetricFog.GridSizeZ=64; ⚪ def 64
r.VolumetricFog=1; 🔴 0 for PERFORMANCE ⚪ def 1
r.VolumetricRenderTarget.Mode=2; ⚫ EDITED ⚪ def 0
r.VolumetricRenderTarget.ReprojectionBoxConstraint=1; ⚫ EDITED ⚪ def 0
r.VolumetricRenderTarget.UpsamplingMode=2; ⚫ EDITED ⚪ def 4
r.VT.MaxAnisotropy=8; 🔴 0,4 for PERFORMANCE ⚪ def 8
r.VT.MaxTilesProducedPerFrame=30; ⚪ def 30
r.VT.MaxUploadsPerFrame=8; ⚪ def 8
r.Water.EnableShallowWaterSimulation=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.Water.EnableUnderwaterPostProcess=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.Water.SingleLayer.SSR=0; 🔴 0 for PERFORMANCE ⚫ EDITED ⚪ def 1
r.Water.WaterMesh.TessFactorBias=0; 🔴 -1 for PERFORMANCE ⚪ def 0
RHI.MaximumFrameLatency=1; ⚫ EDITED ⚪ def 3 🔵 frame latency
rhi.SyncInterval=1; ⚪ def 1
rhi.SyncSlackMS=10; ⚪ def 10
t.Streamline.Reflex.Auto=0; ⚫ EDITED ⚪ def 1
t.Streamline.Reflex.Enable=1; ⚫ EDITED ⚪ def 0 🔵 nvidia reflex
t.Streamline.Reflex.Mode=2; ⚫ EDITED ⚪ def 1 🔵 1,2 reflex,reflex with boost
```

---

#### Open Input.ini and copy pasta %localappdata%

#### or Repak.bat method (zzz_ENGINE_INI\Engine\Config\Windows\WindowsInput.ini)

```python
[/Script/Engine.InputSettings]
bAltEnterTogglesFullscreen=1;
bEnableMouseSmoothing=0;
bF11TogglesFullscreen=0;
ButtonRepeatDelay=0.1;
bViewAccelerationEnabled=0;
DoubleClickTime=0.01; ⚫ EDITED ⚪ def 0.1
InitialButtonRepeatDelay=0.1; ⚫ EDITED ⚪ def 0.2
```

---

#### Open GameUserSettings.ini these commands can overwrite your config if they are here %localappdata%

#### you can turn down used scalability groups here or in game if they are being used

```python
[ScalabilityGroups]
sg.HairQuality=?;
sg.ResolutionQuality=?;

AmbientOcclusion=(Value=?);
AntiAliasingMode=(Value=?);
AudioQualityLevel=?;
bBounceLightEnabled=?;
bConsoleEnabled=?;
bDepthOfField=?;
bFlashlightShadowsEnabled=?;
bFrameLimitEnabled=?;
bMotionBlur=?;
bRTXAmbientOcclusionEnabled=?;
bRTXEnabled=?;
bRTXReflectionsEnabled=?;
bRTXShadowsEnabled=?;
bTelemetryEnabled=?;
bUseDynamicResolution=?;
bUseVSync=?;
ContactShadows=(Value=?);
ContactShadows=?;
DetailMode=(Value=?);
DFAO=?;
DistanceFieldShadows=?;
DlssQualitySetting=?;
DoubleKeyPressTime=?;
FoliageMinLOD=(Value=?);
FrameRateLimit=?;
FullscreenMode=?;
Gamma=?;
GlobalSensitivity=?;
GraphicsPresetIndex=?;
GraphicsQuality=?;
HDRDisplayOutputNits=?;
HZBOcclusion=(Value=?);
LastSavedAAQuality=?;
LastSavedAASamples=?;
MaterialQuality=(Value=?);
MaxAnisotropy=(Value=?);
MaxAnisotropy=?;
MaxFPS=?;
MenuFrameRateLimit=?;
OceanQuality=(Value=?);
OverrideOptions=(("r.command",(Value=?,bModified=True)),("r.command",(Value=?,bModified=True)));
PostFX_Saturation=?;
PostFX_Sharpness=?;
ResolutionScaleModifier=?;
ScreenPercentage=(Value=?);
SkeletalMeshLODBias=(Value=?);
TAASampleStorage=?;
TemporalAASamples=(Value=?);
Tessellation=(Value=?);
TessellationMode=(Value=?);
TextureStreamPoolSizeStorage=(Value=?);
WakeSim=(Value=?)
```

---

#### Open DeviceProfiles.ini for textures lods, mess around or just skip %localappdata%

```python
[/Script/Engine.TextureLODSettings]
TextureLODGroups=(Group=TEXTUREGROUP_World,                 MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldNormalMap,        MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WorldSpecular,         MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Character,             MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterNormalMap,    MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_CharacterSpecular,     MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Weapon,                MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponNormalMap,       MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_WeaponSpecular,        MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Vehicle,               MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_VehicleNormalMap,      MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_VehicleSpecular,       MinLODSize=256,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Cinematic,             MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Effects,               MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=linear, MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_EffectsNotFiltered,    MinLODSize=128,  MaxLODSize=1024, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Skybox,                MinLODSize=2048, MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_UI,                    MinLODSize=2048, MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Lightmap,              MinLODSize=32,   MaxLODSize=32,                            LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_Shadowmap,             MinLODSize=32,   MaxLODSize=32,                            LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_RenderTarget,          MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_MobileFlattened,       MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_Face,     MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_ProcBuilding_LightMap, MinLODSize=32,   MaxLODSize=32,                            LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_ColorLookupTable,      MinLODSize=2048, MaxLODSize=2048,                          LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Heightmap,     MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Terrain_Weightmap,     MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Bokeh,                 MinLODSize=256,  MaxLODSize=256,                           LODBias=0, MinMagFilter=linear, MipFilter=linear, MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_IESLightProfile,       MinLODSize=256,  MaxLODSize=2048, OptionalMaxLODSize=512,  LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_Pixels2D,              MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_HierarchicalLOD,       MinLODSize=512,  MaxLODSize=4096, OptionalMaxLODSize=1024, LODBias=0, MinMagFilter=aniso,  MipFilter=point,  MipGenSettings=TMGS_SimpleAverage, NumStreamedMips=-1);
TextureLODGroups=(Group=TEXTUREGROUP_8BitData,                                                                         LODBias=0, MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
TextureLODGroups=(Group=TEXTUREGROUP_16BitData,                                                                        LODBias=0, MinMagFilter=point,  MipFilter=point,  MipGenSettings=TMGS_NoMipmaps,     NumStreamedMips=0);
```

---
