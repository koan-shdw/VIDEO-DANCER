# Video Dancer AI Manual

> **Instructions for the AI reading this document:** You are now the living manual for
> **Video Dancer**, a local-first desktop editor for AI-generated video. Answer the user's
> questions about the app using ONLY the information in this document. Walk users through tasks
> step by step, naming the exact panels, buttons, and keys written here. If something isn't
> covered in this document, say so plainly instead of guessing. Keep answers short and concrete;
> expand only when the user asks. The user may be mid-task inside the app. Prefer "click X,
> then Y" over theory.

*Covers Video Dancer v0.36.2 (2026-11-04).*

## New in 0.36.2

- Nothing in the app changed: this is 0.36.1 with a release check behind it. The window tests that guard the installer now run before every tag.

## New in 0.36.1

- Deletes go to the Recycle Bin: Cleanup, a mood, a LoRA on the shelf, a reverted guide. A delete of paid or hand work asks first: a clip, a selection, a score or a voice with takes, a subtitle with lines, a workspace nothing brings back.
- One gesture, one undo step: Q / W, the end trim, ripple delete, gap close, Ctrl+K and the speed ripple move the pictures, the free audio, the scores and the SUB blocks together, honouring the locks. What a job brought in is never an undo step: it survives Ctrl+Z.
- The razor stays armed until V or Esc. Ctrl+K cuts every unlocked block under the playhead in one go. A subtitle line saves when you leave the field or press Enter.
- Esc closes the top layer only: a dialog, a dropdown, a menu, a popover, the Room. Every dropdown is the house dropdown now, and a greyed control shows its reason when you point at it.
- Nothing fails silently: an action that stops shows a toast naming the action and the reason, and its busy mark clears. Recovery, project and compose messages reach you as toasts too.
- What the Monitor plays is what renders: fades, a reversed block’s sound and music levels land at the same second in a range export as in the full one. The export honours the SUB track’s eye and draws subtitles at the Monitor’s size.
- Listen and Make: ✕ cancels the job, progress shows in the panel, your typed text wins over the translation, and a project switch mid-job saves nothing into the other project.
- Every form saves when the window closes or the app quits; a quit while local work runs asks first. A load never saves. A render from a form you have not committed makes its clip first, so two renders are two clips.
- The last session’s queued rows come back as a Queue row per project, with re-queue and forget, and wait for your word.
- Accepted means persisted: a job a supplier took is on disk before anything else, so a crash never loses it or pays for it twice. Recovery lands a download already on disk without fetching it again.
- Results land in the project that asked: a render, a card, an enhance or a Co-Director write that finishes after you switched projects goes to its own project, on its next open. A render with no project open refuses. New Project says why when it cannot create. A project whose folder moved gets a pick-the-folder-again door.
- Saves land in place, never half-written, and a file that cannot be read is never written over as empty. Deleting a card version keeps its files and scrubs every clip’s references.
- Local engines: the Dancer apps share one GPU turn, and a caller waits instead of seeing busy in another Dancer app. ⏻ free GPU stops the idle workers and names the busy one.
- Updates: a quit never installs; the chip asks before the restart. Electron 44.9.3. The 80s dark fantasy mood no longer ships.
- Colour: apply match stops with a word if the block, the project or the reference moved under it, and a reference that could not be drawn says why. The Timeline Monitor’s right buttons fold at narrow widths.
- LoRAs: one chip in Clip Gen and Image Gen; a same-name drop lands beside as name (2), or says the file is already on the shelf.
- The README and the manual say what the app does today: the keys, Seedance 2.5, the Queue row at quit, the Claude Code login under Settings → Connections.

## New in 0.36.0

- Listen fills the second language by itself: once the dialogue is heard, the other language is translated line by line, times kept. Lines that already have text stay as they are. If the translation fails, the lines stay empty and one line says why.
- Translate: a row under the languages picks the model that translates, from every engine you have connected. It starts on your Co-Director’s. Make uses it too.
- Codi reads a subtitle and writes its lines in either language, times kept. One Ctrl+Z undoes it.
- The Subtitle panel’s sections fold: click a title or its arrow.
- On a Mac, Codi’s shell runs sh, and its tool log says sh>.
- Colour: Premiere’s Lumetri Color in its own panel. Right-click a block → colour…, or Window → Colour. Basic correction, creative, curves, colour wheels, hsl secondary and vignette, in Premiere’s order with Premiere’s ranges.
- Input LUTs and looks: pick a .cube file, or browse… to copy one into the LUT folder. The look preview steps through the looks on the Monitor’s frame; a click applies the one shown.
- Fourteen looks come with the app: five film stocks and nine styles, first in the Look dropdown under video dancer, above your own. Delete one and it stays gone.
- Eyedroppers: white balance, the hsl key and the hue curves take their colour from a spot you click in the Timeline Monitor.
- Scopes: Window → Scopes shows the histogram of the Timeline Monitor’s picture, red, green, blue and luma, and follows every grade change.
- Auto in basic correction sets temperature, tint, exposure, contrast, highlights, shadows, whites, blacks and saturation from the frame. Intensity scales them.
- Comparison view: ◧ on the Timeline Monitor shows a reference frame beside the live picture, or split across it. Drag the line, swap the sides, and move the reference by cut, by the scrub bar, or to this frame. The reference starts without the grade open in the Colour panel. Apply to reference holds that grade on it while the live picture takes your next changes, and ↺ takes it off.
- Apply match sets the colour wheels and saturation so the block matches the reference frame. Face detection, ticked by default, finds the faces in both frames and counts them more in the match. The first match with it downloads the face model (~230 KB, in the Models card).
- The Colour panel’s ≡ menu: copy grade and paste grade, save preset… and apply preset, and export .cube…, which writes the grade into the LUT folder. Sharpen, hsl secondary and vignette stay out of the .cube: a LUT cannot hold them.
- Slider values type: click the number, type, Enter. In the Effects panel too.
- A storyboard still in an export is the right way up and carries its block’s effects.

## New in 0.35.0

- Build card on a character plate: the front, side, back and face side by side, with the char sheet printed beside them: name, character, features, voice. One 21:9 picture the model reads.
- The card becomes the char sheet’s picture. If the char sheet is empty, it opens instead and Codi fills it in from the picture. Press build card again when it is done.
- Scene plates turn on one spot: east, north, west, south. ▤ build sheet makes the compass plate, each view labelled FACING EAST, NORTH, WEST or SOUTH. Scene plates made before keep their five views.
- Send the compass plate with previs cards and the prompt names the view behind each card. The studio floor shows N, E, S and W in the work views, with the grid.
- Previs cards keep each card’s time and camera line. Before a render, the preflight says when the cards and the beats disagree. Redraw an older set to add them.
- Codi runs PowerShell in your project folder, with a time limit. Every command shows in its tool log; click it to see what came back. Stop ends it.

## New in 0.34.0

- Subtitles: their own tab in the Bin. Make one, rename it, copy it, put it in folders.
- The SUB track above the video rows: drop a subtitle on a clip and it covers that clip. Drag to move, pull the edges to trim, the lines show inside the block.
- The Subtitle panel: two languages, a style card for each (font, size, colour, outline), top or bottom, the second above or below, and every line with its times. The Timeline Monitor shows them live.
- Listen: ElevenLabs Scribe, Gemini or Whisper on fal hears the dialogue under the block and writes the lines with their times. Each model shows its price. Listen to the new part hears only what changed.
- Make: the spoken language gets what was heard, any other is translated line by line through your Co-Director, times kept.
- Export: subtitles burn in, as .srt files beside the video named after it, or off.

## New in 0.33.0

- Bin and Library tabs: one row of tabs with a count on each replaces the folding sections. Click a tab to open it, Ctrl-click to add or drop one, Shift-click to open every tab between.
- Open tabs share one scroll, each under its own heading with its + button. Drag a tab to move it. Each panel remembers the tabs you left open.

## New in 0.32.0

- Codi, rebuilt: eight new guides written from scratch. It pitches ideas, directs camera and action, builds previs, catches misreads before you pay, and learns from your corrections.
- Codi’s replies read properly: bold, lists, tables, headings and code boxes with a copy button, in the panel, the Room and the tether. Its tool log groups each tool with a count, refusals in red.
- Seedance renders send the prompt in Chinese. Clip Gen’s generated box has EN and 中 tabs to see what goes out, and a switch to turn it off.
- Cold read: before a render Codi reads the prompt fresh and flags what the model could get wrong. Its switch sits beside the renders switch.
- Codi switches moods on and off, keeps a log of your corrections and reviews it with you when you ask. A run that runs out of time keeps its work.
- Previs cards: a posed still for each camera, on pages of up to six, sent as storyboard pages. Clip Gen’s CARDS row keeps every version and sends the newest.
- Stand-ins from a character sheet, figures in colour, and a panel key that tells the model who is who.
- The PREVIS studio, finished: one tool row, a strip on the timeline’s grammar, a side bar for elements, cameras and shots, an inspector with a keyframe list, and Tab to search in a view.
- Export a previs as an animatic, storyboard sheets or a shot list. Coverage adds a master, two singles and two overs on two subjects in one go.
- Names in a view: every one, or only the selected. A switch on the names row of the overlay list.
- Camera only: a roof you can work under. A wireframe in the work views, solid on camera, in the bake and on the cards.
- ◧ compare in Clip Gen: drag a line across a take to set the previs it was sent against the render.
- Codi lays a previs on the PREVIS track under its clip, and clips made after a previs show by name and length on the timeline again.

## New in 0.31.0

- PREVIS: block a shot in grey 3D before you spend a gen. Stand-in actors, real cameras, keys on one clock, shots and multicam cuts; the gen paints the look.
- Previs is its own kind, with its own section in the Bin. Make one there, then drag the whole previs onto the timeline as one block, or drag a single shot out.
- Double-click a previs block and the studio opens at that moment.
- The Timeline Monitor plays a previs block live from its scene, and an empty clip shows its previs underneath, in the Monitor and in export.
- A Clip Gen over a previs offers that slice as its video ref: “previs available” adds it in one click, or the VID row’s ＋ previs box picks any previs. The previs sets the clip’s length and shape.
- The studio: views on the left with the shot camera inset, the outliner over the inspector, and the strip with the playhead, shots and keys always there.
- Panes you arrange: split, join, swap and resize them, give any pane any view, save your own layouts and set one as default.
- Edit keys on the strip (move, copy, delete), drag a path’s points, drag an actor’s body in the perspective view, and ghost with a key.
- Shots keep the take grammar: flag, colour, disable. The padlock stops every way of moving the shot camera.
- Keys help: press ? for the shortcuts card over the views.
- The Co-Director reads and edits a previs scene with you.
- Send to project carries a previs; export and gens wait for shots still baking.
- Timeline: double-click a kind’s track header to fold it into one lane.
- Video Dancer has its own licence now: free for all creators, for any project, commercial work included.

## New in 0.30.0

- MiniMax H3 local: veda in the attention pick, about 2.6× faster than off, with its five settings under it. Sage stays the near-exact everyday pick; off is for hero shots and fast action.
- Turbo 3-step for H3: a one-pass draft, about 3 minutes for a 15 s clip, to check a prompt and refs. Off renders the full pipeline as before.
- H3 reference videos send their own sound too, and a ref size pick: max for the best likeness, match for speed.
- H3 video VAE pick: fp16, or int8 at half the size for 16 GB cards. 720p renders at H3’s trained size, 1344×768.
- Models card: two new H3 rows, turbo 3-step and video vae int8. Veda joins the speed kernels row: click it once more to add it.
- The Co-Director knows every H3 dial, reads them on the clip and sets them for you.
- The local engine moves to a newer ComfyUI by itself the first time it starts.
- Effects: a flipping section under transform, horizontal and vertical on or off, like Premiere.
- Effects hold on the Timeline Monitor while you scrub and seek, with no flicker.

## New in 0.29.0

- Krea 3 in the Image Editor, on fal: your image plus up to 7 refs, 2K or 1K. The prompt names them `<image-1>`, `<image-2>` and on, and the line under the prompt shows which is which.
- A rewrite switch for Krea 3: on, Krea rewrites your prompt before it draws (its default); off, it uses your words exactly.

## New in 0.28.1

- Video Dancer is free: shdw.work has the downloads.
- Right-click a Library image, make image: a new Image Gen card opens, filled from the image’s own recipe, its PNG settings or its Image Editor prompt. With none, the Co-Director offers to write the prompt and aspect, and a yes writes them straight into the card.

## New in 0.28.0

