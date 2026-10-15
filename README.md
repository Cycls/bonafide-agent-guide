# Bonafide Agent — a guide for Bonafide's 3D artists

**Bonafide Agent** is the creative assistant built for Bonafide's team. You talk to it like a colleague in a chat. You describe what you want in plain words, and it makes it: concept images, edits, 3D models, a full 3D scene from a CAD drawing, an event layout on a venue plan, and a small Blender-style studio to finish things by hand.

You don't need any technical knowledge. If you can brief a junior artist, you can use the agent.

Open it at **https://bonafide.cycls.ai** and sign in.

---

## 1. The first five minutes

1. **Pick a workspace** (see section 2). For a project, use that project's workspace.
2. **Start a new chat** and say what you want, in your own words.
3. **Drop files into the chat** when you have them: a reference image, a sketch, a DXF drawing, a 3D model, a logo.
4. **Read what the agent answers.** It often shows you an improved version of your prompt first and asks *Proceed? (yes / no / edit)*. Reply "yes", or change it.
5. **Find your files** in the Files panel. The agent saves everything for you, in tidy folders.

A good first message:

> New project: "Riyadh Season food court". Make a concept image of a night-time food court with warm string lights, palm trees and wooden kiosks.

---

## 2. Your workspace — where your work lives

Think of a workspace as **a project drive** that the agent can see and tidy. You switch between workspaces from the workspace menu.

### The three kinds of workspace

- **Your personal workspace** is only yours. Nobody else can open it, not even an administrator.
- **General** is Bonafide's shared workspace. Everyone in the Bonafide organization can see it.
- **Project workspaces** are the ones you create with **+ New workspace**. Only the members you add can see them.

### Our advice: one workspace per project

For every project you work on, **create a workspace for it** and **add the people who work on that project**:

1. Open the workspace menu and click **+ New workspace**. Give it the project's name, for example *E1 Jeddah GP*.
2. In the workspace's **Members**, click **Add members** and pick your teammates on the project.
   - The list shows people who are already in Bonafide's organization.
   - Someone new must first be invited to the organization by an administrator, with **Invite member**.

That way:

- **everyone on the project** sees the same files: briefs, concepts, 3D scenes and models;
- **people who aren't on the project** don't see it at all. The only exception is Bonafide's organization administrators, who can open every project workspace.

As the workspace's creator, you can add or remove members at any time.

### Good to know

- **Your conversations stay yours.** In a project workspace, your teammates see the files, not your chats. To show someone a conversation, use **Share**: the link can be open to anyone who has it, or only to people in Bonafide's organization.
- **Each workspace has its own library** (see below). To reuse a model from another project, download it there and drop it into a chat here.
- **Deleted files, apps and chats go to the Trash** and stay there for 30 days.
- **Deleting a workspace deletes all its files.** Only its creator or an administrator can do it.

### What's in it

You never have to create these folders. The agent makes them when it needs them, and tells you where it saved each file.

| Folder | What it is, in plain words |
|---|---|
| `attachments/` | Everything you dropped into a chat. |
| `projects/` | One folder per project (the agent calls a project a *pitch*). |
| `projects/<name>/00_brief/` | **The project's memory.** The agent writes the brief here: client, event, style, deadlines. It reads it back before working, so a project keeps its context from one day to the next. |
| `projects/<name>/03_design/` | Images: `concepts/` (first ideas), `keyvisuals/` (hero visuals), `moodboards/` (sets of options), `assets/` (cut-out objects), `event-plan/` (event layouts). |
| `projects/<name>/04_3d/` | The 3D scenes made from a CAD drawing: renders, the 3D file, the Blender file. |
| `projects/<name>/99_archive/` | Older versions. When you reject something or replace it, the agent **moves** it here. Nothing is deleted. |
| `library/` | **Your team's 3D library.** Every 3D model the agent makes is filed here by category (furniture, lighting, events, plants…). Every project in this workspace can reuse it. |
| `renders/` and `exports/` | What you rendered or exported from the Studio. |
| `apps/` | The Studio's own files. Leave them alone. |

**Versions.** Files are named like `booth-v1-2026-10-15.png`. Ask for "another version" and you get `-v2-`, without losing v1.

**Opening files.** Click an image to see it. Click a `.glb` to turn it around and zoom in the 3D viewer. Click a `.blend` to open it in the Studio (section 9).

---

## 3. How to talk to Bonafide Agent

### The golden rules

