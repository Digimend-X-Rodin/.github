Device: Poco X7 Pro 5G
Device code name: rodin
Device maintainer: Omkar Parte

Lunaris AOSP v3.13
Date - 08/11/2026

Changelog – 148 commits

1. Import Lunaris blur optimizations patch
2. Make use of flag TARGET_LOW_END_BLUR
3. Optimize UI rendering & adjust display properties
4. audio: Fix static/crackling in game voice chat
5. sepolicy: Grant system_server batteryinfo
6. Build Bluetooth audio from source
7. sepolicy: Label audio props + SmartPA calibration node
8. Correct ownership for /dev/ufs-bsg0
9. Build minimal MediaTek telecom/telephony-common JARs
10. Move MediaTek IMS bootjars back to system_ext
11. blob-patches: Update IMS patches
12. sepolicy: Move to common MediaTek sepolicy vndr
13. Drop HIDL lbs/netdagent, build from source
14. Drop secure video encoders (fix Discord screen share)
15. Move mtk_platform_codecs_config.xml to device tree
16. Enable MM zRAM daemon support
17. powerhint: Fix AUDIO_STREAMING_LOW_LATENCY state
18. fastbootd enabled by default
19. sepolicy: Fix audio feedback via MTK prop namespace bypass
20. Fix GPay & Chrome black screen camera
21. Revert "Add misound audio blobs for Aurisys"
22. Retune LMK & protect init from OOM kills
23. Disable fpsop game effects and BT misound
24. init: Sync permissions with stock OS3.0.303.0
25. sepolicy: Move to common sepolicy vndr
26. Update blobs to OS3.0.303.0.WOJMIXM
27. sepolicy: Address sysfs_dmabuf denials
28. Build dummy libion_mtk
29. Enable legacy MTK raw vendor parameters
30. Include chipinfo script
31. Drop chipinfo, build from source
32. Move Xiaomi secure element blobs out of NFC section
33. Change Bluetooth vendor ID to MediaTek, Inc.
34. Drop MediaTek thermal core
35. Drop unused/duplicated mkbootimg args
36. Drop MediaTek Mali ICompression service
37. Build IMtkAudio interface
38. Build wlan_assistant daemon from source
39. Switch to prebuilt WiFi HAL
40. SystemUI: Adjust physical power button Y location
41. SystemUI: Reduce blur radius to avoid artifacts
42. Launcher: Move enhanced blur radius to dimens.xml
43. Launcher: Reduce blur radius
44. Add sepolicy
45. parts: Handle full boot completed alongside locked boot
46. Address more sepolicy
47. Lunaris-AOSP bringup
48. Patch: Allow bypass-charge access to sysfs_batteryinfo
49. Add Fenrir source patches
50. Patch: Consolidate Xiaomi package allowlist extensions
51. Introduce automated source-side patching mechanism
52. Add misound audio blobs for Aurisys
53. Configure per-refresh-rate SurfaceFlinger durations
54. sepolicy: Label Dolby & MediaTek VDEC properties
55. Revert "Add android.hardware.audio.pro.xml permission"
56. Revert "Enable config_supportAudioSourceUnprocessed"
57. parts: Drop dedicated charging thermal profile & monitor
58. sepolicy: Allow vendor services to interact with system suspend
59. sepolicy: Allow citsensorservice access to persist/mnt_vendor
60. sepolicy: Labels/permissions for battery & charger sysfs
61. parts: Move Settings tile to System category
62. sepolicy: Add bypass charge node read access
63. Build bypass charge
64. Update blobs to OS3.0.302.0.WOJMIXM
65. Revert "Add device name/model as Poco X7 Pro"
66. Apply Leica video LUT fallbacks on extraction
67. Fix notification flicker and color distortion
68. sepolicy: Address ADPF scheduling & misc hardware denials
69. Import ADPF profiles & display tuning from frankel
70. sepolicy: Split parts_app policy for Treble compliance
71. Redesign and extend XiaomiParts
72. Add sepolicy
73. Add shell perms to write ZRAM
74. UDFPS: Dynamic animation size & offset calculations
75. Enable zram earlier during boot
76. Set correct parameter for A2DP suspend
77. Enable double-tap & single-tap
78. sepolicy: Label fdsd persist dir for Xiaomi MTD service
79. Add device name/model as Poco X7 Pro
80. sepolicy: Address parts_app denials
81. Sync power hints with lineage-libperfmgr AIDL states
82. Optimize SurfaceFlinger composition & display pipeline
83. Relax thermal limits & tune CPU throttling thresholds
84. Revert "Optimize SurfaceFlinger composition & virtual display pipeline"
85. Revert "Increase Linux CMA memory allocation to 512M"
86. Enable MTK GED KPI
87. props: Optimize SurfaceFlinger & virtual display pipeline
88. Revert broken AI tuning, re-align with stock MTK configs
89. sepolicy: Address vendor service denials, clean property macros
90. sepolicy: Expose miev/migt/displayfeature props publicly
91. sepolicy: Drop neverallow
92. sepolicy: Import stock displayfeature props & backlight nodes
93. sepolicy: Add missing DMA-BUF & DMA-Heap policies
94. Update fingerprint for Fenrir
95. Pin Fenrir patch
96. Enable RKP TEE and StrongBox provisioning
97. Stop passing flag 3 to vbmeta images
98. Enable Fenrir support
99. Patch Dolby Vision codecs
100. sepolicy: Add more policy for vendorcodec
101. Add missing EGL config required by libmeow
102. extract-files: Consolidate duplicate blob fixups
103. fixup! sepolicy
104. sepolicy: CIT sensor test (jiiov) + more wakeup nodes
105. Switch to MEOW GL
106. f2fs: Enable ATGC on metadata partition
107. Increase Linux CMA memory allocation to 512M
108. Switch to explicit refresh rate controls
109. power: Adapt powerhint & cgroups to stock HyperOS
110. sepolicy: Add missing camera prop prefixes for miuicamera
111. sepolicy: Add missing property contexts from stock
112. sepolicy: Make vendor_mtdservice_prop vendor_public_prop
113. sepolicy: Add missing device nodes & socket contexts
114. sepolicy: Camera property definitions & access permissions
115. sepolicy: Move camera data file contexts to miuicamera
116. sepolicy: Allow vendor_init to read mtk_coredump_prop
117. sepolicy: Resolve denials, remove misys vendor HAL policies
118. sepolicy: Add vendorcodec domain for Dolby Vision codec
119. Add properties & init configs for Lunaris Dolby
120. Align graphics & SurfaceFlinger properties with stock
121. sepolicy: Address parts_app & vendor_init denials
122. GraphicBuffer size fixup for com.xiaomi.plugin.filter.so
123. Update Xiaomi Miui camera support
124. sepolicy: Label Rodin wakeup nodes
125. Aperture: Disable video stabilization
126. Enable config_supportAudioSourceUnprocessed
127. Add android.hardware.audio.pro.xml permission
128. Update blobs to OS3.0.301.0.WOJMIXM
129. sepolicy: Update hal_aidlbgservice from OS3.0.300.0
130. extract-files: Use libtinyxml2-v36 compat shim
131. Sync audio & media configs with stock
132. Add thermal symlinks
133. Disable MTE
134. Build MediaTek boot control service
135. Improve performance and thermal headroom
136. Build with Lunaris Dolby UI
137. sepolicy: Fix parts_app thermal & CIT audio denials
138. Import CIT stack and calibration blobs
139. sepolicy: Fix vendor camera & citsensorservice denials
140. sepolicy: Fix denials for Xiaomi Parts app
141. parts: Modernize UI with Jetpack Compose & Material 3
142. Overhaul power and thermal configurations
143. overlay: Reorganize & sync display configs with OS3.0.300.0
144. Clean up duplicate device framework matrix entries
145. Sync properties with OS3.0.300.0 & tune SurfaceFlinger
146. Adjust proprietary file extraction configurations
147. overlay: Disable config_sf_limitedAlpha
148. udfps: Refactor FOD touch & illumination handling