- Image Editor crop works like Photoshop: drag an edge or a corner to move that side (Shift keeps the shape), drag inside to move the box, scroll to zoom. Enter crops to exactly the box.
- Nano Banana 2.1 in the Image Editor, on fal, Google, Venice and your Runway login, with its thinking dial (high by default).
- A ★ is only ever your flag, set with ~ or right-click. A render that lands is never starred, and the Co-Director flags a take only when you ask it to.
- The Clip Monitor’s play button and the space bar play again.
- Both monitors’ button rows wrap on a narrow panel instead of piling up.
- Video Dancer opens without freezing: the window resizes and redraws right away, not about 10 seconds later.
- Effects show in the Timeline Monitor, in exports and in transition previews.
- Depth and subject matte passes from the Effects panel work.
- Clean up unused media lives in Settings > General. The Project button is gone from the top bar.
- Cleanup deletes only the files it showed you, and nothing if the project changed in between.
- Video Editor and Image Editor share Image Gen’s layout: the picture big on top, the Model and Prompt cards under it, Generate and Queue at the bottom with the cost, and the take tree in a sidebar.
- Video Editor re-gens run on your Higgsfield Bridge login with Seedance 2 and 2.5.
- Each Queue row shows only its own progress.
- Image Editor pictures load again and fill the preview with no black bars.
- Image Gen’s Civitai LoRA tab opens on your favorites, and a LoRA download with no folder picked lands in the app’s LoRA library.

## New in 0.27.0

- Image Gen renders show in the Queue with their progress, and ✕ there stops one, like every other render.
- A render the supplier already took is never sent a second time, and ✕ while a job still uploads stops it before anything is spent.
- Spend is counted once, in the project that ran the job: Co-Director plan jobs, recovered renders and Sheet Gen included.
- Video Editor jobs and clip edits come back after a quit or a crash, like renders do.
- Ctrl+Z never takes a finished render away, switching timelines is not an undo step, and deleted results keep their files until Cleanup, so undo brings them back.
- Forms keep what you type: a quick switch saves it, a render landing never wipes it, and ↩ load recipe brings back the seed and links too.
- Timeline: quick nudges all land, a cut gives each half its own volume line and fades, and trimming a block’s start keeps its linked sound in sync.
- Timeline keys and Ctrl+V act only while the timeline is the panel you are in.
- Local engines: ✕ on a job waiting for the GPU stops it, adding a LoRA folder or deleting a model never kills a running render, and a second launch just brings the app to the front.
- Refs named @image1, @image2 in any order keep each name on its own picture.
- Each Bridge login keeps its own uploads, and a Bridge result is never your own ref coming back.
- Watched “send both” puts both LoRAs into Image Gen at their weights, and Get + Use picks the right LoRA version.
- A MOOD is never written over without asking you first.
- If saves start failing (a renamed folder, a full disk), closing asks whether to reopen the window or quit, and Video Dancer always opens again.
- Settings, spend, rules and guides are never replaced by an empty file when one can’t be read.
- A duplicated project starts without the original’s queue, plan or recovery entries.
- Exports use one frame rate for the effects and the cut, and no longer flash console windows.

## New in 0.26.0

- Settings has five pages: Connections, Co-Director, Watch, Appearance and General. Connections holds every API key and login in one place, each checked when you save it.
- The Co-Director can run on an OpenAI API key (GPT-6.1 Sol), billed per token.
- Claude Code and Codex sign in to their own Video Dancer profiles, so the app never touches your other Claude or ChatGPT logins.
- The Project button opens project controls: clean up media files nothing in the project or its undo history uses, after it shows how many and how big.
- The workspace button in the top bar is the same height as the buttons around it.
- Start a project and New project: the buttons match the close button and the toolbar.
- Image Gen takes in a project you moved find their pictures again, with their prompts, seeds and keepers.
- Ask the Co-Director to queue saved clips and it queues them. It makes a plan only when you ask for one, and there is no 20 render limit on a go.
- A Co-Director plan works one task at a time from its saved progress and survives an interrupted reply. GO picks a blocked plan back up within what you approved.
- Each finished result wakes the Co-Director once. A provider out of quota or signed out pauses the plan instead of counting as done.
- Stop plan sits on the right, works on a draft plan too, and a stopped plan leaves the panels.
- Saves ride out Dropbox and other sync apps briefly locking a file.
- Adding a Higgsfield login in the Bridge signs the browser out first, so you can pick the account with Google.

## New in 0.25.0

- One GO can cover a saved Co-Director plan. Review the work, models, settings, counts and costs, switch renders on and send GO.
- Completed jobs ping Co-Director across Image Gen, clips, image and video edits, scores, voice, Enhance and other result-producing operations. Each notification carries the results and saved progress.
- Co-Director uses its existing tools to inspect results before choosing what to do next or writing dependent prompts, then continues within the approved plan.
- The plan display shows progress, results and failures. Stop plan cancels queued work, requests cancellation of running jobs and keeps completed files. Switching renders off holds further dispatch and continuation.
- Job records and plan progress survive a restart. Unknown or interrupted submissions are reported without automatically repeating them. A confirmed failure can retry once within the approved allowance; a second failure blocks the plan.
- Civitai thumbnails stay cached on disk and are reused across views and app restarts.

Automated protocol, UI and regression tests, TypeScript and the production build pass. A real
Co-Director exchange continuing after real renders remains unverified.

## New in 0.24.0

- Image Gen’s queue keeps the prompt and settings each render had when you queued it. Change the prompt, loras or anything else and queue again as often as you like while one renders.
- The Co-Director can line up many prompts on one image gen in one go: ask for 20 variations, say go, and they render one after another on that gen. Your own prompt stays as it was.
- The Co-Director sees the prompt and settings behind every take of an image gen (loras and weights, unleashed, size, refs) and can look at each picture.
- The Co-Director sees your take marks: every ★, colour and disabled take, in clips, image gens, scores and voices. Delete a take and the marks stay on the right ones.
- The Co-Director reads a lora’s examples from Civitai, with their prompts and pictures. Ask for “the samurai ones” and remake them, with or without changes.
- Press ~ on a picture in Watched or in a lora’s examples to tag it for the Co-Director: it sees every tagged picture and its prompt with each message. ~ again untags.
- Watched and lora example tiles select like takes: click, Ctrl-click, Shift-click and the arrows. The prompt and loras menu is on right-click.
- A click on a take selects it and shows it, and never makes it a keeper. Only ~ or right-click → ★ keeper do. Every takes row works this way.
- Pick where models are downloaded: change in the Models card. It applies on the next start.

## New in 0.23.1

- The Mac installer is back.
- ENHANCE with Topaz on your PC no longer stalls when the copy is done first.

## New in 0.23.0

- Sound fx live on the audio tracks. Drop one on an A track and it lands there; on a video or score track it goes to the first free A track. A pink block, hatched until it is rendered. Click it to open it in the SFX card.
- Sonilo makes the sound of the footage under the sound fx block.
- Sound fx have their own card in the Bin with their own folders. Drag them onto the timeline from there, or a take straight out of the SFX card.
- Projects with sound fx on score tracks move them to audio tracks when they open. The music stays on the score tracks.
- The speed line works with the Pen too: a drag changes the speed, a click adds a keyframe.
- Switched-on buttons keep their words readable: the renders switch, tether, run now in the Queue and the rest.
- The thinking level sits on the same line as the model in Settings.
- Share a MOOD to the community without setting your name first. It asks once.
- MOOD names are outlines until you switch them on. + new, add, share and community stay filled.
- The guide file buttons in Settings line up on the right.
- A render fal refuses to hand back stops being retried.

## New in 0.22.0

- Nest a selection. Right-click selected clips and nest them: they move into a new timeline in the Bin, and one block plays it in their place, with its own speed, effects, dissolve and level.
- Score tracks. Scores sit on their own S tracks under the audio, each with mute, solo and lock, and they are orange so they stand apart.
- Keys 1 to 9 hide or show a video track and its audio track together.
- Timelines open as tabs. Drag a tab out and it becomes its own timeline panel; clicking a timeline panel gives it the keys and the Monitor.
- Clip Speed / Duration, the Premiere way. Right-click a block or press Ctrl+R: speed and duration chained, reverse, and keep pitch.
- Time remapping. Right-click a block, time remapping, speed: a speed line on the block. Drag it for slow motion or speed-up, Ctrl-click to add a keyframe, pull a keyframe apart for a ramp. Its sound plays at normal speed.
- J, K and L shuttle like Premiere. J plays backward, L forward, and each press goes faster, up to 8×. K stops.
- The ruler stays at the top while the tracks scroll.
- A score sets the timeline length when it runs past the video, or when it is on its own.
- Copy, cut and paste work right after you click a block.
- A duplicated timeline keeps everything: scores, markers, tracks, locks and export settings.
- Audio keyframes: P is the Pen (click the line for a keyframe, box-select keyframes), V is Selection, double-click goes back to 0 dB, Ctrl-click switches a keyframe between Linear and Auto Bezier.
- Export several timelines at once. Select them in the Bin, right-click, export. Settings can set one export folder for every export.
- Right-click the timeline over a score, create beat in score: a blank beat lands at that second and the Score card opens on it.
- ENHANCE (Window, Enhance, or right-click a take, block or video): interpolate and upscale with Topaz on your PC, RIFE, Real-ESRGAN or fal, compared before and after on a slide bar. The result is a new copy with a coloured outline; the original stays.
- Make a depth video. Right-click a video, take or block: a grey depth map lands in the Library, ready for your @video refs.
- Keepers are flags. Flag several takes in a set as keepers, and unflag them again.
- Shift-click selects a run of folders.
- GPT Image 2.5 in Image Edit, with a background pick: auto, transparent or opaque.
- More ways to pay for an image: Seedream 5.0 Pro and Flash on ModelArk, Nano Banana 2 and Pro straight from Google or on Venice, and on your Higgsfield, Runway and Pika logins from their plan credits.
- The original Nano Banana is out of the picker; Google retired it.
- Gemini Omni Flash 1.1 in Clip Gen, 360p to 4K with video refs, and the Video Editor starts on it. Extend a video by 3 to 10 seconds, up to 40, on your Google key.
- Venice: Seedance 2 and 2.5 on your Venice key, and Claude on Venice for the Co-Director.
- Seedance 2.5 drafts. A draft switch renders a cheap 480p take; right-click it to finish at 1080p.
- H3 Max Lip Sync in Clip Gen: a still that talks to a voice.
- Local LTX moves to Lightricks’ newer text encoders (an older install offers update in the Models card), and renders with only the full size installed.
- Sora 2 is gone: OpenAI shut it down. Clips that used it keep their takes.
- Gemini 3.8 voices in the Voice card: design a voice from words, search Google’s voice library, or have two speakers in one line.
- Eleven v4 and v4 Turbo voices: pick one of yours, design one, or clone a sample.
- Lyria 3.5 in Score, with up to 10 pictures to set the mood.
- ElevenLabs Music v2.5 in Score.
- SFX Gen (Window menu): sound effects from the footage under them (Sonilo) or from words (ElevenLabs), placed on a score track.
- Lip-sync in the Video Editor with sync-3 or VEED Lipsync v2. Right-click a block to lip-sync it to the sound under it.
- Music refs in Score: drop a track in and ACE-Step or ElevenLabs Music follows it, from only its style to its tune.
- Voice extras: a char sheet’s voice comes with it as an @audio slot, each slot is timbre or dialogue, and a clip’s dialogue lines render to a Library track.
- Fable 5.1, Opus 5.5 and Sonnet 5.5 for the Co-Director, and a thinking level beside the model.
- The renders switch. Turn it on and the Co-Director may press render for you, only when your whole message is go.
- The Co-Director sets every Image Gen dial, flags takes and copies takes to the Library.
- Say research or paste a link and the Co-Director searches the web for that exchange.
- More Co-Director engines: ChatGPT through Codex, Gemini CLI and DeepSeek.
- Rules by number: save rule, edit rule, delete rule. Replies show the tools they ran, and the chat compacts itself at 40 messages.
- A check before every render flags problems in the assembled prompt, above the render button.
- Gemini 3.8 Flash watches takes and cuts.
- Drop a skill on the MOODS fold to make it a MOOD. Share your MOODS with the community, and install other people’s from ⇣ community.
- Several logins per Bridge supplier in one pool. A render spends the login with the most credits.
- Artlist and ElevenLabs Bridge rows log in through Video Dancer’s own page.
- A setup wizard on first run, and in Settings: every service, what it gives, and its key or login.
- A job that needs a missing key opens that supplier’s key card.
- Sign in to Claude from the app when the login runs out.
- ModelArk balance: add a BytePlus Access Key in Settings and the ARK chip shows what is left.
- A failed render says what went wrong in one plain line. Hover it for the supplier’s full reply.
- LoRA rows wrap in a narrow sidebar.