1. **Say what you want, not how to do it.** "A hero image of the VIP lounge at sunset" is perfect. You don't need to name software, models or settings.
2. **Name the project once.** The agent asks *"What should we call this pitch?"* if you don't. After that it remembers.
3. **Brief it like a person.** The event, the mood, the materials, the colours, the time of day, what must not change.
4. **Attach rather than describe** when you have a reference: a photo, a sketch, a logo, a drawing.
5. **One job at a time per chat.** While the agent works, the chat is busy. For something else in parallel, open a second chat.
6. **Any language works.** Write in Arabic, English or French; the agent answers in your language. If text must appear *inside* an image (a headline, a sign), write it exactly as it should read, in its own script.

### Smart Mode — the improved prompt

Before making an image, the agent rewrites your idea with the craft details an artist would add: lighting, lens, composition, materials, mood. It shows you this **Enhanced** prompt and waits for your answer:

- **yes** — go;
- **edit** — change a word or two first;
- **no** — start again.

To skip this step, say **"raw"** or **"just generate"**, and it uses your words exactly.

### Vague prompts and clear prompts

| Instead of… | Try… |
|---|---|
| "Make a stage." | "A concert stage for 5,000 people, black truss, a huge LED wall, purple and blue light, seen from the crowd at night." |
| "Change this." | "Keep the layout of this photo but make it a desert evening, with lanterns and Arabic patterns on the panels." |
| "3D of the drawing." | "Turn this DXF into the 3D fan village: white tents, beige paving, palm trees along the promenade, festive daytime feel. Keep everything where the drawing puts it." |
| "Fix it." | "The tents are too dark: make the roofs white and the poles silver." |

---

## 4. Images

Ask for a picture and the agent makes it, usually in well under a minute. It picks the right tool for what you describe:

| You want | Just say |
|---|---|
| A hero concept | "A key visual of a luxury booth for a car launch, glossy black floor, soft top light." |
| A photoreal scene | "Photoreal: a beach lounge at golden hour, linen sofas, wooden deck." |
| People and faces | "Portrait style: two hosts in white uniforms welcoming guests." |
| A clean deck visual | "Brand style: a flat illustration of the fan zone map in our blue and white." |
| Readable text in the image | "A sponsor wall with the words *JEDDAH GP 2027* in bold white letters." |
| A moodboard | "Give me 8 directions for a futuristic gaming arena." (up to 12 at once, quick and small) |

Concepts are saved at least in Full HD. Hero visuals can be pushed to 4K (see *Upscale* below).

---

## 5. Editing images

Drop an image into the chat, then say what to change.

- **Change the whole image:** "Make this daytime render a night scene, with warm uplights."
- **Swap or remove one thing:** "Replace the plastic chairs with rattan armchairs." / "Remove the car on the left."
- **Cut out an object:** "Remove the background", for a transparent PNG for your catalogue or deck. Add "precise edges" for hair, fur or fine details.
- **New background:** "Put this sofa in a marble lobby."
- **Upscale:** "Upscale this to 4K" (720p, 1080p, 1440p or 2160p).
- **Keep a plan or sketch, add the look:** drop a floor plan, a sketch or a venue photo and say "render this as a night-time festival, keep the layout exactly". The agent keeps your lines and paints over them.

Handy chain for catalogue items: *"Make a wooden reception desk, cut it out, and upscale it."* The agent runs the three steps for you.

---

## 6. 3D models from a picture

Show the agent an object, or describe one, and it builds a textured 3D model.

> Make a 3D model of this armchair. *(with a photo attached)*
>
> Make a 3D model of a modern ticket kiosk, white and wood.

- **What you get:** a **GLB**, with materials, to view and use right away, plus an **OBJ** with its textures for any 3D software.
- **Need FBX?** Ask for it. The FBX version is a bit less detailed, so only ask when you really need FBX.
- **Where it goes:** the `library/`, in the right category, with the source picture and a preview, ready to reuse in any project of the workspace.
- **How long:** a minute or two.
- **Tips:** one object per picture, seen clearly, on a plain background.

These models can then go into a 3D scene (section 7).

---

## 7. From a CAD drawing (DXF) to a full 3D scene

This is the agent's big one. Give it a site plan, a venue or a masterplan as a **.dxf**, and it models the whole site in 3D. You get four rendered frames, a polished set, a 3D file and a Blender file.

### Tell it what you want from the drawing

A drawing on its own does nothing; the agent asks what you need. Depending on your words:

- *"What is this drawing? How big is it?"* — it reads the drawing and explains it. A minute or two.
- *"An image inspired by this layout"* — a concept painted over the plan.
- *"Lay the event out on this site"* — the event layout (section 8).
- *"The site in 3D"* — the full 3D scene, below.

### Write the brief like an artist

