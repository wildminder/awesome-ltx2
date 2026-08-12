<p id="lora" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓ LoRA

### ▣ Enchancer, special

* Lightricks LTX-2.3
  * [LipDub IC-LoRA](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-LipDub) - Enables lip dubbing on top of LTX-2.3 for video dubbing via joint audio-visual diffusion (based on JustDubIt research)
* OmerHagawa
  * [Greenscreen Avatar IC-LoRA](https://huggingface.co/OmerHagawa/ltx2-greenscreen-avatar-ic-lora-vertical-v1) - Greenscreen avatar IC-LoRA for vertical video
* systms
  * [SYSTMS FLW IC-LoRA](https://huggingface.co/systms/SYSTMS-FLW-IC-LORA-LTX-2.3) - Seamless shot-to-shot transitions IC-LoRA with trigger word `FLW`, uses gray frames (RGB 127,127,127) between clips
* [LTX-2.3-IC-LoRA-Colorizer](https://huggingface.co/DoctorDiffusion/LTX-2.3-IC-LoRA-Colorizer) by [DoctorDiffusion](https://huggingface.co/DoctorDiffusion) (331 MB) - Colorize black and white videos
* [JUST-DUB-IT](https://huggingface.co/justdubit/justdubit)
* [Best-Face-Swap-Video](https://huggingface.co/Alissonerdx/BFS-Best-Face-Swap-Video)
* [Image-to-Video Adapter LoRA](https://huggingface.co/MachineDelusions/LTX-2_Image2Video_Adapter_LoRa)
  * Original by MachineDelusions
  * [siraxe variant](https://huggingface.co/siraxe/MachineDelusions_LTX-2_Image2Video_Adapter_LoRa) - Stripped audio layers + rank64 compressed (2.62 GB, 655 MB rank64 bf16)
* Lightricks LTX-2.3
  * [HDR](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-HDR) - Enables 16-bit HDR video generation and converts SDR video to HDR using LogC3 transform for extended dynamic range
  * [Union Control](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Union-Control) - Unified IC-LoRA combining Canny + Depth + Pose control signals for multi-signal video generation conditioning
  * [Motion Track Control](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Motion-Track-Control) - Guides object motion using sparse point trajectories via colored spline overlays on reference videos
* vrgamedevgirl84
  * [Enhancer1](https://huggingface.co/vrgamedevgirl84/LTX2.3_Enhancer1) - Video enhancement LoRA
  * [Enhancer2](https://huggingface.co/vrgamedevgirl84/LTX2.3_enhancer2) - Second video enhancement LoRA
* oumoumad
  * [IC luminance map](https://huggingface.co/oumoumad/ltx-2_IC_LUMIPARTICLES)
  * [LTX-2 IC-LoRA-Ungrade](https://huggingface.co/oumoumad/LTX-2-19b-IC-LoRA-Ungrade) - Removes color grading and contrast from footage, returning neutral ungraded appearance
  * [LTX-2.3 IC-LoRA-Ungrade](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Ungrade) - LTX-2.3 version of color grading removal IC-LoRA
  * [IC-LoRA-Outpaint](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Outpaint) - Extends video canvas by generating new content in black regions (letterbox areas), filling with temporally consistent content
  * [IC-LoRA-ReFocus](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-ReFocus) - Removes lens blur and restores focus to out-of-focus footage (lens blur only)
  * [IC-LoRA-Uncompress](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Uncompress) - Removes MP4 compression artifacts (blocking, banding, mosquito noise) and restores clean video
  * [IC-LoRA-MotionDeblur](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-MotionDeblur) - Removes motion blur from footage
  * [IC-LoRA-Deinterlace](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Deinterlace) - Removes interlacing artifacts from video
  * [FXIC LTX2 IC-LoRA](https://huggingface.co/oumoumad/fxic-ltx2-iclora) - Flux-inspired IC-LoRA for LTX video transformation with multiple optimizer variants (adamw, prodigy, masked) at various training steps
  * [DeArchive LTX-2.3](https://huggingface.co/oumoumad/ltx-2.3-dearchive-lora) - In-Context LoRA for restoring archive video (old B&W footage, low-res web rips, sepia-toned silent-era prints) into colored, high-definition modern cinematography (Rank 128, 5,000 steps)
* Kijai
  * [Realisdance](https://huggingface.co/Kijai/LTX2-IC-LoRAs/resolve/main/realisdance_ltx2.3_ic-lora_step_02000.safetensors) - IC-LoRA trained on the realisdance dance set (312 MB)
  * [SAM3D Body v42](https://huggingface.co/Kijai/LTX2-IC-LoRAs/resolve/main/ltx23_sam3dbody_v42_restarts-step00004000.comfy.safetensors) - IC-LoRA tied to SAM3D body pose conditioning (624 MB)
* Cseti
  * [IC-LoRA-Cameraman v1](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-Cameraman_v1) - Transfers camera movements (zoom, pan, tilt, orbit) from reference video to generated output
  * [IC-LoRA-EditRefVid v1](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-EditRefVid_v1) - Edit reference video IC-LoRA for editing existing videos using reference guidance
  * [IC-LoRA-Cameraman v2](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-Cameraman_v2) - v2 of the Cameraman IC-LoRA with a larger and more diverse dataset; replicates camera motion from a reference video. No trigger word required.
  * [IC-LoRA-CrossView Prompt v0.9](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-CrossView-Prompt) - Virtual second camera IC-LoRA: give it a reference video + a short camera-angle prompt using the trigger `crossview.` and re-render the same scene from a new viewpoint. v0.9 proof-of-concept trained on synthetic multi-view data; no starting image needed.
  * [IC-LoRA-CrossView Warp v0.9](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-CrossView-Warp) - Depth-warp novel-view IC-LoRA for LTX-Video 2.3 (22B). Given a video + a depth-warp of the same video (from the CrossViewWarp ComfyUI node, Depth Anything V2 input) and an azimuth/elevation/distance offset, renders the scene from that new viewpoint. Sibling of CrossView-Prompt v0.9. (192 MB)

* 100percentrobot
  * [Audio-Reactive LORA](https://huggingface.co/100percentrobot/LTX-2.3-Audio-Reactive-LORA) - Generates audio-reactive videos with motion synchronized to musical elements (beats, rhythm)
* LiconStudio
  * [VBVR-lora-I2V](https://huggingface.co/LiconStudio/Ltx2.3-VBVR-lora-I2V) - Enhances video generation for complex reasoning tasks including multi-object interactions, physical causality, and spatial relationships
  * [VBVR-lora-I2V Special](https://huggingface.co/LiconStudio/Ltx2.3-VBVR-lora-I2V)
  * [Licon MSR V2](https://huggingface.co/LiconStudio/LTX-2.3-Multiple-Subject-Reference) - Multiple Subject Reference v2: IC-LoRA preserving character identity / clothing / objects across frames in multi-reference video generation. Improves consistency, stability and scene logic vs. v1. Requires the [ComfyUI-Licon-MSR](https://github.com/liconstudio/ComfyUI-Licon-MSR) plugin.

* TheBurgstall
  * [LTX-2.3-Skin-Hair](https://huggingface.co/TheBurgstall/LTX-2.3-skin-hair) - Refines skin texture and hair rendering, reduces plastic skin artifacts, improves specular highlights 
  * [VR-360-Outpaint IC-LoRA](https://huggingface.co/TheBurgstall/VR-360-Outpaint-LTX2.3-IC-LoRA) - Outpaints standard widescreen footage into a full 360° equirectangular projection for immersive/VR viewing.
  * [Seamless-Equirectangular LTX-2.3 LoRA](https://huggingface.co/TheBurgstall/Seamless-Equirectangular-LTX2.3-LoRA) - Rank-128 LoRA for equirectangular 360° text-to-video generation with LTX-2.3 (15k steps). Trigger `Equirectangular`. Pairs with the [ComfyUI-Seamless-Equirectangular](https://github.com/Burgstall-labs/ComfyUI-Seamless-Equirectangular) node pack and EquiRoPE / Geometric CFG / per-step roll / circular VAE / wrapped noise setup.

* Nightfury16
  * [Staging IC-lora 512](https://huggingface.co/Nightfury16/ltx2.3-staging-ic-lora-512) - Staging IC-LoRA for video composition control (512 latent scale)
* siraxe
  * [MergeGreen IC-lora](https://huggingface.co/siraxe/MergeGreen_IC-lora_ltx2.3) - Maintains motion at start/end frames, use middle frames with RGB 0,191,0 (75% green fill) in IC-LoRA workflow
  * [TTM IC-lora](https://huggingface.co/siraxe/TTM_IC-lora_ltx2.3) - Makes cutouts cartoony and adds cartoony characters to video scenes, based on the TTM approach (use with Img To Video bypass + Add Video IC-LoRA Guide node)
* Lightricks LTX-2
  * [Canny Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Canny-Control) - Edge detection control for structural guidance
  * [Depth Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Depth-Control) - Depth map conditioning for 3D spatial control
  * [Detailer](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Detailer) - Enhances fine details and textures in generated videos
  * [Pose Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Pose-Control) - Human pose estimation control for motion guidance

**Upscaler LoRAs:**
* [LTX 2.3 Upscale IC-LoRA](https://huggingface.co/Zlikwid/LTX_2.3_Upscale_IC_Lora) by [Zlikwid](https://huggingface.co/Zlikwid)
  * Generative refinement LoRA for upscaling lower-res or soft videos
  * Works by bicubic upscaling first, then running through LTX 2.3 with this LoRA
  * Use prompt: `upscale`
* [LTX2.3-ICEdit-Insight](https://huggingface.co/joyfox/LTX2.3-ICEdit-Insight) by [JoyFox Lab](https://huggingface.co/joyfox)
  * Task-aware video restoration and editing model family
  * Supports: Video Restoration, HD Enhancement, Watermark Removal, Subtitle Removal
* [Singularity LTX-2.3 OmniCine](https://huggingface.co/WarmBloodAban/Singularity_LTX-2.3_OmniCine_Preview0.1) by [WarmBloodAban](https://huggingface.co/WarmBloodAban)
  * Comprehensive optimizer for LTX2.3 I2V and First/Last Frame workflows
  * Features: Limb Evolution, Shot Injection, Natural Expression, Physical Integrity, Cross-Style Potential
  * Uses "Singularity" prompting framework with 7-block bilingual structure
* yuvraj108c
  * [LTX-2.3-22b-IC-LoRA-Any-Trajectory-Instruction](https://huggingface.co/yuvraj108c/LTX-2.3-22b-IC-LoRA-Any-Trajectory-Instruction) - IC-LoRA porting Any Trajectory Instruction (ATI) to LTX-2.3; lets users draw motion paths on an input image and have the model generate videos following those trajectories (splines). Trained on 25 video pairs at 768x768x81 bucket size, 3000 steps.
* zghhui
  * [OmniNFT RL-LoRA](https://huggingface.co/zghhui/OmniNFT) - Modality-wise Omni Diffusion Negative-aware Fine-Tuning RL-LoRA for joint audio-video generation (paper arXiv:2605.12480). Provides both LTX-2 and LTX-2.3 variants.
  * [LTX-2.3-OmniNFT-RL-LoRA (Kijai mirror)](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/loras/LTX-2.3-OmniNFT-RL-Lora_bf16.safetensors) - Same OmniNFT RL-LoRA repackaged by Kijai in bf16 (588 MB).
* VetoBugger
  * [LTX2.3-CrispLora](https://huggingface.co/VetoBugger/LTX2.3-CrispLora) - Crisp enhancement LoRA for LTX-2.3 (`LTX2.3_Crisp_Enhance.safetensors`).
* SyFeee
  * [LTX-2.3 Dual-Character LoRA](https://huggingface.co/SyFeee/LTX2.3-Dual-Character-en) - Image-to-video character-consistency LoRA tuned for two-character dialogue scenes and multi-shot cinematic generation. Works for ancient Chinese fantasy, modern urban, and 3D anime styles. Recommended strength 0.7-0.9 standalone, 0.3-0.5 when stacked with style LoRAs.
* WarmBloodAban
  * [Singularity LTX-2.3 OmniCine V1](https://huggingface.co/WarmBloodAban/Singularity-LTX-2.3_OmniCine_V1) - Updated V1 of the OmniCine integrated optimization framework. Restructures LTX-Video 2.3 generation logic with focus on I2V, First/Last Frame, and Reference-to-Video workflows. Nearly 100,000 training steps. Includes `Singularity-LTX-2.3_OmniCine_V1.safetensors` (2.57 GB) and `Singularity-LTX-2.3_OmniCine_V1nsf.safetensors` (2.57 GB, NSF variant).

<a id="lora-styles"></a>

### ▣ Styles
* elismasilva
  * [Latin Dance](https://huggingface.co/elismasilva/LTX-2.3-LoRa-Latin-Dance/resolve/main/LTX-2.3-Latin%20dance.safetensors) - Latin dance motion/style LoRA for LTX-2.3 (rank ~128). (214 MB)
* OmerHagawa
  * [LTX2 UME PixelArt LoRA](https://huggingface.co/OmerHagawa/ltx2-ume-pixelart-lora) - Pixel art style LoRA for LTX-2
* Playtime-AI
  * [Commission LTX-2.3 MtF Transformation](https://huggingface.co/Playtime-AI/Commission_LTX-2.3-MtF_Transformation_v2.1) - MtF transformation style LoRA for LTX 2.3
* Andro0s
  * [Pixar Toon Style LoRA](https://huggingface.co/Andro0s/LTX_2.3_Pixar_Toon_Style_LoRa) - Pixar-style CGI toon cinematic look with trigger word `P1x4r`
* Cseti
  * [Arcane-Jinx v1](https://huggingface.co/Cseti/LTX2.3-22B_Arcane-Jinx_v1) - Style LoRA inspired by Arcane's Jinx character design
  * [ReStyle IC-LoRA](https://huggingface.co/Cseti/LTX2.3-22B_ReStyle_IC-LoRA) - Image-guided style transfer IC-LoRA that re-renders videos in a target style while preserving original content and motion
* lopho
  * [Gantz O v1.0.0](https://huggingface.co/lopho/ltx2-movie-loras) - Movie-style LoRA (654 MB, 10000 steps)
* bionicman69
  * [Arnold Style](https://huggingface.co/bionicman69/Arnold_LTX23) - Arnold Style LoRA for LTX 2.3. Get to the choppa!
  * [Star Trek TNG Style](https://huggingface.co/bionicman69/StarTrek_TNG_Style_LTX23) - Star Trek: The Next Generation style LoRA for LTX 2.3
* joeygambino
  * [Surfaces Realism](https://huggingface.co/joeygambino/ltx23-surfaces-realism-lora/resolve/main/ltx23_surfaces_v1.safetensors) - Materials/realism LoRA (rank 32, video branch) that kills the "plastic" look: cracked wet asphalt stays cracked and wet, concrete gets pores and rust streaks, floors scuff, wood grains show. No trigger word — trains as unconditional LoRA behavior. Load at 1.0 and write prompts normally. (336 MB)
* CoachBate
  * [Abercrom-ME](https://huggingface.co/CoachBate/ltx-2.3-22b-ic-lora-abercrom-me) - Vintage A&F Quarterly americana style-transfer IC-LoRA: transforms an input photo (subject + clothing + scene) into moody monochrome / sun-drenched beach / locker-room aesthetics with full styling makeover. Image-conditioned; pairs with the bundled `ABERCROM-ME IC-LoRA by coachbate-v3_20steps_3phase_3stage3.json` workflow. (384 MB, 2000 steps)
* ssjenforcer191
  * [Homelander](https://huggingface.co/ssjenforcer191/Homelander_LTX2.3) - Character IC-LoRA for The Boys' Homelander. Triggerword `HeroHomelander` (optionally append `wearing red leather gloves` / `dark blue cape and ornate red-and-gold collar`). Rank 64, 1500 steps, no regularization. Note: occasional letterbox black bars from training data. (~1.25 GB)
* oumoumad
  * [LTX-2-19b-LoRA-SPROUT](https://huggingface.co/oumoumad/LTX-2-19b-LoRA-SPROUT)
  * [Clay Stop Motion](https://huggingface.co/oumoumad/clay-stop-motion-lora-ngtvspc)
* kabachuha
  * [Hydraulic press](https://huggingface.co/kabachuha/ltx2-hydraulic-press)
  * [Cakeify](https://huggingface.co/kabachuha/ltx2-cakeify)
  * [Big Anime Breasts](https://huggingface.co/kabachuha/ltx2-big-anime-breasts)
  * [Eat](https://huggingface.co/kabachuha/ltx2-eat)
  * [Squish – One Hand Only](https://huggingface.co/kabachuha/ltx2-squish-one-hand)
  * [POP! Inflatable Animation](https://huggingface.co/kabachuha/ltx23-pop) - Comically inflate and pop cartoon/anime characters into confetti and fabric scraps (I2V focused)
* [CRT Animation Terminal](https://huggingface.co/lovis93/crt-animation-terminal-ltx-2.3-lora) by [lovis93](https://huggingface.co/lovis93) - Real late-80s/early-90s CRT monitor look with scanlines, phosphor glow, chromatic aberration, and dithering. Trigger word: `crtanim,`. Available in 4000 and 10000 training steps variants
* vrgamedevgirl84 Style LoRAs
  * [ClayMationStyle](https://huggingface.co/vrgamedevgirl84/LTX2.3_ClayMationStyle) - Clay animation style LoRA for LTX-2.3
  * [Wild West Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Wild_West_Style_LoRa)
  * [Paper Cut Out Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Paper_Cut_Out_Style_LoRa)
  * [Post Apocalyptic Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Post_Apocalyptic_Style_LoRa)
  * [Pixar Toon Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Pixar_Toon_Style_LoRa)
  * [Luxe Sensual Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Luxe_Sensual_Style_LoRa)
  * [Soft Enhance Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Soft_Enhance_Style_LoRa)
  * [Crisp Enhance Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Crisp_Enhance_Style_LoRa)
  * [Fantasy Puppet Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Puppet_Style_LoRa)
  * [Fantasy Realism Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Realism_Style_LoRa)
  * [Fantasy Painterly Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Painterly_Style_LoRa)
  * [Fantasy Anime Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Anime_Style_LoRa)
  * [Cozy Felt Style](https://huggingface.co/vrgamedevgirl84/LTX2.3_Cozy_Felt_Style_LoRa)
  * [Clay Mation Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Clay_Mation_Style_LoRa)
  * [90s Animation Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_90s_Animation_Style_LoRa)
* [Alissonerdx LTX-LoRAs Collection](https://huggingface.co/Alissonerdx/LTX-LoRAs) - Comprehensive collection including:
  * Anime2Half-Real - Converts anime-style content to half-realistic aesthetic (4500 steps, rank64)
  * Edit-Anything Global - Global editing LoRA variants (6000-9000 steps, rank128)
  * Inpaint Masked R2V/T2V - Region-based inpainting LoRAs for masked video editing
  * Real2Anime/Anime2Real - Style conversion LoRAs (rank64)
* Nebsh
  * [Outfit Switch](https://huggingface.co/Nebsh/LTX2_Outfitswitch)
  * [Handheld run](https://huggingface.co/Nebsh/LTX2_Handheld_run)
  * [Atomic Explosion](https://huggingface.co/Nebsh/LTX2_AtomicExplosion)
  * [HERO CAM](https://huggingface.co/Nebsh/LTX2_Herocam_Lora)
  * [Animatediff V1](https://huggingface.co/Nebsh/LTX2_Animatediff_style)
  * [PUSH TO GLASS](https://huggingface.co/Nebsh/LTX2_Pushtoglass)
  * [Object POV](https://huggingface.co/Nebsh/POVObject)
* [Squish](https://huggingface.co/ovi054/LTX-2-19b-Squish-LoRA)
* [Yoshiaki Kawajiri Retro Anime](https://huggingface.co/tarn59/Yoshiaki_Kawajiri_Retro_Anime_LTX2) - LoRA trained on Yoshiaki Kawajiri's distinctive retro anime art style
* Playtime-AI
  * [DonaldTrump](https://huggingface.co/Playtime-AI/LTX-2.DonaldTrump)
  * [Rick_and_Morty](https://huggingface.co/Playtime-AI/LTX-2.3-Rick_and_Morty-BETA) - BETA LoRA for Rick and Morty animated style
  * [LTX-2.3-Rick_And_Morty_v2](https://huggingface.co/Playtime-AI/LTX-2.3-Rick_And_Morty_v2) - Updated Rick and Morty v2 LoRA trained on the Smith and Rick Sanchez characters (undertrained; voices/clothing can be off; v3 in training)
  * [LTX-2.3-Wednesday_Addams](https://huggingface.co/Playtime-AI/LTX-2.3-Wednesday_Addams)
  * [LTX-2.3-Kermit_the_Frog](https://huggingface.co/Playtime-AI/LTX-2.3-Kermit_the_Frog)
  * [LTX-2.3-Jenna_Coleman](https://huggingface.co/Playtime-AI/LTX-2.3-Jenna_Coleman)
  * [LTX-2.3-Marge_Simpson](https://huggingface.co/Playtime-AI/LTX-2.3-Marge_Simpson) - Marge Simpson character LoRA trained on the base LTX-2.3 Dev model. Trigger words: `2d animation`, `Marge Simpson` (use `2d animation` to avoid getting 3D animation)
  * [LTX-2.3-Bender](https://huggingface.co/Playtime-AI/LTX-2.3-Bender) - Bender (Futurama) character LoRA. Trigger words: `2d animation`, `Bender the bending robot`
  * [LTX-2.3 Sulphur Gyrating Hips](https://huggingface.co/Playtime-AI/LTX-2.3_Sulphur-Gyrating_Hips) - Motion LoRA driven by the trigger `She thrusts her hips in a sexual manner`
* SOLRICKS
  * [LTX-2.3-Yesilcam-Turkish-Cinema](https://huggingface.co/SOLRICKS/LTX-2.3-Yesilcam-Turkish-Cinema) - Nostalgic Yeşilçam Turkish cinema visual style with warm cinematic tones and classic film atmosphere. Recommended strength 0.7.
  * [ltx-2-3-ue5-style-lora](https://huggingface.co/SOLRICKS/ltx-2-3-ue5-style-lora) - Unreal Engine 5 (UE5) cinematic style LoRA. Trigger word: `ue5_style`.
  * [Sci-Fi Cinema](https://huggingface.co/SOLRICKS/ltx-2.3-sci-fi-cinema) - a cinematic science-fiction style LoRA for LTXV / LTX-2.3. Trigger word: `srx_scifilm`.
  * [LTX-2.3 Product Ad Style](https://huggingface.co/SOLRICKS/ltx-2.3-product-ad-style) - Cinematic product-commercial style for luxury / cosmetics / tech / fashion ads. Trigger `srx_commercial`, recommended strength 0.85.
  * [LTX-2.3 The Art of Marbling](https://huggingface.co/SOLRICKS/ltx-2.3-the-art-of-marbling) - Marbling / ebru ink-flow style (paper, pigment, fluid art, Turkish ebru). Trigger `srx_ebrumotion`, recommended strength 0.85.
* SyFeee Chinese Drama Pack
  * [ltx2.3-chinese-drama-charlora](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-charlora) - Character LoRA trained on 78 episodes of Chinese historical drama; specialises base model for live-action, photoreal cinematic generation in Han dynasty / wuxia settings. Trigger words: `char_0_person` through `char_9_person`. Recommended strength 0.8–0.9.
  * [ltx2.3-chinese-drama-iclora-canny](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-iclora-canny) - IC-LoRA conditioning on Canny edge/line-art video; controls scene composition and architectural layout from reference outlines. Use with `char_0_person` for character reference.
  * [ltx2.3-chinese-drama-iclora-depth](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-iclora-depth) - IC-LoRA conditioning on monocular depth video (Depth-Anything-3); transfers 3D geometric structure from reference to generated video. Strong on interior scenes.
  * [ltx2.3-chinese-drama-iclora-pose](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-iclora-pose) - IC-LoRA conditioning on DWPose 133-keypoint skeleton render; transfers pose from reference video while preserving Chinese drama style. Stackable with character LoRA.
* mxturbo
  * [Formula1-Cockpit-T-Cam-LTX2.3](https://huggingface.co/mxturbo/Formula1-Cockpit-T-Cam-LTX2.3) - LoRA trained on 1.6L V6 Turbo Hybrid Era F1 T-Cam onboard footage. Generates cockpit/T-cam onboard video. Trigger: `16LV6HybridF1` (car type); follow the "T-cam onboard view..." / "AT-cam onboard view..." prompt style.
* chsengni
  * [ltx2.3-fpv-motion](https://huggingface.co/chsengni/ltx2.3-fpv-motion) - Smoother FPV (First Person View) camera movements and improved low-speed flight shots.
* EllaPriest45 — three large LTX-2.3 LoRA collections (NSFW / characters / styles); open each repo for the full file list
  * [LTX2.3_Actions](https://huggingface.co/EllaPriest45/LTX2.3_Actions) — **Huge collection of NSFW LoRAs** for LTX-2.3 (179 `.safetensors`, ~137 GB): explicit action / motion / pose LoRAs. Pairs with 10Eros / Sulphur-2.
  * [LTX2.3_Characters](https://huggingface.co/EllaPriest45/LTX2.3_Characters) — **Character LoRAs**: massive per-celebrity likeness collection for LTX-2.3 (394 `.safetensors`, ~130 GB; each `Name - LTX2.3.safetensors` ~327 MB).
  * [LTX2.3_Styles](https://huggingface.co/EllaPriest45/LTX2.3_Styles) — **Style LoRAs**: large visual-style collection for LTX-2.3 (35 `.safetensors`, ~20 GB): anime, claymation, cyberpunk, post-apocalyptic, cozy felt, and more.
* TheBurgstall
  * [LTX-2.3-Body-Positivity](https://huggingface.co/TheBurgstall/ltx-2.3-bodypositivity-lora)
  * [LTX-2.3-Googly-Eyes](https://huggingface.co/TheBurgstall/ltx-2.3-googlyeyes-lora)
* TheBurgstall (LTX-2)
  * [EarthZoomOut](https://huggingface.co/TheBurgstall/EarthZoomOut-LoRA-LTX-2-19b)
  * [GroupPhoto](https://huggingface.co/TheBurgstall/GroupPhoto-LoRA-LTX-2-19b)
  * [WHATUSEE](https://huggingface.co/TheBurgstall/WHATUSEE_LTX-2-19B_LoRA)
* [Black Venom](https://huggingface.co/siraxe/black_venom_ltx2)
* Levmar
  * [ltx2-lora](https://huggingface.co/Levmar/ltx2-lora) — Image-to-Video LoRA fine-tuned from `ltx-2.3-22b-dev.safetensors` with the LTX LoRA Trainer (6000 steps, LR 1e-4, batch 1). Two checkpoints: `lora_weights_step_02000.safetensors` and `lora_weights_step_06000.safetensors` (~428 MB each). License: other.
* Lightricks
  * [Camera Control: dolly-in](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-In/blob/main/ltx-2-19b-lora-camera-control-dolly-in.safetensors)
  * [Camera Control: dolly-left](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Left/blob/main/ltx-2-19b-lora-camera-control-dolly-left.safetensors)
  * [Camera Control: dolly-out](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Out/blob/main/ltx-2-19b-lora-camera-control-dolly-out.safetensors)
  * [Camera Control: dolly-right](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Right/blob/main/ltx-2-19b-lora-camera-control-dolly-right.safetensors)
  * [Camera Control: jib-down](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Jib-Down/blob/main/ltx-2-19b-lora-camera-control-jib-down.safetensors)
  * [Camera Control: jib-up](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Jib-Up/blob/main/ltx-2-19b-lora-camera-control-jib-up.safetensors)
  * [Camera Control: static](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Static/blob/main/ltx-2-19b-lora-camera-control-static.safetensors)
  * [Union-Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Union-Control/resolve/main/ltx-2-19b-ic-lora-union-control-ref0.5.safetensors)
* eraRelentless
  * [LTXreal](https://huggingface.co/eraRelentless/ltx23REALISM) - Realism stylization for LTX-2.3; trigger `realism`
* nnndite
  * [ltx2.3 Foot Model](https://huggingface.co/nnndite/ltx2.3foot) - Foot / lower-limb LoRA for LTX-2.3
* fal
  * [LTX-2.3 IC-LoRA — 3D Render to Photoreal](https://huggingface.co/fal/LTX-2.3-3DREAL-LoRA) - IC-LoRA turning rough 3D viewport / Blender blockouts into photoreal cinematic video while preserving composition and camera. Trigger `3DREAL`. v2 (`3DREAL-strong-v2`) is the newest and is also exposed on fal.ai as `render-to-real`.
* a3xrfgb
  * [Fable 5 — Vintage Style LoRA](https://huggingface.co/a3xrfgb/Fable5_Ltx2.3_vintage_style) - Vintage-style minimal-illustration / stop-motion / typography LoRA for LTX-2.3, used in the Fable 5 intro. Trained on a personal RTX 3090 (~5 hours).

<a id="lora-special"></a>

### ▣ Special

* [Wan2.1 VAE Adapter](https://huggingface.co/HDHCDev/Ltx2_2_Wan2.1_VAE_Adapter)
  * Latent space adapter for converting between LTX-2 and Wan2.1 VAE representations
  * `latent_adapter_final.pt` (447 MB)
* TenStrip
  * [LTX2.3 JoyAI LoRA Extracted](https://huggingface.co/TenStrip/LTX2.3_JoyAI_Lora_Extracted) - LoRA extracted from [jdopensource/JoyAI-Echo](https://huggingface.co/jdopensource/JoyAI-Echo); boosts prompt response and motion in LTX-2.3 (also used for NSFW/Sulphur/Eros) at strength 0.4–0.7.
  * [DMD LoRA (r256)](https://huggingface.co/TenStrip/LTX2.3_DMD_Lora/resolve/main/LTX2.3_DMD_reshaped_r256.safetensors) - DMD-distillation delta extraction from [JoyAI-Echo](https://huggingface.co/jdopensource/JoyAI-Echo), reshaped for rank-256 sampling. Use at 1.0 with 8/4-step upscale or experiment with other sigmas; any euler or LTX-compatible sampler. No custom loading needed. (4.86 GB)
  * [DMD LoRA Hybrid v1](https://huggingface.co/TenStrip/LTX2.3_DMD_Lora/resolve/main/LTX2.3_DMD_hybrid_v1.safetensors) - Hybrid DMD distillation: works inside blocks 0-25 to increase movement strength above the standalone DMD without letting the LTX distilled LoRA redraw or bring negative base-model tendencies. Improves movement smoothness and consistency. (4.86 GB)
  * [DMD LoRA Hybrid v2](https://huggingface.co/TenStrip/LTX2.3_DMD_Lora/resolve/main/LTX2.3_DMD_hybrid_v2.safetensors) - v2 of the hybrid DMD distillation. (4.86 GB)
* ltx-community
  * [ltx2-compile-keytest](https://huggingface.co/ltx-community/ltx2-compile-keytest) - IC-LoRA fine-tune from `ltx-2.3-22b-dev.safetensors` (300 training steps, batch size 1, LR 2e-4). Trained with the [LTX LoRA Trainer](https://huggingface.co/spaces/ltx-community/ltx2-lora-trainer).
* zzmicer
  * [Sax](https://huggingface.co/zzmicer/ltx2-sax-lora-noaudio/resolve/main/lora_weights_step_04000.safetensors) - Saxophone audio LoRA (video-only, no-audio conditioning) at 4000 steps. (403 MB)
  * [Violin (8s)](https://huggingface.co/zzmicer/ltx2-violin8s-lora/resolve/main/lora_weights_step_03000.safetensors) - Violin audio LoRA trained on 8-second clips at 3000 steps. (856 MB)
  * [Guitar](https://huggingface.co/zzmicer/ltx2.3-22b-guitar-lora/resolve/main/lora_weights_step_03000.safetensors) - Acoustic guitar audio LoRA at 3000 steps. (1.71 GB)
  * [DJ](https://huggingface.co/zzmicer/ltx2-dj-lora-lr5e4-rank128/resolve/main/lora_weights_step_01800.safetensors) - DJ/electronic-music audio LoRA (rank 128, LR 5e-4) at 1800 steps. (1.71 GB)
* Lightricks
  * [LTX-2.3-22b-LoRA-Foley-V2A](https://huggingface.co/Lightricks/LTX-2.3-22b-LoRA-Foley-V2A) - Official Lightricks Foley V2A (video-to-audio) LoRA for LTX-2.3. Generates realistic, visually-synced Foley sound effects from video. Rank ~small (216 MB); pairs with the workflow JSON in the repo (`ltx-2.3-foley-v2a.json`).
  * [LTX-2.3-22b-IC-LoRA-Clean-Plate](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Clean-Plate) - Official Lightricks Clean-Plate IC-LoRA. Removes people/objects from video frames for steady background plates. Rank 128 (312 MB); pairs with the `LTX-2.3_-_V2V_mass_remove_people_Clean-Plate-Lora.json` workflow.
  * [LTX-2.3-22b-IC-LoRA-Relight](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Relight/resolve/main/ltx-2.3-22b-ic-lora-relight-1.0.safetensors) - Official Lightricks Relight IC-LoRA (single-stage, distilled). Relights a scene using a reference sphere image that defines the target lighting direction and color. Pairs with the bundled `LTX-2.3_Relight_ICLoRA_SingleStage_Distilled.json` workflow. (312 MB)
  * [LTX-2.3-22b-IC-LoRA-Cross-Eyed](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Cross-Eyed/resolve/main/ltx-2.3-22b-ic-lora-cross-eyed-0.9.safetensors) - Official Lightricks Cross-Eyed IC-LoRA v0.9. Converts standard video into side-by-side 3D stereo output (cross-eyed viewing). (327 MB)
  * [LTX-2.3-22b-IC-LoRA-Colorization](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Colorization/resolve/main/ltx-2.3-22b-ic-lora-colorization-0.9.safetensors) - Official Lightricks Colorization IC-LoRA v0.9. Adds realistic color to B&W or desaturated input video. (906 MB)
  * [LTX-2.3-22b-IC-LoRA-Deblur](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Deblur/resolve/main/ltx-2.3-22b-ic-lora-deblur-0.9.safetensors) - Official Lightricks Deblur IC-LoRA v0.9. Removes blur and restores sharp, focused video. (906 MB)
  * [LTX-2.3-22b-IC-LoRA-Decompression](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Decompression/resolve/main/ltx-2.3-22b-ic-lora-decompression-0.9.safetensors) - Official Lightricks Decompression IC-LoRA v0.9. Removes MP4 compression artifacts (banding, mosquito noise) and restores clean video. (906 MB)
  * [LTX-2.3-22b-IC-LoRA-Water-Simulation](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Water-Simulation/resolve/main/ltx-2.3-22b-ic-lora-water-simulation-0.9.safetensors) - Official Lightricks Water-Simulation IC-LoRA v0.9. Adds physically-plausible fluid/water dynamics to reference video (reflections, ripples, splashes). (906 MB)
  * [LTX-2.3-22b-IC-LoRA-Instant-Shave](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Instant-Shave/resolve/main/ltx-2.3-22b-ic-lora-instant-shave-0.9.safetensors) - Official Lightricks Instant-Shave IC-LoRA v0.9. Removes facial hair in video-to-video. (654 MB)
  * [LTX-2.3-22b-IC-LoRA-In-Outpainting](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-In-Outpainting/resolve/main/ltx-2.3-22b-ic-lora-in-outpainting-0.9.safetensors) - Official Lightricks In-Outpainting IC-LoRA v0.9. Extends canvas in any direction from reference video, filling new regions with consistent scene content. (1.31 GB)
  * [LTX-2.3-22b-IC-LoRA-Day-To-Night](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Day-To-Night/resolve/main/ltx-2.3-22b-ic-lora-day-to-night-0.9.safetensors) - Official Lightricks Day-To-Night IC-LoRA v0.9. Converts daytime footage to nighttime with matched lighting/shadows. (327 MB)
* fbjr
  * [LTX-2.3-22b-IC-LoRA-Audio-Only-Context](https://huggingface.co/fbjr/LTX-2.3-22b-IC-LoRA-Audio-Only-Context) - Two IC-LoRA checkpoints for audio-only and cross-modal audio-video context conditioning on LTX-2.3. Audio-only checkpoint (156 MB, `audio_only_step_01000.safetensors`) preserves a reference audio identity through a generation pass; cross-modal checkpoint (276 MB, `cross_modal_step_01000.safetensors`) extends that to joint audio-video conditioning.
* FuzzPuppy
  * [LTX-2.3 Foley](https://huggingface.co/FuzzPuppy/LTX-2.3-Foley-LoRA) - Video-to-audio LoRA for LTX-2.3 that adds realistic, visually synchronized Foley / sound effects over a video (multiplier 1.0–3.0; pairs with the LTX Community License).
  * [Black Magic](https://huggingface.co/FuzzPuppy/LTX-2.3-Black-Magic-LoRA/resolve/main/black-magic-ic-lora-450.safetensors) - Video-to-video IC-LoRA for low-light / shadow reconstruction. Restores underexposed footage to natural, well-exposed video with realistic colors and recovered shadow detail. Pairs with the bundled `ltx23-black-magic-lora-workflow.json`. (312 MB)
* Hoffm4nz
  * [LTX-2.3-22b-IC-LoRA-Golden-Hour](https://huggingface.co/Hoffm4nz/LTX-2.3-22b-IC-LoRA-Golden-Hour) - IC-LoRA fine-tune that biases generation toward warm "Golden Hour" lighting aesthetics. Root canonical checkpoint `ltx-2.3-22b-ic-lora-golden-hour.safetensors` (312 MB); four per-step snapshots are also available in the `checkpoints/` folder of the repo (step_00250 → step_01000, 312 MB each).
* JanKanta
  * [LensRemover](https://huggingface.co/JanKanta/ltx-2.3-22b-ic-lora-lens_remover/resolve/main/lens-eraiser-ltx23-ic-lora.safetensors) - Video-to-video IC-LoRA that removes lens flares, veiling glare, lens dirt, and other optical artifacts from footage while keeping the underlying scene intact. Dual-encoding: works on both sRGB/Rec.709 and ARRI LogC3 inputs (selected via trigger word). Pairs with the bundled `LensRemover_comfyui_workflow.json`. (312 MB)

* vpakarinen
  * [Motion Stabilizer for LTX-2.3](https://huggingface.co/vpakarinen/motion-stabilizer-ltx-23) - Motion LoRA stabilises body movement and rotation in LTX-2.3.
* Comfy-Org
  * [ltx-2.3-22b-ic-lora-ingredients-0.9](https://huggingface.co/Comfy-Org/ltx-2.3/resolve/main/split_files/loras/ltx-2.3-22b-ic-lora-ingredients-0.9.safetensors) - Comfy-Org-distributed ingredients IC-LoRA for LTX-2.3 (the other three siblings in the same folder — `id-lora-celebvhq-3k`, `id-lora-talkvid-3k`, `distilled_1.1_lora_dynamic_fro09_avg_rank_111_bf16` — are already linked from the Checkpoints / ID-LoRA tables).
* linoyts
  * [ltx2.3-ic-lora-ingredients-multishot](https://huggingface.co/linoyts/ltx2.3-ic-lora-ingredients-multishot) - IC-LoRA fine-tune from `ltx-2.3-22b-dev.safetensors` (2,500 training steps, LR 1e-4). Trained for multi-shot ingredient-conditioned generation.
  * [ltx2-ic-lora-ui](https://huggingface.co/linoyts/ltx2-ic-lora-ui) - LoRA fine-tune from `ltx-2.3-22b-dev.safetensors` (20 training steps; treats UI-screen aesthetics). Inherits LTX-2.3 base license.
* rzgar
  * [Motion Enhancer (N54W)](https://huggingface.co/rzgar/LTX-2.3-Motion-Enhancer-n4w/resolve/main/LTX-2.3-Motion-Enhancer-n4w.safetensors) - General-purpose N54W motion enhancer LoRA. Enhances fluidity, coherence, and motion when stacked as a companion LoRA alongside other specialized models. Extensively tested with top-rated Civitai LoRAs. (2.17 GB)
  * [Distilled LoRA 384-1.1 "n4w"](https://huggingface.co/rzgar/ltx-2.3-22b-distilled-lora-384-1.1-n4w) — Modified official 384-1.1 distilled LoRA that *cooperates* with N54W LoRAs (instead of fighting them), improving motion and appearance. Two variants: full rank ~7.08 GB (`ltx-2.3-22b-distilled-lora-384-1.1_n4w.safetensors`) and low-VRAM rank-128 ~2.40 GB (`ltx-2.3-22b-distilled-lora-384-1.1_rank_128_n4w.safetensors`). Use at strength 0.5–0.65 stacked with your N54W LoRA. Apache-2.0.
* joeygambino
  * [American Accent (audio)](https://huggingface.co/joeygambino/ltx23-accent-american-audio-lora/resolve/main/ltx23_accent_american_v2_rank32.safetensors) - Audio-branch LoRA (rank 32) that makes accent wording in prompts actually work. LTX-2.3's voice prior ignores accent requests in certain regions (e.g. young female characters default to Australian); this LoRA turns accent prompts into reliable control. **Requires 24 fps** — off-24 fps overrides accent wording entirely. (168 MB)


<a id="lora-id-lora"></a>

### ▣ ID-LoRA (Identity-Driven In-Context LoRA)

**ID-LoRA** is a method that enables identity-preserving audio-video generation in a single model. It jointly generates a subject's appearance and voice, letting a text prompt, a reference image, and a short audio clip govern both modalities together. Built on top of LTX-2.3 (22B), it is the **first method to personalize visual appearance and voice within a single generative pass**.

Unlike cascaded pipelines that treat audio and video separately, ID-LoRA operates in a **unified latent space** where a single text prompt can simultaneously dictate the scene's visual content, environmental acoustics, and speaking style—while preserving the subject's vocal identity and visual likeness.

**Key Features:**
- Text prompt controls the scene and content
- Reference image preserves the subject's visual likeness
- Short audio clip preserves the subject's vocal identity
- Single unified generation pass for both appearance and voice

**Available LoRAs for LTX-2.3:**

| LoRA | LoRA Rank | Size | Download |
|:---|:---|:---:|:---|
| ID-LoRA-TalkVid-3K | 128 | 1.1 GB | [![][gh-AviadDahan]](https://huggingface.co/AviadDahan/LTX-2.3-ID-LoRA-TalkVid-3K) ┊ [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2.3/resolve/main/split_files/loras/ltx-2.3-id-lora-talkvid-3k.safetensors) |
| ID-LoRA-CelebVHQ-3K | 128 | 1.1 GB | [![][gh-AviadDahan]](https://huggingface.co/AviadDahan/LTX-2.3-ID-LoRA-CelebVHQ-3K) ┊ [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2.3/resolve/main/split_files/loras/ltx-2.3-id-lora-celebvhq-3k.safetensors) |

**Resources:**
- [Project Page](https://id-lora.github.io/) | [GitHub](https://github.com/ID-LoRA/ID-LoRA) | [Paper (arXiv: 2603.10256)](https://arxiv.org/abs/2603.10256)

