# Minecraft
<img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft is a sandbox game that works using **OpenGL**.
## Get Started
First of all, I definitely suggest that you use <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> [Prism Launcher](https://github.com/PrismLauncher/PrismLauncher) because it is **open source** and it provides more options than the official <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft launcher.
### Install Prism Launcher
You can install <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher following [these steps according to your distribution](https://prismlauncher.org/download/?from=button).
### Install Java
<img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher automatically installs Java for you.
### Install Minecraft
- Launch <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher and continue until the **memory allocation** step.
- Then, make sure to change `Maximum memory allocation` value. There is a rumor that if you allocate half your RAM, you are going to get good performance. However, this is wrong because:
  - When you play <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft, the game tries to free up allocated memory that is no longer used by objects to avoid memory issues. This is called **garbage collection**.
    - However, you **should not** allocate **too much or too little** RAM, because:
      - If you allocate **too much** RAM, the game will wait longer between garbage collection cycles and each cycle will take longer to complete, that's why you are going to get bigger lag spikes.
      - If you allocate **too little** RAM, the game will perform garbage collection too often and this will cause big lag spikes again.
    - When <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft uses between `50-75%` of allocated RAM, it is the ideal value for smaller lag spikes. I suggest that you experiment different values yourself to find your ideal value. You can check RAM usage by pressing `F3` during the gameplay.
- After completing quick setup, add your <img width="16" height="25" alt="microsoft" src="https://github.com/user-attachments/assets/d19efd30-17c2-4af2-9147-121dd23ebda6" /> Microsoft account in the launcher.
- **Next** : `Add Instance` **-** `Version` **-** `Select the version you desire and scroll down` **-** `Select "Fabric" as the mod loader` **-** `OK`
## Optimization
- `Settings` **-** `Minecraft` **-** `Tweaks` **-** `Enable Feral GameMode` **&** `Use discrete GPU (only if you have two GPUs)`
- `Settings` **-** `Environment Variables` **-** `Add` **-** `mesa_glthread=true`
<img width="731" height="96" alt="image" src="https://github.com/user-attachments/assets/3cd34257-d1cf-4509-8967-d8499e61318a" />

- If you are using <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/675b9126-59e6-4fbf-af53-1a023465daf7" /> **NVIDIA**, you should use the `__GL_THREADED_OPTIMIZATIONS=1` environment variable instead.
- You are ready to play <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft now. However, the performance of the game can still be increased through performance mods and optimized in-game settings.
## <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6cf43b97-0cc2-4867-afd8-078e2921fc2b" /> Sodium Method - Recommended for Version 1.16.3 and Later
`Right click Minecraft instance` **-** `Edit` **-** `Mods` **-** `Download mods`
### Essential Performance-Increasing Mods and Dependencies
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/92248b98-184c-4276-b0fa-fcda3fe75472" /> [Alternate Current](https://modrinth.com/mod/alternate-current)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7132b796-85f6-49a8-9c96-213106a6be3f" /> [AsyncParticles](https://modrinth.com/mod/asyncparticles)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1f386453-e995-452e-a87f-95157f3fe3fe" /> [BadOptimizations](https://modrinth.com/mod/badoptimizations)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7f4ae3ef-99b3-4533-8bf6-978b0cf1e877" /> [Better Biome Reblend](https://modrinth.com/mod/bbrb)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/15cd42eb-fa80-4855-b21a-07538165dd9a" /> [Concurrent Chunk Management Engine](https://modrinth.com/mod/c2me-fabric)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/232977c7-0ac0-4d8e-a877-e7f7794a9874" /> [Debugify](https://modrinth.com/mod/debugify)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/4373d9ec-48b8-4bb4-92dc-719962e4dc43" /> [Dynamic FPS](https://modrinth.com/mod/dynamic-fps)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f8b036c0-221c-4f12-bf58-385a4804b6ff" /> [Fabric API](https://modrinth.com/mod/fabric-api)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/48535102-153e-446d-829c-ed27fb4391fb" /> [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/28a987ce-fdac-4843-9c96-bbcd971bf9aa" /> [Fadeless](https://modrinth.com/mod/fadeless)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/2471f744-dead-4151-93fa-151fe138b842" /> [Fast IP Ping](https://modrinth.com/mod/fast-ip-ping)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3fffc2a4-0e63-40f9-9719-e379cfdaf9ce" /> [Fast Item Frames](https://modrinth.com/mod/fast-item-frames)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/ba1d30cd-e721-46b9-9e62-65543c643b12" /> [FastQuit](https://modrinth.com/mod/fastquit)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/2a7ddd1e-8664-42e2-b8ac-d4aece4e5292" /> [FerriteCore](https://modrinth.com/mod/ferrite-core)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3269b8ed-7731-410d-a581-7a8144c06e12" /> [GPU Tape](https://modrinth.com/mod/gputape)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/ab8c6ab5-9494-455e-914d-bed1a097ad83" /> [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/98609414-ff79-4be0-ac62-b84d7076ba25" /> [Krypton](https://modrinth.com/mod/krypton)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/c1a3edac-6ef7-48ec-beef-b0b6201f3f8a" /> [Lithum](https://modrinth.com/mod/lithium)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f4a02bad-226a-4c02-8e2d-05b38ab423cd" /> [Mod Menu](https://modrinth.com/mod/modmenu)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/54448033-1b48-4da5-ac3a-8929b6a86591" /> [ModernFix](https://modrinth.com/mod/modernfix)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/df48f692-fceb-43b8-8d9a-ca0c8631c068" /> [No Chat Reports](https://modrinth.com/mod/no-chat-reports)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/4c2d1972-8856-4877-b338-f70dd49ac6b9" /> [Noisium](https://modrinth.com/mod/noisium)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/8673044d-ad8c-4d9e-a8da-973fd47fbfdd" /> [PacketFixer](https://modrinth.com/mod/packet-fixer)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6fb44882-8266-4436-b72f-187c8e314bf5" /> [Particle Core](https://modrinth.com/mod/particle-core)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/be35e263-1f27-4503-9473-2ac0df093585" /> [Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/fc05d450-b282-484c-8ccb-b435a5862132" /> [Remove Reloading Screen](https://modrinth.com/mod/rrls)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cfdb1b64-8465-43e5-abdf-9c87071d16f9" /> [ScalableLux](https://modrinth.com/mod/scalablelux)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6cf43b97-0cc2-4867-afd8-078e2921fc2b" /> [Sodium](https://modrinth.com/mod/sodium)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3e1b5c91-ec49-4d00-a583-ad4f138416a0" /> [Sodium Extra](https://modrinth.com/mod/sodium-extra)
### Optional Performance-Increasing Mods
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e891a10e-feed-4897-8807-ebf071ad506e" /> [Clumps](https://modrinth.com/mod/clumps/versions)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/a41952e1-e8b7-4c72-82db-a49df053213b" /> [Exordium](https://modrinth.com/mod/exordium)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/254a83a8-2c31-4d3b-9055-635face279fd" /> [Let Me Despawn](https://modrinth.com/plugin/lmd)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d8dc60e0-a46f-4b07-82d1-4aba5f26151c" /> [WayFix](https://modrinth.com/mod/wayfix) - *Use this mod only if you are using* **Linux (Wayland)**. *After installing the mod, follow the next steps for full functionality:*
    - `Right click your Minecraft instance` **-** `Edit` **-** `Settings` **-** `Workarounds` **-** `Check "Native libraries"` **-** `Check "Use system installation of GLFW"`
### Quality of Life Mods
These mods do not increase performance but they can enhance your gaming experience.
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f4416a16-ef2b-484b-beb9-14bcf8739749" /> [AppleSkin](https://modrinth.com/mod/appleskin)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/89647668-920c-4c1a-acda-bbbe3df37439" /> [Better Advancements](https://modrinth.com/mod/better-advancements)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/65ebc980-673d-443a-af1a-58491bae4320" /> [Better Clouds](https://modrinth.com/mod/better-clouds)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/975a6695-c061-448a-a8b0-efb9febbb44d" /> [Better Mount HUD](https://modrinth.com/mod/better-mount-hud)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/457a456b-6aa7-4d08-a763-596887b3fc1a" /> [BetterF3](https://modrinth.com/mod/betterf3)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/06629688-afe5-4c33-8b2e-cd216b8a3c03" /> [Chat Heads](https://modrinth.com/mod/chat-heads)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7a092471-2d3c-4750-b98a-5b03bba15d4a" /> [Continuity](https://modrinth.com/mod/continuity)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e15e0dd-f84d-4ab5-8de9-89bc83049848" /> [e4mc](https://modrinth.com/mod/e4mc)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/415b2b80-4f6c-46b9-b522-29abd57992db" /> [Entity Model Features](https://modrinth.com/mod/entity-model-features)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/280b9bcb-8abc-4e2a-998a-628fdfbaf919" /> [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures)
  - You need to install some resource packs for **EMF** and **ETF** mods to work. These resource packs are:
    - <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/5871c983-84ec-4dce-8e2e-70ff170f4327" /> [Fresh Animations](https://modrinth.com/resourcepack/fresh-animations)
    - <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/bc16bf62-c45a-4118-bd1e-86335e84ac57" /> [Fresh Moves](https://modrinth.com/resourcepack/tras-fresh-player)
    - <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/8c424367-bb07-472a-a6a6-58b1ae02dda9" /> [Fresh Animations: Extensions](https://modrinth.com/resourcepack/fresh-animations-extensions)
    - <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f2f43428-391e-46c0-ac10-8d53ecc5d1ee" /> [Trailer Player Animations](https://modrinth.com/resourcepack/fresh-player-animations)
    - Make sure the texture packs are placed accordingly like in the example:

      - <img width="187" height="305" alt="image" src="https://github.com/user-attachments/assets/0cced448-c8a0-48ef-8a7e-0f9a140449a7" />

- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/b6c27501-d819-4e0a-b3b4-cc17169fcac1" /> [Explosive Enhancement](https://modrinth.com/mod/explosive-enhancement)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/71bd5880-201b-41f8-bb5e-053949267b94" /> [Hold My Items](https://modrinth.com/mod/hold-my-items)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/ce6dca60-a2d4-49c7-9f17-ba571558325f" /> [Iris Shaders](https://modrinth.com/mod/iris)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/62a10ece-8839-4a3e-8307-797206324ec8" /> [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/98ad55b0-d271-4246-ad19-a43a32da9853" /> [MinecraftCapes](https://modrinth.com/mod/minecraftcapes)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1cc81c04-523b-4baa-85aa-ca4ea87ef9e4" /> [Model Gap Fix](https://modrinth.com/mod/modelfix)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/fb5b0718-ba49-4a70-8454-05f4dd6fd988" /> [Not Enough Animatons](https://modrinth.com/mod/not-enough-animations)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/77bf5030-673d-443c-8c62-2006b0d379ef" /> [Sit](https://modrinth.com/mod/bl4cks-sit)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/fc8149d9-567a-4a17-beed-c59407297cc1" /> [Smooth Scroll](https://modrinth.com/mod/smooth-scroll)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3e42a5d2-c40e-4eba-8a97-533b4b1ab59b" /> [Subtle Effects](https://modrinth.com/mod/subtle-effects) - *disable* **Particle Core mod** *or disable* **particle culling feature** using **Mod Menu mod** *if you want to use this mod*
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/8aa74f40-726c-4cd5-ae01-ce14aad9bd6a" /> [ViaFabricPlus](https://modrinth.com/mod/viafabricplus)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/47669d5e-eb43-44cf-a8b3-225d7ed35cc2" /> [Zoomify](https://modrinth.com/mod/zoomify)
### <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6cf43b97-0cc2-4867-afd8-078e2921fc2b" /> Sodium - In-Game Optimized Settings
- **If you are going to use Zoomify :** `Options` **-** `Controls` **-** `Key Binds` **-** `Change key bind of "Save Hotbar Activator" to something else` **-** `Done`
- `Options` **-** `Resource Packs` **-** `Move "Default Connected Textures" and "Glass Pane Culling Fix" to the right section` **-** `Done`
- `Options` **-** `Video Settings`
  - **General**
    - `Render Distance` **:** 6 chunks
    - `Simulation Distance` **:** 5 chunks
    - `VSync` **:** OFF
    - `Max Framerate` **:** Same value as your **monitor's refresh rate**. If your monitor's refresh rate is **lower than 144 Hz**, try either *unlimited* (might cause overheating) or *double your monitor's refresh rate* (e.g., 120 FPS for 60 Hz screen)
  - **Quality**
    - `Graphics` **:** Fast
    - `Clouds` **:** OFF
    - `Weather` **:** Fast
    - `Leaves` **:** Fast
    - `Particles` **:** Decreased
    - `Biome Blend` **:** 1 block(s)
    - `Entity Distance` **:** 50%
    - `Entity Shadows` **:** OFF
    - `Distortion Effects` **:** 60%
    - `FOV Effects` **:** 60%
    - `Mipmap Levels` **:** 1x
## <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d0f7a6ff-9f07-4c91-b88d-02440fa1e87e" /> VulkanMod Method - Recommended for Version 1.18.2 and Later (for GPUs that completely support Vulkan)
`Right click Minecraft instance` **-** `Edit` **-** `Mods` **-** `Download mods`
### Essential Mods for The Method
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d0f7a6ff-9f07-4c91-b88d-02440fa1e87e" /> [VulkanMod](https://modrinth.com/mod/vulkanmod)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/a1c77f17-1e27-4de5-8729-538a4d4f77a3" /> [VulkanMod Extra](https://modrinth.com/mod/vulkanmod-extra)
- You can use all the mods that are mentioned in <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6cf43b97-0cc2-4867-afd8-078e2921fc2b" /> Sodium method **except:**
  - Better Clouds
  - Exordium
  - ImmediatelyFast
  - Iris Shaders
  - Sodium
  - SodiumExtra
## <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7f6b0e27-e777-46c7-a6e0-bc443b0679e0" /> Optifine Method - Recommended for Version 1.16.2 and Earlier
- If you want to use <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7f6b0e27-e777-46c7-a6e0-bc443b0679e0" /> Optifine, I suggest that you use **the official <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft launcher** instead because it is going to be hard and meaningless to use <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7f6b0e27-e777-46c7-a6e0-bc443b0679e0" /> Optifine through <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher.
- Simply, download <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7f6b0e27-e777-46c7-a6e0-bc443b0679e0" /> [Optifine](https://optifine.net/downloads) for the <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft version you would like to play and click `Install` after running the **.jar** file you downloaded.
### <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7f6b0e27-e777-46c7-a6e0-bc443b0679e0" /> Optifine - In-Game Optimized Settings
- `Options`
  - **Video Settings**
    `Graphics` **:** Fast
    - `Smooth Lighting` **:** ON
    - `Smooth Lighting Level` **:** 50%
    - `Render Distance` **:** 6 chunks
    - `Simulation Distance` **:** 5 chunks
    - `Max Framerate` **:** Same value as your **monitor's refresh rate**. If your monitor's refresh rate is **lower than 144 Hz**, try either *unlimited* (might cause overheating) or *double your monitor's refresh rate* (e.g., 120 FPS for 60 Hz screen)
    - `Entity Shadows` **:** OFF
    - **Quality...**
      - `Mipmap Levels` **:** 1
      - `Emissive Textures` **:** OFF
      - `Custom Fonts` **:** OFF
      - `Connected Textures` **:** Fast
      - `Custom Sky` **:** OFF
      - `Custom Entity Models` **:** OFF
      - `Random Entities` **:** OFF
      - `Custom Colors` **:** OFF
      - `Natural Textures` **:** OFF
      - `Custom Items` **:** OFF
      - `Custom GUIs` **:** OFF
      - `Distortion Effects` **:** 60%
      - `FOV Effects` **:** 60%
    - **Details...**
      - `Clouds` **:** OFF
      - `Trees` **:** Fast
      - `Fog` **:** OFF
      - `View Bobbing` **:** OFF
      - `Vignette` **:** Fast
      - `Rain & Snow` **:** Fast
      - `Stars` **:** Subjective
      - `Swamp Colors` **:** OFF
      - `Alternate Blocks` **:** OFF
      - `Entity Distance` **:** 50%
      - `Biome Blend` **:** 3x3
    - **Performance...**
      - `Render Regions` **:** OFF
      - `Smart Animations` **:** ON
      - `Smooth FPS` **:** ON
      - `Fast Render` **:** ON
      - `Fast Math` **:** ON
      - `Smooth World` **:** ON
    - **Animations...**
      - `Textures Animated` **:** OFF
      - `Particles` **:** Decreased
    - **Other...**
      - `Telemetry` **:** OFF
# Conclusion
This guide was about Minecraft installation and optimization on Linux. I hope the guide has been useful. Thank you for reading, happy gaming! 🐧