The drawing gives the *where*. Your brief gives the *what* and the *feel*. Keep it short and visual. Here is a real example:

> **E1 Jeddah GP — a fan village on the Corniche, race weekend.**
>
> The VIP lounge on the rounded quay head is a real two-storey glass building with a roof terrace, its lounges and bars inside; the detail sheet on the drawing is its floor plan. A white JEDDAH GP arch opens the promenade, lined with flag banners and beige totems. On the quay: a small stage with an LED screen, a kids' play area, the giant yellow E1 letters wall, white tents over the lounge seating and a light railing along the water.
>
> The feel: premium and festive, in E1 blue, white and a touch of yellow.
>
> Keep everything where the drawing puts it.

And a shorter one:

> **The AFC Asian Cup 2027 at the KASC stadium.** The round stadium sits at the centre, with wide paved spokes running out to the ring roads and the car parks. Just north of it, the fan zone, packed with tents, kiosks and a big stage; fences, light towers and cabins across the whole precinct. The feel: match day, crowds arriving, a festival around the stadium. Keep everything where the drawing puts it.

**Tips**

- Say what the drawing's blocks and areas *are* when it isn't obvious: "the rectangles on the quay are tents", "the hatched area is sand".
- Give colours, materials and the time of day.
- Mention anything the lines don't show: a building that should be glass, a road that is closed.
- Notes written on the drawing itself help too.

### What happens next

The agent tells you in one line that it's starting, then works on its own:

1. **Reads the drawing.**
2. **Plans the scene,** splitting it into parts: ground, structures, furniture…
3. **Builds each part.** A team of 3D agents works in parallel, and **their test renders appear in the chat** as they go.
4. **Renders the four final frames:** *hero*, *aerial*, *eye level* and *detail*.
5. **Makes a "hi-fi" set:** an AI finish pass over the four frames, for presentation.
6. **Packs the scene** as one **GLB** (opens in the 3D viewer) and a **Blender file** (`.blend`, with its lights and editable materials).

**How long:** from about 20 minutes for a small site to an hour and a half or more for a big one. You can close the tab: the work carries on, and the links are in the chat when you come back.

**Which images to trust:** the Blender frames follow the drawing's real dimensions. The hi-fi set looks more polished but is a retouch, so small details can differ.

### Changing the 3D — during the build or after

You will see the test renders arrive. If something is wrong:

1. Press **Stop**.
2. Write the change, as precisely as you'd tell a colleague:
   > The stage is too small, make it twice as wide.
   >
   > Make all the tents white.
   >
   > More palm trees along the promenade.

The agent redoes **only the parts concerned** and keeps everything else. You can also ask for changes after the run is finished. The previous frames are kept in `renders/previous/`.

A change that needs something the plan never had, like a new kind of structure, can't be patched in. The agent will say so and offer a new run.

### Using your own assets

Your own models and visuals come first, before the library's:
- models you attach: `.glb`, `.fbx`, `.obj`, `.blend`, `.stl`, `.ply`;
- models the agent made for you (section 6);
- logos and visuals.

Say what each one is for, and its size when you know it:

> Use this armchair in the VIP lounge, it's 90 cm high.
>
> Put our logo on the big screen above the stage.
>
> Use the kiosk you made yesterday for all the food stalls.

The agent prepares each model at its real size, keeps it light, and hands it to the right part of the scene.

### Something got cut?

If a run stops halfway (you pressed Stop, or an error), just write **"continue"**. Nothing finished is lost; the agent picks up where it stopped.

A page reload or a closed tab does **not** stop a run: wait, and the results arrive in the chat.

---

## 8. Event layout on a venue drawing

Give the agent a **venue drawing (.dxf)** and describe the event. It works out **what the event needs** and **where everything goes**: stages, screens, seating, food, toilets, first aid, prayer areas, shade, back of house, gates.

Before starting, it asks, in one message, for what it can't guess:

1. **The event:** what it is and its name (the name titles the sheet).
2. **The peak headcount:** everyone on site at the busiest moment.
3. **When:** dates and daily opening hours.
4. **Where on the drawing:** only if it isn't obvious.

> Plan a family fan village on this site for the Saudi Cup. 8,000 people at peak, 4 to 11 pm, February. Visitors arrive from the north car park; the coastal road stays open.

**What you get** (10–30 minutes):
- **your own drawing, with the event added** on its own layers, the venue untouched;
- **a presentation sheet**, shown in the chat;
- the figures: zones, objects, toilets against the minimum needed, first-aid posts, the longest walk to a toilet.

Toilet and first-aid numbers follow international defaults. Confirm them with the local authority.