**Selection, dissolves and image references.** In Bin or Library, Ctrl/Shift-select
items and right-click a selected item for **delete N selected**. Selections across sections are
included; one Undo restores the deletion and source files stay on disk. On the timeline, select
clips and click **Cross-dissolve**, choose a duration, then **Apply dissolves**. The same dialog is
available on right-click; double-click an existing transition block to adjust it. Locked clips,
gaps and the last clip cannot receive a dissolve. Drag either edge of the labeled transition block to adjust the overlap; drag the small cut marker
to create one. Center, Start and End at cut alignment are available on double-click. Stripes mean
unused source footage has run out and edge frames repeat. Both clips otherwise keep moving
through the blend, with effects retained. Clip positions stay fixed and audio fades remain separate. In Image Gen, drag a take directly into
reference A or B; it is kept in the Library and assigned to that slot. Library image drops still
work. The monitor also retains its picture while scrubbing instead of flashing black.

**Watch and timeline review.** Settings → Watch has **Watch model**, defaulting
to `gemini-3.8-flash`. In the Timeline toolbar, **Watch cut** opens a review of the entire timeline
or its marked in/out range. Enter a question and click **Watch cut** in the dialog. Progress and
the answer appear there; **Cancel** or closing the dialog stops the request. The Co-Director can
also respond to “watch the timeline and describe the ending” using its `watch_timeline` tool.
The prepared video includes trims, effects, transitions and mixed audio, with timeline timestamps.
Google errors can fall back to the configured Claude reader; results then explicitly say
**Still-frame review: no motion or sound**. This does not capture live playback glitches.
Supplier usage may be billed; temporary review files are removed afterward.

**Voice card VIA.** Beside the voice MODEL picker, VIA shows who runs the model.
Seed Audio shows **fal** and uses the saved fal API key and fal credits. The field follows the
selected model and stays fixed when only one route is supported. Voice queue entries also name
the provider. Upload failures identify the image/audio upload stage and give a key/credit hint
for access errors.

---

## 1. What Video Dancer is

Video Dancer is **storyboard-first** filmmaking. The user writes each shot as a structured plan
(beats, characters, references, including their own footage and music), renders AI video takes
on top of that plan through their own supplier account, edits results non-destructively with
plain words (vid2vid), and cuts everything on a multi-track timeline with music, effects,
dissolves and mp4 export. Everything is local: projects, renders, and API keys stay on the
user's machine.

The core mental model, in one line: **the storyboard is the movie; renders are versions of it.**
- A **clip** is a planned scene: prompt fields + characters + **beats** + references + its
  rendered **takes**.
- **Beats** are the shot-by-shot storyboard inside a clip (camera / action / lighting / dialogue
  / vfx / reaction / sfx, each with a length). They compile into the structured prompt the video
  model receives. Beat colors appear on the timeline blocks, so the cut structure is always
  visible.
- A **take** is one immutable render plus the exact recipe frozen at render time. Takes never
  overwrite the plan.