**Changes:**
- *"Move the main stage to the north edge, facing south"* → a new version; the old one is kept.
- *"Another design"* → a fresh option.
- Edited the drawing yourself in CAD? Attach it again and ask the agent to check it.
- **Then the 3D:** *"Now make this event plan in 3D"* runs the full 3D scene (section 7) on the layout.

---

## 9. The Studio — your 3D scene in the browser

The **Studio** is a small Blender-style editor inside Bonafide Agent, with real Blender doing the renders. To open it, **click any `.blend` in your Files**, or ask the agent to *"open the Studio"*. After its first use in a workspace, the Studio is also in the workspace's **Apps**.

If you already have a scene open, the Studio asks whether to **open** the file in its place or **add** it to your scene. Your original `.blend` is never modified.

### Work by hand

It feels like Blender:
- **select:** click, Shift-click, A;
- **move, rotate, scale:** G / R / S, or the gizmo;
- **add, duplicate, delete, hide:** Shift+A, Shift+D, X, H;
- **edit mode:** Tab, then 1 / 2 / 3 for vertex, edge, face; extrude (E), inset (I), bevel (Ctrl+B), fill (F), merge (M);
- **views:** the numpad views, Solid or Material shading, and **F12 to render**.

The outliner, materials and modifiers are all there.

### …or ask the agent

In the chat, describe the change and the agent edits the same scene:

> Make the stage floor glossy black and add two spotlights aimed at the centre.
>
> Delete the trucks behind the tent.
>
> Put this texture on the back wall. *(with an image attached)*
>
> Render it in Full HD.
>
> Make a 10-second turntable video of the kiosk.

Every change is saved. You can always go back with undo, or ask the agent to "go back to the previous version".

### Renders, videos, exports

- **Snapshot:** a quick preview in a few seconds.
- **Render:** the final image, under a minute, saved in `renders/`.
- **Video:** turntables and simple camera or object moves, up to 10 seconds (240 frames at 24 fps), at 1280×720. Keep the Studio open while it renders.
- **Export:** GLB, Blend, FBX, OBJ or STL, saved in `exports/`. If you deleted something in the Studio, the export is without it; your original file stays as it was.

### Good to know

- **One person edits a scene at a time.** If you and the agent change the same thing at once, your version wins and you get a warning.
- **Not available:** sculpting, geometry nodes and UV editing (beyond simple projections). Animation is moves only, no rigs.
- **Size:** files up to 500 MB, scenes up to 10,000 objects. Big venue scenes are fine.
- **"The Studio engine is busy":** it is shared, so wait a minute and try again.

---

## 10. When something goes wrong

| You see | Do this |
|---|---|
| The run stopped halfway | Write **"continue"**. Nothing is lost. |
| "Something went wrong" | Try again once. If it repeats, send the reference code shown with the message to the Cycls team, who run the agent. |
| The agent asks you a question | Answer it. It only asks when a guess would waste your time, for example before an hour-long build. |
| You don't like a result | Say what's wrong, precisely: "too dark", "the logo is cut off", "the tents should face the sea". |
| You lost a file | Look in the project's `99_archive/`: replaced work is moved there. Deleted files are in the **Trash** for 30 days. |

---

## 11. House rules

Please keep to Bonafide's content rules in every request:

- no depiction of a prophet or a deity;
- no nudity;
- no alcohol;
- no weapons.

---

## 12. Cheat sheet

| I want… | I say… | I get… |
|---|---|---|
| A concept | "A key visual of…" | an image, saved in `03_design/concepts/` |
| Options | "Give me 8 directions for…" | a moodboard |
| An edit | *(image)* "Make it night / replace the chairs…" | the edited image |
| A cutout | *(image)* "Remove the background" | a transparent PNG |
| A bigger image | "Upscale to 4K" | the same image, sharper |
| A plan painted | *(plan or sketch)* "Render this as…, keep the layout" | an image on your lines |
| A 3D object | *(image)* "Make a 3D model of this" | GLB + OBJ in the `library/` |
| A drawing explained | *(DXF)* "What is this drawing?" | a summary and an overview |
| A full 3D site | *(DXF)* "The site in 3D:" + your brief | 4 frames, a hi-fi set, GLB, Blender file |
| A change to the 3D | **Stop**, then "make the tents white" | only those parts rebuilt |
| My own model in the scene | *(model)* "Use this armchair in the lounge, 90 cm high" | your model in the 3D |
| An event plan | *(DXF)* event, headcount, dates, hours | your drawing with the event, plus a sheet |
| Hand editing | click a `.blend` in Files | the Studio |
| Picking up after a stop | "continue" | the run resumes |