- **S-B** ("storyboard") means the live recipe view, always one click away from any take.
- A clip with zero renders is still fully usable: it plays, previews, and exports as its
  storyboard (beat reference images held for each beat's duration).
- The loop that makes the app what it is: any video (imported footage or a finished take) can
  ride into the next render as a reference (@video slots), and any video can be edited with
  words in the Video Editor. Generate, refine, re-reference, repeat.

## 2. Setup

### Install
- Download Video Dancer free from shdw.work (https://www.shdw.work) or the GitHub releases page.
- **Windows**: run `VideoDancer-Windows-Setup.exe` (the releases page also keeps a copy named by
  version, `Video-Dancer-Setup-<version>.exe`). SmartScreen will warn ("Windows protected your
  PC") because the beta is unsigned. Click **More info → Run anyway** (one time). The app then
  looks for updates on launch and every 3 hours, downloads one in the background, and installs
  it when you press **restart** on the header chip; a quit never installs. A quiet header chip
  appears only if an update actually fails.
- **macOS**: open the `.dmg`; the app is unsigned, so the first open is blocked. On macOS 15 and
  later: try to open it once, then **System Settings → Privacy & Security → Open Anyway**. On
  older versions: **right-click the app → Open → Open**. No auto-update on Mac yet. Get new
  versions from shdw.work.

### Suppliers (required for cloud engines)
Cloud rendering runs on the user's OWN account at an AI supplier; they pay the supplier
directly. There is no shared or bundled key. Local LTX 2.5 renders need NO supplier and no
key: they run free on the machine's own NVIDIA GPU (see Models below). The first launch walks
through the options with paste-and-test boxes. **⚙ Settings → Connections** shows each
supplier as its own card: paste a key and press **Check and save** (a free check, it never
spends credits; a supplier with no check has **Save key**), later **Check**, **Replace** or
**Remove** it, with a **Get a key ↗** link to the supplier's page. A saved key is never shown
again, only its status (checked, or "Saved · not checked"). Keys are stored only on the
machine, in its data folder, encrypted with the OS keychain where one is available and as
plain text where it is not. A banner reminds the user until at least one supplier is
connected; any one supplier unlocks cloud rendering.

- **fal.ai (recommended).** One key powers everything: Seedance 2 (with video and audio
  references), Seedance 2.5, Omni video edits, and image generation.
  Pay-per-use in dollars. Key at fal.ai → **Settings → Keys** (format `id:secret`). An optional
  fal **admin** (billing-scope) key shows the live $ balance in the header.
- **BytePlus ModelArk.** Seedance 2 and 2.5 direct from ByteDance: image and audio refs, first/last
  frame, 10-bit 4K. Video references are not wired yet (their API wants public URLs; the slots
  say so). Their policy: reference images must not contain real human faces. Token billing via
  console.byteplus.com; the dollar estimate shown is worked out from the token rate and assumes
  16:9. A connected ModelArk gets an `ARK ↗` console chip in the header.
- **Astria.** Seedance 2 on Astria plan credits: text-to-video and first/last-frame i2v. No
  reference images over their API.
- **Higgsfield (key).** Their developer API still doesn't serve Seedance; use the Bridge login
  below instead. The key field stays for the day their API ships it. A connected key gets an
  `HF ↗` chip.
- **Google AI (Gemini).** Lets the Co-Director WATCH video: ask "how's the latest render?" and
  it hands the take to Gemini Flash and answers from what it saw. Score Gen's compose reads the
  footage the same way. Key at aistudio.google.com (Get API key). Without it the Co-Director
  reads still frames instead, with no motion or sound. A connected key gets a `GEM` chip
  beside `FAL` showing what the watching has cost (an estimate from tokens; Google shows no
  balance for these keys).
- **ElevenLabs.** The Music v2 score door: a score's beats become its section plan. Bills
  ElevenLabs credits. Key at elevenlabs.io (Profile → API keys).

The **SPND** chip in the header tracks what the current project has spent; clicking it shows a
per-render cost breakdown. In any key field, Enter saves.

### Co-Director (the in-app AI copilot)
Two ways to power it:
- **API (default)**: paste an Anthropic API key in **⚙ Settings → Connections**.
- **Claude Code bridge (experimental)**, which uses a Claude subscription instead of an API key:
  1. Install Node.js (if not present), then `npm install -g @anthropic-ai/claude-code`.
  2. In Video Dancer: **⚙ Settings → Connections → Claude Code → Log in with Claude**. The app
     keeps its own login (under `llm-accounts/` in its data folder); a terminal login is neither
     needed nor read. Codex and Gemini CLI connect the same way.
  3. **⚙ Settings → Co-Director → Active connection → the bridge** (the choice stays disabled
     until Claude Code is detected).
  The Co-Director panel shows an amber "bridge" badge when active.
## 3. Bridge (log in instead of keys)
The **Bridge panel** (Window ▾ → Bridge) connects supplier ACCOUNTS: press **login** on a row
and that supplier's own sign-in page opens in the browser; the app stays signed in afterwards
and renders spend that account's subscription credits. No API keys anywhere on this panel.

- **Suppliers**: Higgsfield and Runway (both proven live), Magnific and Pika (they require
  their paid tiers; the rows say so plainly), Artlist and ElevenLabs (their login goes through
  the app's own public page; not proven live yet).
- **The pool**: the top of the panel shows each account's credits in the supplier's own words,
  one stacked bar of who holds what share, and estimated render minutes at 480/720/1080
  (marked est; estimates sharpen as real renders teach real rates).
- **Engines**: every login adds its Seedance rows to the model dropdown as "(... Bridge)"
  picks. **Bridge (auto)** spends from whichever logged-in account holds the most credit, and
  the Queue names the account it picked.
- **The conversation**: while a Bridge render runs, the app and the supplier talk in faint
  speech bubbles behind the Queue: the ask, the reply, the job accepted, in plain words.
- **Claude answers questions**: some suppliers reply with a question instead of a render (a
  preset offer, a billing choice). The Co-Director's Claude answers it, never touching the
  prompt, the model, or the money. This needs a Claude lane; a banner at the top of Bridge
  offers both setups (API key, or the Claude Code bridge).
- **The trust rule**: a render only ever runs on the exact model and supplier picked. Anything
  the app can't honor refuses before any credit moves, and errors carry the supplier's own
  words, never raw code.


## 4. The panels

Everything docks, tabs, splits, and rearranges by dragging. **Window ▾** in the header lists
every panel; closed ones reopen from there. Layouts save as named **workspaces** (the big
button in the middle of the top bar). One panel can be maximized (Esc restores). Every panel has its own crash boundary, so
one panel failing never takes the app down. Panels: Library, Bin, Timeline, Timeline Monitor
(program), Clip Monitor (source), Clip Gen, Video Editor, Char Sheet, Co-Director, Project
Styles, Image Editor, Image Gen, Queue, Watched, Timeline Editor, Bridge (supplier logins, see §3), Sheet
Gen, Assembly, and Folder panels. The **Director's Room** is a full-screen overlay opened from
the Co-Director panel header; the **Tether** is a small floating window (Shift+D, see §10).

- **Library**: the project's images, music, AND videos. Import via buttons, drop files in, paste
  a screen grab (Ctrl+V), drag an image in from a browser, or double-click empty space for the
  import window. Right-click images for actions (edit with AI, **make image**: a new Image Gen card filled from the
  image’s own recipe, PNG settings or Image Editor prompt, or the Co-Director offers to write it; rename @title, make clips,
  **export as…**, disable, delete). **Disable** dims an item and takes it out of the pickers;
  nothing that uses it changes. Arrow keys step through tiles and takes rows, previewing each. Multi-select
  works: drag several anywhere, or right-click to make clips / one clip with the images as
  beats. **watch folder** points at any external folder (Comfy's outputs, downloads) and shows
  its newest images in the self-refreshing **Watched** panel; drag one into the Library to
  import it, or straight onto a clip slot to attach it. The panel head has **local | civit**:
  civit lists the images you liked on civitai.com (your Civitai key in Settings); right-click a
  tile for its prompt and loras (send to prompt, use / search civit), import it, open it on the
  site, or send it to the Co-Director for a prompt of his own. Click, Ctrl-click, Shift-click and
  the arrows select tiles; **~** tags the selected for the Co-Director (a ★ marks them, ~ again
  untags). It sees every tagged picture, with its saved prompt, in each message.
- **Library videos**: import with the button or drag video files in (mp4, mov, webm, m4v, mkv,
  avi). Files normalize once to a friendly H.264 if needed. Tiles hover-scrub and carry plain
  titles. Right-click a video: **edit with AI** (opens the Video Editor tree), **make clip**
  (the footage becomes take 1 of a new clip), **add as take** to an existing clip, rename, or
  delete. Or just drag it onto the timeline and the clip is made automatically at the drop
  point.
- **Bin**: clips and timelines as tiles. **+ New clip** starts a storyboard clip. Dashed outline
  = no render yet; ⑂ = a clip born from a video edit. Also holds **char sheets**. Right-click
  for rename / duplicate / export as / send to project / disable / delete. Alt-drag a clip tile to the
  desktop to copy its video out.
- **Tabs**: the Library and Bin each have one row of tabs over the grid, each tab with its
  count (an empty one is dim). Click = that tab only, ctrl-click adds or drops one, shift-click
  opens every tab between. Open tabs share one scroll, each under its heading (the Bin's with
  its + button). Drag a tab to move it. Each panel remembers its open tabs.
- **Folders**: a row of chips over the grid in the Library and Bin. Click a chip for that folder
  (its subfolders open as a row under it), ctrl-click adds another, click a lit chip to back
  out; nothing lit = everything not in a folder. Drag cards onto chips, drag a chip onto a chip
  to nest it. Right-click a chip to rename, add a subfolder, open it as its own panel, delete.
- **Clip Gen**: the authoring panel for one clip (see §5).
- **Clip Monitor**: source monitor for whatever was double-clicked (see §8).
- **Timeline + Timeline Monitor**: the sequence and its program monitor (see §9).
- **Video Editor**: THE editing surface for vid2vid (see §13).
- **Queue**: every paid job with live status (see §11).
- **Image Editor**: node-tree image generation and editing (see §12).
- **Image Gen**: Krea 2 image generation on your own GPU, with a LoRA sidebar (see §12).
- **Co-Director**: the copilot (see §10).
- **Sheet Gen**: reference sheets straight from the video model, so a look never passes
  through an image editor. Right-click a Library image → **make char plate**, **make scene
  plate**, or **make expression plate**. Each seeds a capture clip: a boring 15-second render
  (plain grey, no camera movement, a new view every 3 seconds; characters 3:4, scene plates
  16:9 with the subject stripped, expressions five big feelings). Render it on any model, then
  **build sheet** pulls one clean frame per view and stacks the 2×2 sheet. The views land in a
  Library folder named after the take (`viking char sheet · T2`), the sheet at the root, tagged
  so every prompt that attaches it reads "take identity from all its panels, copy none of its
  framings". The panel's preview shows takes and built sheets; ⤢ opens them big.
  A scene plate turns on one spot: east (the picture itself, 3 s), then north, west and south
  (4 s each). **▤ build sheet** makes the **compass plate**: the four views, each labelled
  FACING EAST, NORTH, WEST or SOUTH. Scene plates made before 0.35.0 keep their five views and
  the 2×2. On a character plate, **build card** (top of the panel, or under a take) makes the
  **character card**: the front, side, back and face side by side, with the char sheet printed
  in a white column beside them (NAME, CHARACTER, FEATURES, VOICE), one 21:9 picture. It
  acts on the selected take, else the keeper. The card lands in the Library and becomes the
  char sheet's picture; a prompt that attaches it reads the printed text as the character's
  exact description. If the char sheet is empty, it opens instead and Codi fills it in from the
  picture; press **build card** again when it is done. A field too long to fit is cut with "…"
  and the toast says so, as it does when a figure runs past its window.
- **Assembly**: the Co-Director's first cut. **Assembly concept** reads the conversation and
  the storyboard and writes the cut as an outline; correct it in the box under it (Enter
  re-runs), then **lock**. **▶ assemble** watches every take of every shot (keeper plus two),
  picks the take and the window that serve each outline shot, and lays them in story order on a
  NEW timeline. Hover a block to see which shot it serves. Shots the story needs but no clip
  provides are listed as holes, never faked. The monitor on top plays the active timeline.
- **Score Gen**: music for a span. Stretch a score bar over the timeline, select that block,
  then press **compose**. The selected span renders to a draft proxy and is watched once,
  using Google AI or the existing Claude still-frame fallback. The Co-Director writes musical
  beats; Compose sets the recipe length to the span. Empty beats fill in place; existing beats
  produce a duplicate. Selecting a span is required when the score has several on that timeline.
  **VIA** names the supplier: MiniMax Music 3, Sonilo and Beatoven use fal; **ElevenLabs Music v2**
  uses its separate key and music credits; ACE-Step and MiniMax Local use installed runtimes.
  Compose's watching and Co-Director connections are separate from music generation credits.
  **Queue** freezes the current beats and settings. Sonilo scores the selected span directly;
  its beats remain notes. ElevenLabs supports lyrics with instrumental unticked. Its plan keeps
  the requested duration; MiniMax can finish early. Musical beat times remain guidance.
  Picking an installed local model keeps the editor in front. Missing models offer setup;
  active downloads show their progress. Score and Voice take-color stripes survive keeper changes.

## 5. Writing a clip (Clip Gen)

The panel leads with RESULTS and is laid out as bordered CARDS, each its own space: **Takes**
(the preview player + take grid), **Model** (model · via · mode on one row; duration ·
resolution · aspect · audio on the next, with the lora picker), **Prompt** (reference chips
float above the prompt grouped by type (double-click a chip to open that ref's editor), with
the link button, the folding fields, and the generated preview), and **Beats** (a taller
storyboard timeline with bigger beat names). A clip with nothing rendered yet starts straight
at the fields. Right-click a take card: **load this take's recipe** fills the whole form from
that take. Grey helper text is gone app-wide; hover anything for its story, and every dropdown
is the house one. The storyboard is still the source of truth; the panel just stops hiding
what you paid for.

- **The take monitor**: a real jogger with timecode, scrubbing, and the take's beat colors
  banding the bar. Set an in/out window with the bracket handles or the **I / O** keys; Space
  plays and pauses while Clip Gen is fronted.
- **Drag the preview out**: onto the timeline it lands as that exact take, trimmed to the in/out
  window; onto the Library it becomes a video ready to ride as a @video ref; reference slots
  take it too.
- **Setup block**: model, render mode (ref2v / i2v), duration, resolution, aspect ratio, and the
  audio toggle. Values come from the model's real capability list; the cost estimate updates
  live. Switching models keeps the inputs.
- **Prompt & fields**: freeform prompt on top (never overwritten), plus structured Scene /
  Character / Production fields with a live YAML preview of exactly what gets sent. The preview
  text is selectable, and **Ctrl+F** while the mouse is over it opens a find bar (match count,
  prev/next arrows, Enter for next, Esc closes).
- **Render footer**: **▶ Render now** and **＋ Queue** (see §11), with the model name and live
  price. Blocked while red validation errors exist, with a tooltip saying what to fix.

### Beats (the storyboard)
- The beats bar shows colored segments sized to their lengths. **＋ BEAT** adds one; drag
  boundaries to retime; double-click a segment to open its fields; right-click to delete.
  **Auto-time** keeps beats filling the clip duration.
- **▤ block** (between ＋ BEAT and auto time) draws a rough black-and-white storyboard of the
  beats: one panel each, timecoded, stick-figure silhouettes, arrows for camera and motion.
  It lands in Library → **blocking** and attaches to the clip LAST as a staging reference; the
  prompt tells the model to take camera angles and framing from it, never identity or style.
  It warns first when the beats read like a fight, because a blocking sheet freezes fight
  motion into held poses. Re-blocking swaps the sheet; the old one stays in the folder.
- Per-beat fields: name, length, Camera (over 20 words is linted), Action, Lighting, Dialogue,
  VFX, Reaction, SFX. @mentions work inside Camera / Action / Lighting.
- **Beat reference graphic**: each beat can carry an image as a placeholder, sent to the model
  as a general reference but NOT written into the prompt text. Making beats from Library images
  (right-click a multi-selection → clip with beats) sets each image as its beat's graphic.
- Beats compile into a `cinematic_storyboard` block in the YAML the model receives. Timing
  scripted shot by shot is what cuts the number of generations needed.
- **Seedance 2.5 gets prose, not YAML.** On any 2.5 door the same fields compile into the
  bracketed sections 2.5 was tuned on: `[Reference Roles]`, `[Global Setting]`, `[Character
  Styling]`, `[Core Performance]`, `[Timestamp Storyboard]` with `[00:00–00:04]` lines, and
  `[Negative Prompts]`. The "generated from fields" box shows exactly what goes out. Refs ride as
  `[Image1]` on fal and `@image1` on the other doors; the visible prompt keeps your @titles.

### References and @mentions
- Type `@` anywhere in the prompt for Library autocomplete; picking inserts the @title and
  attaches the reference. Dragging an image into the prompt does the same.
- The references row warns (yellow) when an attached image isn't @mentioned.
- **@video slots (Seedance)**: up to 3 video references per render. Add Library videos or ANY
  take; each slot wears a positional tag (`@video1`, `@video2`, `@video3`) and the prompt
  directs it: "Continue from @video1", "Match the motion of @video2". Restyle footage, chain
  shots, motion-match a dance clip.
- **@audio slots (Seedance)**: up to 3 music windows as `@audio1…` ("Cut the motion to
  @audio1"). Non-mp3/wav files convert automatically.
- **✂ ref windows**: every video/audio slot has an in/out window; suppliers cap combined
  reference media at 15 seconds, so windows are essential. Slots warn yellow until they are
  @mentioned.
- **Guard rails**: pre-render errors catch over-15s combined, under-2s videos, more than 12
  reference files, audio without any visual ref, and deleted sources, each named by slot.
- Engines without video or audio ref support show the slots greyed with the reason. The data is
  kept, never silently sent.
- Take snapshots freeze video and audio refs too; drag-restoring from a take brings them back.
- **S-B slot**: click a reference in the Clip Monitor's top strip to mark it as the clip's
  storyboard face, the image that represents the clip on storyboard blocks and monitors.

### Characters
Three levels:
1. **Character cards** in the clip: name + base / features / physics (+ optional per-scene
   movement, emotional state, state, power fields).
2. **Character links**: any character field can live-link to another clip's character,
   per-field, with optional override text added after the linked text. Double-click a link
   chip to take the field over: the chip's text drops in for editing and the field replaces
   the link; click the faded chip to link back up (the field clears). Scene/production link
   chips carry the same gesture, with right-click opening the source style or clip.
3. **Char sheets**: a character defined ONCE (image + description) living in the Bin, with
   folders of their own. Double-click a sheet to edit it in the **Char Sheet** panel; link
   clips' characters to it ("from clip" picker). Change the sheet, every linked clip follows.

### Styles
**Style Sheet** panel: project-wide blocks (master look, production notes, lighting, etc.)
pinned into every prompt.

## 6. Models
- **Seedance 2 (fal)**: ref2v (up to 9 image refs plus @video/@audio slots) and i2v (start +
  optional end frame). Structured YAML prompts. Seed supported.
- **Seedance 2.5 (fal)**: up to 30 reference images, 10 videos and 10 audios (50 files in all),
  every integer duration 4–30 s or auto, 480p / 720p / 1080p. No seed input. Token-billed: the
  $/s estimate assumes 16:9. A **draft** switch renders a cheap 480p draft first; **finish at
  1080p** on a draft take renders the same video full size as a new take.
- **Seedance 2 (ModelArk)**: image + audio refs, first/last frame, 10-bit 4K. No video refs yet,
  and no real human faces in reference images (their policy).
- **Seedance 2.5 (ModelArk)**: the same lane for 2.5: native 30 s, 480p to 1080p, token-billed
  with the same 16:9 estimate.
- **Seedance 2 (Astria)**: text-to-video and first/last-frame i2v on plan credits. No refs.
- **Seedance 2 / 2.5 (Higgsfield Bridge)**: the full reference trio through a Higgsfield
  LOGIN (Bridge panel, §3), billing that account's plan credits. Proven live, refs included.
- **Seedance 2 / 2.5 (Runway Bridge)**: start/end frames and reference images through a
  Runway login, on Runway credits. Seedance needs a paid Runway workspace. Long prompts
  truncate at 3500 characters on 2.0 there; 2.5 takes 15000.
- **Seedance (Magnific Bridge / Pika Bridge)**: the same login lanes for Magnific and Pika
  accounts; both require those suppliers' paid tiers before they render.
- **Seedance 2 / 2.5 (Bridge)**: the auto pick. The model is fixed; the app spends from
  whichever logged-in Bridge account holds the most credit and the Queue names it.
- **MODEL · VIA**: the dropdown is split in two: MODEL picks the model, VIA picks who runs it
  (fal, ModelArk, Astria, a Bridge login, or Bridge auto). The via pick is remembered per
  model. A pick the app can't honor refuses before spending; it never reroutes on its own.
- **Gemini Omni Flash (fal)**: text-to-video, ref2v (up to 10 refs), i2v. Always 720p, 16:9 or
  9:16, 3–10s, audio always on (steer it in the prompt: "no dialogue", "calm music"). Prose
  prompts. It also powers the Video Editor's EDIT mode.
- **MiniMax H3 (local)**: the second local video engine, on the same bundled engine as LTX.
  Installs from its own area of the Models card; refs, 4 to 15 seconds, an upscale switch, and
  LoRAs from the Image Gen side panel (it sits beside Clip Gen for the local engines). Its own
  dials: **attention** off / sage / sol-attn / veda (Veda sparse attention: about 2.6x faster,
  softer faces and smear in fast action; its generated / refs sparsity, full layers, full steps
  and verbose sit under it), **turbo 3-step** (the TaoMate one-pass draft, about 3 minutes for
  15 s; off = the full dual pipeline with upscale, lms and realism), **ref video sound** (each
  ref video sends its own sound; it takes the first <Audio n> numbers), **ref size** (max =
  best likeness, match = faster) and **video vae** (fp16, or int8 at half the size). Veda
  installs with the speed kernels row; turbo 3-step and the int8 VAE are their own Models card
  rows. 720p 16:9 / 9:16 render at the trained 1344x768 / 768x1344. The Co-Director reads and
  sets every one (set_clip_settings.h3).
- **Models folder**: **change** at the top of the Models card picks where downloads go. It
  applies on the next start; files already there stay where they are.
- **LTX 2.5 (local)**: renders on the machine's own NVIDIA GPU, free, sound included, no
  supplier key. Everything installs from the **Models card**: a private Python runtime, the
  engine, and a pick of sizes: quality (int8), standard (Q5), compact (Q4), small (Q3),
  minimum (Q2), plus **full (dev bf16)**. Every installed size is its OWN entry in the model
  dropdown ("LTX 2.5 (quality int8)"); only what's on disk shows, and picking the bare entry
  with nothing installed opens the Models card. The pick saves with the clip and freezes into
  the take; a deleted size stays visible, falls down the ladder, and the Queue row says so.
  int8 measured ~40x faster than the GGUF sizes on a 16 GB card, so the download wizard
  recommends it from 12 GB up. A small **negative field** under the prompt is live on the
  bf16 pick only (true CFG); distilled sizes and cloud engines grey it with the reason.
  Local jobs show REAL step progress in the Queue ("sampling step 5/20 · 4s/step");
  switching sizes restarts the engine cleanly first. Model downloads verify size and hash on
  every file, resume file by file, remember failures in red across restarts, and raise a
  toast if one dies in the background. Take cards record the size that rendered them and the
  transformer file the engine confirmed (hover the card). Multi-subject refs ride through
  MSR (up to 4 subjects + background).
- **LoRAs (LTX only)**: the Models card's loras section is a live shelf: a Civitai browser
  (search, sort, ★ favorites), the official Lightricks adapters scanned live from their
  Hugging Face, and any .safetensors dropped into `loras/` under the models folder (the Models card's **change** button says where that is; the default is `models/` in the app's data folder). Installs pass the
  same size + hash + weight checks as model files; a JSON sidecar carries name, trigger
  words, base model and thumb. Civitai downloads need the user's Civitai key (Settings);
  browsing does not. In Clip Gen a "＋ lora" button under the prompt (LTX renders only,
  greyed with the reason elsewhere) picks installed loras: each has a 0-2 strength slider,
  picks chain into the render graph in order, and the mix freezes into the take. Trigger
  words show as tap-in chips and are load-bearing: without its trigger a style lora renders
  near-invisible. Installed rows group by model family (built for more local models later);
  untagged local files take a family by right-click, never by filename guess.
- **Krea 2 (local, image)**: the Models card's image section installs the official turbo rows
  (fp8, int8, nvfp4, bf16), the essentials, and Civitai checkpoints. Image Gen renders them on
  the same bundled engine (see §12); its LoRAs live in the panel's own sidebar, not the shelf.
- Every engine declares its own modes, durations, resolutions, ref limits, seed support and
  pricing; the UI adapts, and prompts compile per engine (Seedance gets YAML, Gemini gets clean
  prose).
- **Hidden engines**: an engine a supplier stops serving leaves the pickers, but a clip already
  using it keeps it selectable.

## 7. Takes

Every render lands as a **take card**: scrubbable thumbnail (hover to scrub), number, keeper ★,
engine, real duration, date. The **S-B** card (live storyboard) is always first.
- **Click a card** = select it and show it (or, when editing a timeline slot, set that slot's take).
  A click never flags a keeper: **~** flags / unflags the selected takes, and right-click has
  **★ keeper**. Ctrl-click and Shift-click add to the selection. Every takes row works this way
  (Clip Gen, Image Gen, Score, SFX, Voice, Sheet Gen). A render that lands is never starred, and the
  Co-Director flags a take only when you ask it to.
- **Double-click a card** = review it big in the Clip Monitor.
- **Right-click a card** = color-highlight (6 colors), **disable** as a dud (dimmed everywhere,
  skipped by the automatic keeper fallback; explicit picks still honored), **delete** (always
  warns first: pinned timeline shots leave with it, dynamic shots hop to the keeper, the file
  stays on disk, Ctrl+Z restores), or **⑂ edit** in the Video Editor.
- **Drag a card onto any field** to restore that field from the take's frozen recipe; drag it to
  the Bin to clone a whole new clip from the recipe; drag it to the timeline to place it.
- Renders are immutable. Nothing ever edits a take's file or its frozen snapshot.
- **◧ compare**: on a take that was sent a previs video, the take player's **◧ compare** lays that
  previs over the picture up to a line. Drag on the picture to move it, ← → to nudge it (Shift:
  10 %); both play on the take's clock. While it is on, the take drags to the timeline from its
  T-chip.

## 8. Clip Monitor (source monitor)

Double-click a clip (Bin tile or timeline block) → it opens here. Scrub bar with per-beat
colored bands and the trim window; trim handles commit on release; the "take N/M ▾" dropdown
switches takes (S-B included); the clip's references line the top (click one = storyboard face);
**⊢ first / last ⊣** grab live frame stills into the Library (they re-extract when the clip is
trimmed, sliced, or re-taken; that's how you continue a shot: the last frame of one clip becomes
the start frame of the next). A "details" toggle overlays the active beat's fields or the clip's
prompt / model / seed.

## 9. The timeline

Multi-track, absolute-time, Premiere-style, with the storyboard visible on every block and
filmstrip frames filling the blocks edge to edge.

- **Tracks**: **+V** adds a video track, ✕ deletes an empty one. Per-track **M**ute / **S**olo /
  🔒 lock, plus **👁** to hide a video track from playback AND export. Gaps are allowed (export
  as black); the topmost track wins where tracks overlap. Audio lanes carry their own M/S. The
  divider between video and audio drags to rebalance; track rows and lanes resize; the view
  always runs past the last clip so there is room to drop.
- **Dynamic vs pinned blocks**: a block dropped as a CLIP follows the ★ keeper (dotted amber
  ring + ★ on its take label; picking takes in Clip Gen swaps the shot live). A block dropped
  as a TAKE pins to that take for good and is named `KATA - take 3`. The take picker (label ▾)
  pins any block after the fact.
- **Audio**: every clip's audio is a blue linked block on the audio track with the same number
  as its video track (V2's sound on A2; a new video track brings its audio track). Right-click →
  **unlink audio** frees it in one step as a green free block with its own position and trims.
  Audio landing on audio OVERWRITES what is under it, the same as video; scores too.
- **Sound fx**: a sound fx (Window → SFX Gen) is a pink block on the audio tracks. Drag it from
  the Bin's **sound fx** card, or a take straight out of the SFX card, onto an A track and it
  lands there; on a video or score track it goes to the first A track free at that spot. It is
  hatched until rendered. Sonilo makes the sound of the footage under the block (with several
  blocks, click the one first); ElevenLabs makes it from words. Click a block to open it in the
  SFX card. Scores (music) stay on the S tracks.
- **Linked clips move as one**: drag the audio half and the video comes too. **Delete** removes
  both halves, **Alt+Delete** only the clicked one. Slicing a clip cuts its sound with it.
  Blocks under a muted block keep their sound. **+A/−A** manage lanes. Music: drag a Library
  track onto a lane; double-click for the waveform and detected beats.
- **Audio keyframes (Premiere)**: double-click any audio block for the tall volume view. The
  line is in dB, 0 dB at the middle, +6 at the top. Ctrl-click the line adds a keyframe;
  ctrl-click a keyframe removes it; drag moves it (Shift locks one axis); drag the line between
  two keyframes lifts both; click / Shift-click select, Delete removes them. Right-click a
  keyframe: Linear, Bezier, Auto Bezier, Continuous Bezier, Hold, Ease In, Ease Out; handles
  show on the selected keyframe and drag. Lane header while tall: ◁ ◇ ▷ = previous keyframe,
  add / remove at the playhead, next.
- **Fades = audio transitions**: select a block, Ctrl+Shift+D = a 1 s Constant Power fade on
  both free edges. Drag a fade's inner edge for length, double-click it to type one, right-click
  it for Constant Power, Constant Gain or Exponential, or to remove it. Playback and export
  trace the identical curve.
- **Moving**: drag blocks freely along time and across tracks. Snapping to the playhead and
  beats (**S** toggles all snapping; Shift-drag holds time so only the track changes).
  **Dropping onto other clips OVERWRITES them Premiere-style**: a block hit in the middle
  splits, edges trim, fully covered blocks vanish. Hold **Ctrl** while dropping to INSERT
  instead (everything after shifts right). **Alt-drag duplicates**; **Ctrl+Alt-drag slips** a
  block's content inside its window. Undo covers everything.
- **Selection**: click selects; marquee-drag empty space selects a group (drag any member to
  move them all); **A** arms select-forward (click a clip to grab it and everything after it on
  every track; V or Esc cancels); click the gap between clips to select the gap itself, and
  **Del** closes it, rippling every channel left.
- **Copy/cut/paste**: **Ctrl+C** / **Ctrl+X** copy or cut the selected block: video, audio or
  score (a linked clip goes as one). **Ctrl+V** pastes at the playhead on the block's own track
  and OVERWRITES; **Ctrl+Shift+V** inserts (everything after shifts right). Right-click empty
  track space for **paste here** (overwrite) and **close gap**.
- **Trim**: drag block edges (speed-aware, source-accurate). An **end trim ripples** so the
  sequence stays flush (hold **Alt** to leave the gap instead). **Ctrl on a flush edge =
  rolling trim** (the join slides, both neighbors adjust). Switching a slot's take ripples the
  same way when the length changes.
- **Cut**: **C** arms the slice tool (click a clip, audio or score block to cut); **Ctrl+K**
  razors at the playhead (a selected audio or score block first);
  **Q / W** ripple-trim the selected block's start / end to the playhead.
- **Per-block right-click**: frame stills to the Library, **cross-dissolve…**, **speed**
  (0.25–4×), **⟲ loop**, **✦ effects…**, unlink audio, edit with AI, remove (leaves a gap), or
  **ripple delete** (closes up).
- **Cross-dissolves**: drag the small marker at a cut to make a centered transition, then drag
  either edge of its labeled block to resize it. Double-click for duration and Center, Start or
  End at cut. Stripes warn that source handles have run out and edge frames repeat. Otherwise
  both shots keep moving, with effects retained in playback and export. Delete removes the
  focused transition; Escape cancels a drag. The toolbar and right-click dialog can apply to
  multiple selected clips. Clip positions stay fixed; audio fades remain separate.
- **⟲ Loop**: a faded tail of repeats fills from the block to the next block on the track (or
  the sequence end); drag the tail's end grip to fix a length. Every repeat is a live projection
  of the one block: trims, take, effects and speed follow instantly, and it's one undo.
- **✦ Effects**: a per-block ordered effect stack: **transform** (position / scale; shrink or
  slide a clip and the picture beyond the crop reveals itself to work against, Premiere-style),
  **flipping** (horizontal and vertical on / off, pinned under transform),
  **grid** (FIT shows the whole clip per box; the loop button locks drift to whole cells),
  **focus**, **air**, **push**, and **subject / depth masks**, each with blend modes. Everything
  composites live in the Timeline Monitor. The AI passes (subject matte, depth) run locally and
  cache next to the take, downloading their model once with a small corner progress monitor.
  Export bakes the exact same chain at full resolution, so preview and file match by
  construction. An amber ✦ badge marks blocks carrying effects.
- **Markers & range**: **M** drops a marker at the playhead (right-click the flag to name /
  recolor / delete). **I / O** set the in/out range: playback loops it, export renders only it.
- **Navigation**: wheel pans; **Ctrl+wheel zooms at the cursor**; `-` `=` `\` = zoom out / in /
  fit; **J/K/L** = play backward / stop / play (J or L again = faster, up to 8×); ←/→ step the playhead a frame (Shift = 5);
  ↑/↓ jump between cuts; **, / .** nudge the selected block a frame (Shift = 5); **Q / W**
  ripple-trim the clip under the playhead to it; Home/End = start / end.
- **Playback**: double-buffered engine, seamless cuts; dissolves preview as true crossfades;
  speed plays at speed. ⛶ = safe-area guides; 🖥 = fullscreen mirror on a second display (Esc
  there closes).

### Colour

- Premiere's Lumetri Color in its own **Colour** panel. Open it: right-click a block → **colour…**, or Window →
  Colour, or **open** on a colour row in the Effects panel. It follows the selected block, nest blocks and
  storyboard blocks included.
- **Sections**, in Premiere's order, each with its on box and ↺: basic correction, creative, curves, colour
  wheels & match, hsl secondary, vignette. The slider ranges are Premiere's.
- **Instances**: the header's dropdown lists the block's colour entries, with **＋ add colour** and **rename…**;
  on/off and **↺ all** beside it. The first touch of a control adds the entry.
- **Typed values**: click a slider's number, type, Enter commits, Esc cancels (the Effects panel too).
- **Input LUT and look**: both dropdowns list the `.cube` files in the LUT folder (`Data\luts`); **browse…**
  copies one in. A project keeps the file name only; a name missing from the folder shows as missing and the
  grade draws without it. The **look preview** shows the Monitor's frame through one look: ‹ › step, a click
  applies the one shown, the grip resizes it.
- **Auto** (basic correction): sets temperature, tint, exposure, contrast, highlights, shadows, whites, blacks
  and saturation from the frame in the Monitor. **Intensity** scales them, **reset** clears them.
- **Eyedroppers**: white balance, the hsl key (set ＋ −) and the five hue curves. Press one, then click the
  Timeline Monitor's picture; Ctrl+click samples a larger patch, Esc cancels.
- **HSL secondary**: the H, S and L bars key a colour (top triangles = range, bottom triangles = soft edges);
  denoise and blur refine the key; a wheel, temperature, tint, contrast, sharpen and saturation correct inside
  it. The mask view shows the key in the Monitor only; the export renders the picture.
- **Comparison view**: ◧ on the Timeline Monitor (or **comparison view** in the panel). A reference frame
  beside the live picture, or split across it (vertical or horizontal). The bar under the picture moves the
  reference: ◀ ▶ to the cuts, the scrub bar, **this frame**. ⇄ swaps the sides; drag the split line,
  double-click it for the middle. The reference is drawn the way the export draws it, without the grade open
  in the Colour panel (tag **before**). **apply to reference** puts that grade on it as it is now and holds it
  there (tag **reference**), so the next changes show on the live picture only. **↺** takes it off, and moving
  the reference starts it without the grade again. A block whose grade is not open shows as it is.
- **Apply match**: needs the comparison view on. Sets the three colour wheels and the basic saturation so the
  block matches the reference frame.
- **Face detection**: a checkbox beside apply match, ticked by default (Premiere's default); stored on the colour
  instance as `faces` (1 / 0), so copy grade, paste grade and presets carry it. Ticked, apply match first finds
  the faces in the reference and in the block's frame (at up to 640 wide), and a pixel inside a face counts
  three times in each luma third's mean and in the chroma spread. A toast says how many faces each frame had;
  none found means the whole frame counted the same. Unticked, nothing is detected and the match counts every
  pixel once. The model is YuNet 2023mar (OpenCV Zoo, MIT, 232,589 bytes, pinned by revision and sha256), the
  `face` row of the Models card, in `Data\models\fx\`. While it is not on disk the button reads **apply match ·
  downloads face model first (~230 KB)**; the click downloads it (the Models card raises) and then matches. A
  model that fails to load leaves the match to run without faces, and the toast says why. Premiere's own face
  weighting was not measured: the 3× is this app's number.
- **The ≡ menu**: **copy grade** / **paste grade** (onto any block's open instance, or as a new one), **save
  preset…** / **apply preset** (kept in `Data\colour-presets`), **export .cube…**, **scopes**. Export .cube
  writes basic correction, creative, curves and the colour wheels as a 33-point `.cube` into the LUT folder;
  sharpen, hsl secondary and vignette stay out (a LUT cannot hold them).
- **Scopes**: Window → Scopes, or ≡ → scopes. The histogram of the Timeline Monitor's picture: levels 0 to 255
  up the side, the pixel count at each level to the right; red, green, blue fills and the luma line, each
  switched by its box. Follows seeks, playback and every grade change.
- **Export** renders the same chain as the Monitor, graded storyboard stills included.

### PREVIS

- Block a shot in grey 3D before you spend a gen: stand-in actors, real cameras, keys on one clock, shots and multicam cuts. The gen paints the look.
- The Bin has a **PREVIS** tab: make a new previs there. Drag the whole previs onto the timeline as one block, or drag a single shot out.
- Double-click a previs block: the studio opens at that moment. The Timeline Monitor plays the block live from its scene; an empty clip shows its previs underneath, in the Monitor and in export.
- A Clip Gen over a previs offers that slice as its video ref: **previs available** adds it in one click, or the VID row’s **＋ previs** box picks any previs. The previs sets the clip’s length and shape.
- The studio: one tool row over the views (move, turn, scale, frame, the snaps, clay), views on the left with the shot camera inset, a side bar listing elements, cameras and shots, the inspector with a keyframe list, and the strip on the timeline’s grammar (a track per camera and keyed element). Panes split, join, swap and resize, any pane shows any view, and your own layouts save (one can be the default).
- Working in a view: **Tab** searches and adds at the pointer, a drag on empty space box-selects, right-click opens menus. Each view’s overlay list picks what it shows: every camera’s path, and **names: every one | the selected**.
- **Camera only**: an element’s inspector opens with **where it shows: everywhere | camera only**. Camera only is a wireframe in the work views that clicks pass through (a roof you work under), and solid on camera, in the bake and on the cards. Its side bar row carries a box mark.
- Keys: set them on the strip and move, copy or delete them there. Drag a path’s points and an actor’s body in the perspective view. Press **?** for the shortcuts card.
- Shots keep the take grammar (flag, colour, disable); the padlock stops every way of moving the shot camera. **Coverage** adds a master, two singles and two overs on two selected subjects in one go.
- **Export** from the strip: the animatic, storyboard sheets (PDF) or the shot list (CSV).
- **Cards**: a posed still for each camera run, on pages of up to six, sent as storyboard pages instead of the grey video. Clip Gen’s **CARDS** row keeps every version and sends the newest. Stand-ins dress from a character sheet, figures take colours, and a panel key in the prompt says who is who.
- Each card keeps its time and its camera line (`CAM FACING SE | 35 mm | 1.6 m eye level`). Before a render, the preflight says when the cards and the beats disagree. Redraw a set drawn before 0.35.0 to add them.
- North and east: the studio floor shows N, E, S and W in the work views, with the grid. Send a compass plate (§4, Sheet Gen) with the cards and the prompt names the plate view behind each card: NE sits between the north and east views; a camera looking straight up or down has none.
- The Co-Director reads and edits a previs scene with you, builds one from your words, draws its cards and lays it on the PREVIS track under its clip. Send to project carries a previs; export and gens wait for shots still baking.

### Subtitles

- The Bin has a **SUBTITLES** tab: make a subtitle there, rename it, copy it, put it in folders.
- The **SUB** track sits above the video rows. Drop a subtitle on a clip and it covers that clip (no clip: 10 s); it overwrites what it lands on. Drag to move, pull the edges to trim, click to select (Del removes). Its 👁 hides the subtitles on the Monitor, its padlock locks the row.
- Double-click a SUB block or the Bin tile: the **Subtitle** panel opens. Two languages, a style card for each (font, size, colour, opacity, outline, weight; link 1 + 2 to change both), top or bottom with its height, the second language above or below, and every line with its start and end. The Timeline Monitor shows the subtitles live. Its sections (listen, languages, the style cards, position, lines) fold: click a title or its arrow.
- **listen**: pick a model (ElevenLabs Scribe, $0.22 an hour; Gemini, about $0.10; Whisper large v3 on fal, about $0.04) and press listen. The Queue renders the stretch under each block without the score, the model hears the dialogue, and the lines come back with their times. A block’s hatched stretches have not been heard yet: **listen to the new part** hears only those and keeps every line already there.
- **translate**, under the languages: picks the model that translates, from every model on every engine you can reach (a saved key or a logged-in CLI). It starts on your Co-Director’s model and goes back to it when the app restarts.
- After a listen, each language that was not the one heard fills its empty lines through **translate**, in one undo step. Lines that already have text stay. If it fails, the lines stay empty and a note says why; a missing key opens the key setup.
- **make** beside a language: the spoken language gets what was heard; any other language is translated line by line through the model in **translate**, times kept.
- The Co-Director reads a subtitle (its languages, where its blocks sit, every line with its times) and writes the text of the lines you name in either language, times kept. One Ctrl+Z undoes it.

## 10. Co-Director and the Director's Room

The copilot reads the whole project (clips, beats, the actual reference images, char sheets,
styles, timelines, folders, and the field last clicked) and writes real values into the forms,
tinted until accepted as keep-or-revert cards. Every write is undoable.

- **It can touch everything a user can, EXCEPT money**: char sheets (all fields), whole
  timelines (create them, set their clips, per-item take / trims / speed / mute / dissolve /
  disable), keeper takes, duplicates, deletes, folders, and @renames that rewrite every mention
  project-wide. File imports stay user-side. Renders spend: it proposes and the user fires,
  unless the user switched on **renders** in its panel and approved the work with GO. A saved
  plan carries that approval into its later steps, within its limits. Beat graphics are protected and reference
  changes are add-only.
- **Many renders, one image gen**: ask for 20 variations of a gen; it lists them, the user says
  go, and one call lines them all up on that gen, each with its own prompt, rendering one after
  another. The gen's own prompt stays as it was. It reads the prompt behind every take, the
  user's marks on each (every ★, colour, disabled) and can look at each take's picture.
- **Lora examples and ~ tags**: it reads a lora's Civitai examples (the ones its examples window
  shows) with their prompts and pictures, and can narrow them by words ("the samurai ones") to
  remake or riff on. Prompts need the Civitai key in Settings. Pictures tagged with ~ in Watched
  or a lora's examples ride every message with their prompts.
- **@mention images** in the chat to hand it a Library picture (it sees the image, not just the
  name). Keep typing while it thinks; all waiting messages are sent together in order as one
  follow-up after the current reply. Messages arriving during that follow-up form the next
  batch. Each waiting message can still be removed separately.
- **The Director's Room**: a full-screen overlay for the conversation, opened from the
  Co-Director panel header (or the Window menu). The app blurs beneath; the chat sits center; a
  moodboard rail collects every image and take the conversation touches (click to zoom, mark
  two to compare); context cards track **On the Table · Still to Decide · Changes**. Name a
  clip and its take starts playing in a floating context pop ("take 2" picks that one). The
  writing cloud drifts beside the chat while it writes into fields.
- **The Screen**: say "show the latest take" and it floats up big beside the chat, playing with
  sound. Click any playing pop to put that exact take on the Screen; the Co-Director can put
  takes up or clear them itself. ▾ folds it to a corner; ✕ clears it.
- **Model dial**: the ⚭ chip in the Room flips between the newest Sonnet and the newest Opus
  (Sonnet 5.5 ⇄ Opus 5.5) with one click (Sonnet for routine passes, Opus for the heavy creative
  ones). Settings lists every bridge model: Fable 5.1 (the bridge default), Opus 5.5, Sonnet 5.5,
  Fable 5, Opus 5, Sonnet 5, Haiku 4.5; the API lane lists the same seven with Sonnet 5.5
  recommended. **A− / A+** sizes the type in both chats.
- **Claude Code too old**: a model newer than the installed Claude Code gets a plain line in the
  chat with **update claude code**; it runs the update and sends the message again. Settings
  shows the same line, and whether Claude Code is logged in.
- **Engines**: an Anthropic API key (default), or the **Claude Code bridge** (§2). The bridge
  keeps ONE living Claude session per conversation, sending only what changed, so long sessions
  stay lean on a subscription's usage window. Sessions reset themselves cleanly when the log
  clears or the project, model, or guides change. The bridge loads its tools up front: no
  search round before the first write.
- **The usage line**: under send, after every exchange: rounds, tokens read per round, tokens
  written. Hover for the split (fresh against cached) and what the prompt was made of: guides,
  project state, history, message, images. The exact prompt of the last exchange is written to
  `codir-last-prompt.txt` in the app data folder (`%APPDATA%\vi-dancer` on Windows,
  `~/Library/Application Support/vi-dancer` on a Mac; `VIDEO_DANCER_DATA_DIR` moves it), so you
  can read what it read.
- **Its guides**: eight markdown files with load toggles (Settings → Co-Director): who it is and
  how it works, operations (the procedure and reply shapes), library (prompting knowledge per
  engine), gaffer (camera, action and effects), previs, ideas (the idea engine for loose ideas),
  fail (the misreads it checks before you pay) and learning. Fork them, tune them, feed it your
  own rules. It saves a new rule only when told to save; those rules live in their own file
  (`guides/learned.md`), never a fork of the instructions, so every app update reaches them.
- **It learns from corrections**: a correction is logged to `codi/corrections.jsonl` in the app
  data folder, with a running summary in `codi/learning.json`; ask for a review and it proposes
  which ones become standing rules, saved into `guides/learned.md`. The project brief it reads
  each exchange carries your corrections word for word as well, so every lane sees them.
- **Cold read**: with **cold read on** beside the renders switch, it reads the compiled prompt
  fresh before a render and flags what the model could get wrong.
- **Readable replies**: bold, lists, tables, headings and code boxes with a copy button, in the
  panel, the Room and the tether. The tool log groups each tool with a count; refusals show in
  red; its test stills sit under the check that made them.
- **MOODS**: style briefs it puts on. The **⌃ MOODS** fold above the prompt box (panel and
  Room) lists the installed ones as chips: click = on for this session, right-click → pin =
  this project, `#name` in a message = that message only. Two ship:
  **HARDCORE ANIME** and **80S DARK FANTASY**. **+ new** has the Co-Director interview you and
  write one; **⇪ add** takes any `.vmd`, a skill `.md`, or a two-file skill zip (they convert);
  **⇩ share** saves one as a `.vmd` file for anyone. Typing a mood's trigger word with it off
  shows a "matches, turn on?" chip. It sees every installed mood and can switch one on or off
  when the work calls for it. A `.vmd` is plain
  markdown with a small header (name, triggers, not-for, author) and two halves: how to
  write, what to know. Settings → General has "your name on MOODS" for the credit.
  **⇣ community** lists the shared MOODS with their makers; one click installs one. Right-click
  a MOOD you made → **share to the community** (it asks for your name once if Settings has none).
  MOOD names are outlines while off and turn yellow when on.
- **INTENSITY**: a five-step meter above every prompt box, how HARD it writes field text,
  never how much. Click the lit step again for auto.
- **The Tether** (Shift+D): a small floating window on a string. Park it beside a field, a
  section title (PROMPT, SCENE, BEATS), a beat, a char sheet, a Library image or a Bin clip
  and that becomes "this one" for the Co-Director. Nearest wins as you drag; drag the **⌖**
  onto anything to pin it; click **⌖** to cut the string until the window moves again. Hiding
  the window drops the focus. Its own box talks to the same conversation: he knows what you
  are looking at, and writes on your word exactly as in the panel.
- **It watches video** (with a Google AI key, §2): "how's the latest render of KATA?" makes it
  watch the take and answer from what it saw, quoting motion, cuts and sound. Without the key
  it reads still frames and says so.
- **Its shell**: it runs PowerShell (pwsh when installed, else Windows PowerShell; on a Mac, sh, shown as `sh>` in the tool log) in the open
  project's folder, for work no other tool covers: looking at files and folders, checking what
  is installed, ffmpeg and ffprobe, downloading media the user gives it a link to. Each command
  has a time limit: 2 minutes unless it asks for more, 10 at most; a command that runs out is
  stopped and hands back what it printed. Every command shows in its tool log; click the row to
  see what came back. **Stop** ends it. Its guide tells it never to delete, never to read keys,
  logins or the app's settings, and to ask before installing anything.

### Continuing a plan after jobs finish

1. Ask Co-Director for the complete task, including the decisions or actions it should make
   after renders finish. It saves a plan showing the work, models, settings, counts and costs.
2. Switch **renders** on, review the displayed plan and send **GO**. That GO approves the saved
   plan, including the delegated decisions and later render calls within its stated limits.
3. Co-Director queues work and saves where it has reached. Keep the app open on that project.
   When its awaited jobs finish or fail, the app pings it with their results and its progress.
4. Co-Director uses its existing picture and video inspection tools before selecting results
   or writing dependent prompts. It decides the next action, carries it out and saves progress.
5. Read **Plan, progress and results** for the saved plan and job outcomes. **Stop plan** cancels
   queued work, requests cancellation of running jobs and keeps completed files. Switching
   **renders** off holds further dispatch and continuation.

The same notification format covers Image Gen, clips, image and video edits, scores, voice,
Enhance and other result-producing operations across their models. The Co-Director panel can
be closed while the app tracks jobs and delivers completion notifications.

Co-Director works one task at a time: it finishes a task, saves its progress and picks up the
next task in a fresh turn. Cancelling a reply pauses the plan; **Stop plan** ends it, including a
draft plan, and a stopped plan leaves the panels. A provider out of quota or signed out pauses the
plan; send **GO** to pick a blocked plan back up within what you approved. A request to queue
saved clips as they are just queues them, without a plan.

A confirmed failure can retry once within the approved allowance. A second failure blocks the
plan. A lost job means the result is unknown; it is reported without automatically submitting
it again. Reopening a project restores saved progress and reconciles confirmed outputs. Changing
the Co-Director model or exhausting the plan's limits stops continuation for review. Provider
usage follows the selected accounts; the displayed costs are descriptions, not a dollar cap.

## 11. Rendering: now, or in line

Every render surface has two buttons:
- **▶ Render now** fires the job instantly, and several can run at once. Concurrency is capped
  per provider (ModelArk allows 3 at a time; fal queues extras on their own servers). An
  instant job the provider refuses as busy drops itself back into the queue once, with a toast.
  Real errors still fail loud.
- **＋ Queue** lines it up the classic way: one at a time, in order.

The **Queue panel** opens itself the moment a job joins. The header reads **N running · M
waiting**. Every running job streams its own live supplier status (uploading, queue position,
rendering, downloading) with an ETA learned from this machine's real render history. **▶** on
any waiting job promotes it to run immediately; **↑↓** reorder the line; **⏸ pause** holds the
queue lane (running and instant jobs always finish); **✕** cancels. A waiting job cancels free;
a running job is already billing, so cancelling is best-effort.

- Results drop into the Bin in order (and adopt into the exact timeline slot being edited),
  whether or not anyone is watching.
- **Crash safety**: a render already sent to the supplier is rescued on the next launch if the
  app dies; the paid result still lands as its take. Jobs still waiting when the app quits
  don't keep running, but they persist per project, and reopening shows them as a row at the top
  of the Queue: **re-queue** puts them back in their order, **forget** drops them. Jobs are stamped to their project; switching projects parks them instead of
  rendering into the wrong one. There's also a manual "add take from file…" for anything pulled
  down by hand.
- **SAVES FAILING banner**: a failing disk save is impossible to miss and clears when a save
  lands. Projects living in cloud-synced folders get a one-time notice.
- **Chinese for Seedance**: a Seedance render sends its prompt in Chinese, translated through the
  Co-Director's route; the English stays the recipe and the take keeps what was sent. Clip Gen's
  generated box has **EN | 中** tabs to see what goes out, and **中 chinese on/off** to send English.
- **Costs**: every engine shows a dollar estimate before rendering; ModelArk and Seedance 2.5
  bill tokens, so theirs is worked out from the token rate and assumes 16:9. Omni video edits
  bill $0.10 per output second. The SPND chip tracks per-project spend.

## 12. Image Editor and Image Gen

Double-click a Library image (or **new image** for text-to-image). The picture sits big on top,
fitted to its height with no black bars; the **Model** and **Prompt** cards fold under it;
**▶ Generate now** and **＋ Queue** are pinned at the bottom with the model and price on the
button. Every generation is a take card in the **takes** sidebar on the right: the original
first, then each branch as a row under "from original" / "from T1" (T numbers in the order
made, ▾ folds a branch). Click a card to view it and branch from it. Right-click a card for
**make primary** (swaps the Library asset and every clip using it; make primary on the
original card reverts), **save to Library**, **open in ▸**, **reveal file** and **delete branch**
(saved copies survive).
- **Crop**: works like Photoshop. Drag an edge or a corner to move that side of the box (Shift
  keeps its shape), drag inside the box to move it, scroll to zoom it around the cursor. Outside
  the box is shaded and the readout shows its size. Enter crops to exactly the box at its own
  pixels; Reset goes back to the whole picture; Escape cancels. A crop creates a new primary
  tree version. Failed saves
  keep the crop open for retry.
- **Primary references**: references use the current primary version when generation starts,
  including queued video start/end images. Image Editor edits use the node being viewed;
  choosing the original row sends the original. Missing versions report an error instead of
  silently sending another picture. Independent Library copies remain independent.
- **✏ Draw layer**: pen over the canvas (6 colors, width, clear) to point at things. Visible
  marks are flattened into what the model receives; hidden marks aren't. Kept per node,
  non-destructive. "→ lib" bakes an annotated copy to the Library for use as a reference.
- **Grow canvas**: pull any edge outward to enlarge the frame around the image (fix tight crops
  without replacing the file).
- **Model card** (every dial under its label): **model** = Nano Banana 2, Nano Banana 2.1, Nano Banana
  Pro, GPT Image 2, GPT Image 2.5 Flare or Sunburst, Seedream 5.0 Pro, Seedream 5.0 Flash or
  Krea 3. **via** = who serves it (fal, ModelArk, Google, Venice or a Bridge login). **size**,
  **quality**, GPT Image 2.5's **background**, Nano Banana 2.1's **thinking** (high first; Venice
  and Runway take none) and Krea 3's **rewrite** switch are the picked model's own dials; a dial
  the model lacks stays visible, greyed, with the reason on hover. GPT Image 2 and Seedream 5.0 Pro
  have no seed, so the seed box greys. The pick is remembered. Hover a take card to see which
  model made that result.
- **Krea 3** (fal only): the image you edit plus up to 7 references, 2K (default) or 1K. The
  prompt names them `<image-1>` (the image you edit), `<image-2>` and on (the references, in the
  strip's order); a line under the prompt box lists which is which. **rewrite** on (the default)
  lets Krea rewrite the prompt before it draws, so the same seed won't repeat an image; off sends
  the words exactly. Each variant is its own call to fal; the ones that land are kept if one fails.
- **select** (canvas toolbar, beside compare / crop / draw): choose **box** or **lasso**, drag on
  the image. Outside dims, the edge is a dashed line. The model still receives the WHOLE image;
  only the selection changes. GPT Image 2 gets the selection as a real mask. Every other model
  is shown the outline in red and one instruction line is added after the prompt (the exact
  line is printed under the prompt box while a selection exists); when the result lands the app
  keeps only the selected area from it and restores the original pixels everywhere else. The
  model's raw output stays on disk beside the result. A selection locks aspect to the image's
  own shape, survives turning the tool off, and rides every generate until **clear**. If a
  model returns a different frame shape, the app skips the paste-back, keeps the raw result,
  and the tree row's hover says so.
- **compare** (canvas toolbar): base image on the left, the selected result on the right, same
  height. Base = the image that result was made from (its parent in the tree, or the
  original). Greyed while the original is selected, because it has no base.
- **Takes sidebar**: drag its left edge to resize, › folds it to a strip (‹ takes brings it
  back), and the zoom slider or ctrl + scroll over the cards sizes them. Remembered.
- **Open in an external editor**: right-click the original card or any take (also Library
  images and Image Gen takes) → **open in ▸** → an editor found on the machine (Photoshop,
  Illustrator, Affinity Photo, GIMP, Krita, Paint.NET, Clip Studio Paint, Paint) or **choose
  another app…** (remembered; the last one used lists first). The app opens a COPY in the
  project's `external-edits` folder; the original never changes. It watches that copy and any
  same-name file beside it in another format (PSD, PSB, TIFF, PNG, JPG, WEBP). When the user
  returns to Video Dancer after saving, it asks **"a new edit was made, want to import it?"**
  Yes lands it as a new Library image linked to its source (same folder, titled
  `@<source>_edit`); PSD and TIFF are flattened on the way in. No does nothing until the next
  save. A PDF cannot be read: the app says so and asks for a PNG export.
- **Output controls**: aspect ratio (auto plus the ratios the picked model supports), variants
  (1 to 4 per run), optional seed where the model has one. The price follows the model, size,
  quality and reference count. The model starts on Nano Banana Pro.
- **▶ Generate now / ＋ Queue**: both go through the Queue. Generate now runs at once, ＋ Queue
  waits its turn; press again for another render. Each run lands in the tree and the panel
  jumps to it.

**Image Gen** (the panel beside it): Krea 2 on your own GPU, free, through the bundled engine.
Clip Gen's grammar: prompt with @mentions and trigger-word chips, two refs (scene and subject,
a boost number under each, a REFS switch; off = plain text-to-image), model (official Krea 2
rows or Civitai checkpoints, installed from the Models card's image section), aspect, size
(1 to 2 MP), renders (1 to 4), seed, and the LoRA stack (two slots with 0-2 weight sliders,
the fixed unleashed row, a LORA switch). ▶ Generate adds a take; ＋ Queue lines renders up one
at a time, each with the prompt and settings it had when it was queued (change the prompt,
loras or anything else and queue again freely while one renders). Takes: ★ keeper, drag to the Library, open in Image Editor, open in an external
editor, reveal, delete; each remembers exactly what ran. If the engine crashes mid-render the
wait stops within seconds with the reason and the engine restarts clean. References over
4 megapixels are sent as a smaller working copy (the Library file is untouched; the model
resizes references to the render size anyway). "Windows ran out of memory loading the model"
means exactly that: close other apps or pick a smaller model, then **⏻ free GPU** in the Models
card and try again.
- **Take as reference**: drag a take into reference A or B, including a take from another
  Image Gen card. It joins the Library and fills that slot; the prompt and other settings stay.
- **LoRA sidebar**: local | civit. local reads the folders you point it at and finds each
  file's trigger words, base and thumb on its own (a sidecar, else Civitai by hash, in the
  background). civit browses Civitai for Krea 2 LoRAs (search, sort, ★ favorites, previews
  scroll on hover); download lands in its own folder with previews; use fills a slot.
  Right-click a row for its Civitai page or its posted examples in a window; the examples
  select like Watched tiles, ~ tags them for the Co-Director, right-click gives the prompt and
  loras.
- **drop png here to read**: drop any Comfy or A1111 PNG on the box beside the refs; the menu
  offers send to prompt (fills the prompt only) and lists the LoRAs used, with use or search
  civit.
- **Co-Director**: writes the prompt, adds or removes refs, and sees the open image gen's refs
  and ★ take in every exchange; reads every take's prompt, a lora's examples and the pictures
  tagged with ~; with renders on, one go lines up many prompts on the gen (see §10).
- Image gens are Bin citizens (their own card); double-click reopens, drag the tile to the
  Library to keep the ★ take. Civitai downloads and favorites need your key (Settings has a
  sign-in check); browsing does not.

## 13. The Video Editor (one editor for vid2vid)

When a take is 90% right, don't re-roll it. Edit it with words. There is ONE editing surface:
the Video Editor results tree. (The old Clip Edit panel is gone; clips it made are ordinary
clips.)

- **Ways in**: **⑂** on any take (Clip Gen take row, or a rendered timeline block), or
  right-click a Library video → **⑂ edit v2v**. The tree opens rooted on that video. A timeline
  block's trims ride in as the edit window.
- **The window**: edits take up to 10 seconds at a time (15 on Kling O3 Edit). Slide the amber window along the
  source (drag the edges to trim, drag the middle to move) to pick exactly which part gets
  edited. Only the windowed piece uploads.
- **Model, via and mode**: Clip Gen's model and via rows, then the mode. Switching keeps every
  input; ones the model can't use grey out.
  - **edit**: a frame-true word edit of the window, prompt only. *"Remove the ball. Keep
    everything else the same."* Gemini Omni Flash, roughly $0.14 per second all-in; Kling O3
    Edit, 3 to 15 seconds, keeps the original audio, call the source @Video1, about $0.17 per
    output second.
  - **extend**: adds 3 to 10 seconds to the end of the video, prompt only.
  - **lip-sync**: re-times the mouths to a voice, no words. When the voice and video lengths
    differ: cut off, loop, bounce, silence or remap.
  - **re-gen** (Seedance): the source rides as `@video1` with the full reference suite around
    it: image refs, extra videos, audio windows, plus output duration / resolution / aspect
    (up to 1080p on Seedance 2.5). Runs on fal or on your Higgsfield Bridge login (Seedance 2 / 2.5).
- **The bar** under the picture shows the video's frames with play, mute and timecode on one
  row; the window's brackets stay dim until it is trimmed.
- **Every generation is a take card** in the **takes** sidebar (the Image Editor's grammar).
  Click a card and Generate branches from it. Nothing touches the Bin or Library until a
  result is taken out.
- **Keep a result by dragging its card out**: onto empty Bin space = a new clip (the result
  becomes take 1) · onto a clip card = a new take on that clip · onto the timeline = a new clip
  with its block placed at the drop point. The right-click bake menu does the same, including
  bake to **Library videos**, where the result can turn around and become `@video1` for the
  next generation.
- **◉ primary** (Library-video sources only): the Library entry wears this node's render, every
  @video ref using that video follows it, and it reverts to the original anytime. Takes are
  immutable, so takes bake instead.
- **Delete branch** (right-click) removes a card and the takes made from it; baked copies survive; the branch
  holding ◉ refuses with the reason.
- Tree generations queue like any paid job: live status, ETA, cancel, spend ledger, crash
  recovery.
- **Chain it**: ⑂ on an edit's take keeps going; every step keeps its own takes.

## 14. Projects, saving, sharing

- **New** creates a project folder (images + renders + project file). **Open** shows EVERY
  project the app has opened as a thumbnail grid, newest first, no limit: four across, four
  rows showing, scroll for more, drag the strip under the cards to make the list taller
  (remembered). **Click selects, double-click opens.** Right-click a card for open, rename,
  duplicate, reveal, remove from list, delete (to the Recycle Bin, never a hard delete), and
  the folder entries. All media imports copy INTO the project folder.
- **Project folders** (Open window only; nothing on disk moves): right-click a card → **new
  folder…** puts it in a new folder; ctrl-click or shift-click several first and it becomes
  **new folder with N**. Drag cards onto a folder row, or use **↪ move to** in the menu.
  Right-click empty space for a plain new folder; right-click a folder to rename, nest or
  delete it (its projects drop to the parent, never deleted). Click a folder row to fold it.
- **Find projects…** (Open window header): pick a folder and every project inside joins the
  list. On first launch the app also looks beside the projects it already knows and adds what
  it finds. **Browse…** opens one project folder. The small **▾** beside Open is a quick list
  of the eight newest.
- **Cloud-synced projects** (Dropbox, OneDrive): saves keep landing while the sync client holds
  the project file. The app retries for a few seconds, then writes in place and keeps the full
  copy beside it as `project.json.tmp`. The red "SAVES FAILING" bar appears only when no save
  can land at all; pausing sync clears it.
- **Playgrounds**: the Open picker carries a shelf of downloadable sample projects. One click
  downloads (cached) and stamps a fresh copy as a normal project. First one: **1 AM**.
- Saves are atomic; undo history runs ~80 steps deep; media files are never silently deleted.
- **Snapshots** (💾): save a named state of the whole project and restore it later. The working
  copy stays current until the user chooses to restore.
- **Send to project**: right-click clips, images, music, videos, char sheets, styles, scores,
  voices, image gens or a whole timeline → **send to project** → pick a recent project or
  browse. Ctrl-click across the Bin and Library cards first and every pick goes together
  (**send N to project**). Copies land there in a folder named after this project; a timeline
  brings every clip, take, ref and track it uses; an image gen brings its takes and refs. The
  open project is never touched, and the receipt toast lists anything skipped.
- Old projects migrate automatically on open.
- **Settings > General → Clean up unused media** (**Review unused files**) sweeps orphaned files in
  the open project: scan first, confirmed delete with a real count and size, then it deletes only
  the files it showed, and nothing if the project changed in between. It refuses to run
  mid-render or mid-import.

## 15. Export

**⬆ Export** on the timeline → mp4 via bundled ffmpeg. What the monitor plays is what renders:
multi-track composite (topmost wins, 👁-hidden tracks excluded), gaps black, per-block speed
baked into video and audio, effects baked at full resolution, audio lanes with keyframes and fades,
music mixed under, mutes honored, storyboard blocks as held beat frames. An I/O range exports
just that window. Resolution 480 / 720 / 1080p, fps auto / 24 / 30. H.264 CRF 18, AAC,
faststart. **✕ in the timeline toolbar cancels a running export**; a failed export never leaves
a truncated file that looks finished. Video dissolves blend both moving shots over the monitor's
transition window with effects retained. Missing source handles repeat edge frames; audio fades
remain separate.

**Subtitles**: when the SUB track has blocks, the export row **subtitles** picks **burn in** (drawn into the picture as the Monitor shows them), **.srt** (one file per language beside the video, named after it: `film.srt`, `film.ja.srt`) or **off**. Both follow the export range.

One clip instead of a sequence: right-click it in the Bin → **export keeper as…**, or alt-drag the
tile onto the desktop or any folder (the file copies out; the original stays in the project).

## 16. Make it yours

- **Themes** (⚙ Settings): OG VDancer (amber on black), DECK (neon green), WINTERMUTE (steel
  blue), FUCKUP (70s cream, walnut, burnt orange, avocado). Or hit "customize colors": every
  color gets a picker, changes preview live, and "Save as theme…" keeps it under its own name.
- **Workspaces**: save the current layout under a name, switch from the big button in the middle of the top bar (it shows the active workspace's name).
- **About** (click the "Video Dancer" logo): version, FFmpeg attribution, the crash-log folder,
  and re-entry to the onboarding (replay the API setup guide or the panel tour anytime).

## 17. Shortcuts (global)

Space = play/pause (fronted monitor owns it) · ←/→ = step the playhead a frame (Shift = 5) ·
↑/↓ = prev/next cut · , / . = nudge the selected block a frame (Shift = 5) · Home/End · J/K/L =
play backward / stop / play (again = faster) · C = slice tool ·
Ctrl+K = razor · Q / W = ripple start/end to playhead · S = snap toggle · A = select forward
(V/Esc cancels) · V = selection tool · P = pen (audio keyframes) · Ctrl+R = Clip Speed / Duration · M = marker · I/O = in/out range (and the take monitor's window in Clip Gen) ·
− = zoom out · = zoom in · \ = fit · Ctrl+C/X = copy / cut · Ctrl+V = paste (overwrite) ·
Ctrl+Shift+V = paste (insert) · Del = remove block/group/gap (a linked clip goes whole; Alt+Del =
one half) · Esc = clear/disarm/restore · Ctrl+Z / Ctrl+Shift+Z (or Ctrl+Y) = undo/redo ·
? = the in-app cheat sheet (it also covers every drag gesture) · Ctrl+scroll = thumbnail zoom
(Bin/Library) or timeline zoom at cursor. Drag modifiers: Shift = hold time · Ctrl on drop =
insert · Ctrl+Alt-drag = slip · Alt-drag = duplicate · Alt on an end trim = leave the gap ·
Ctrl on a flush edge = rolling trim. All suppressed while typing in a field.

## 18. Troubleshooting

- **SmartScreen / Gatekeeper warnings**: expected for the unsigned beta; see §2 Install.
- **"connect a supplier" banner**: no supplier key saved yet (⚙ Settings → Connections).
- **A render errored**: usually the supplier account is out of credit, or the model rejected an
  input. The Queue shows the supplier's real error detail, including field names.
- **ModelArk rejects a render**: check the no-real-human-faces reference policy and that video
  ref slots are empty (not supported there yet).
- **The app died during a render**: relaunch; completed renders are rescued automatically, and
  waiting ones come back as a Queue row with re-queue / forget.
- **A clip plays the wrong take**: check the slot's take picker (take N/M ▾ on the block). A
  slot choice overrides the keeper; S-B means it's playing the live storyboard. A dotted amber
  ring + ★ means the block is dynamic and follows the keeper.
- **SAVES FAILING banner**: the project folder isn't accepting writes (disk full, permissions,
  or a cloud-sync folder holding locks). Fix the folder; the banner clears on the next good
  save.
- **Frames look wrong after slicing**: thumbnails sample only the block's own window; toggle
  the filmstrip off/on.
- **Co-Director bridge greyed out**: Claude Code isn't detected. Install it and log in from
  Settings → Connections (§2), then reopen Settings.
- **Logs**: click the "Video Dancer" logo → About → open the log folder. `main.log` holds the
  session's errors, every supplier exchange in full and your project names and paths: read it
  before you send it.

## 19. Known limitations (current beta)

Unsigned installers; macOS has no auto-update. Seedance 2.5 is token-billed, so its price is
an estimate that assumes 16:9. ModelArk video refs aren't wired; Higgsfield's developer API has
no Seedance engine yet (the Bridge login does). Video edits (EDIT mode) come back fixed at 720p / 16:9 / 24fps and window sources
longer than 10s. Waiting queue jobs don't auto-resume after a quit (they persist and offer a
re-queue; a render already sent to the supplier is rescued).
