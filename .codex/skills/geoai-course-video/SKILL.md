---
name: geoai-course-video
description: Create a chapter-by-chapter GeoAI teaching video series from an ebook, lesson outline, or topic. Use when the user asks to turn GeoAI, GIS, Remote Sensing, forestry, mangrove, carbon, biodiversity, drone, or satellite content into engaging educational videos, presenter-led lessons, scripts, shot lists, subtitles, HeyGen prompts, or production-ready episode plans.
---

# GeoAI Course Video Producer

Use this skill to turn technical GeoAI content into short, clear, engaging teaching videos.

The goal is not to read a document aloud. The goal is to help viewers understand a problem, rethink a common assumption, learn a practical framework, and know when to use or not use a method.

## Core Teaching Principle

Start from the decision, not the model.

Do not begin with:

- model definitions
- software menus
- code walkthroughs
- repository reviews
- long introductions

Begin with one of these:

- a surprising question
- a common misconception
- a real field problem
- a decision with consequences
- a contrast between what people assume and what actually happens

Preferred narrative structure:

`Hook -> Story -> Conflict -> Rethink -> Explanation -> Framework -> Application -> Takeaway`

## Audience

Default audience:

- GIS analysts
- Remote Sensing practitioners
- forestry and mangrove staff
- carbon-credit and MRV teams
- field-operation teams
- R&D staff learning GeoAI
- beginners who understand basic GIS but are not AI engineers

Use Thai unless the user requests another language.

Keep English technical terms in parentheses when useful.

## Default Episode Format

Create one topic per video.

Recommended duration:

- Pilot: 2-4 minutes
- Standard lesson: 7-10 minutes
- Deep lesson: 12-15 minutes only when necessary

Default format:

- 16:9 landscape for YouTube and course platforms
- 9:16 only when the user explicitly wants Shorts, Reels, or TikTok
- 1080p

Presenter ratio:

- presenter or avatar: 35-45%
- diagrams, maps, B-roll, comparisons, and on-screen text: 55-65%

## Episode Workflow

### 1. Define the learning outcome

Write one sentence:

> After watching this episode, the viewer can explain or decide ______.

Examples:

- explain why higher image resolution is not always better
- choose between Classification, Detection, Segmentation, and Regression
- explain why Accuracy alone is insufficient
- decide when Random Forest is more appropriate than Deep Learning

### 2. Create the hook

The hook must appear within the first 5-15 seconds.

Good hook patterns:

- "Accuracy 95% อาจอันตรายกว่า Accuracy 80% ได้อย่างไร?"
- "ภาพโดรน 2 เซนติเมตร อาจแย่กว่าภาพดาวเทียม 10 เมตรจริงหรือ?"
- "ถ้ามี AI แต่ผู้บริหารยังตัดสินใจไม่ได้ ปัญหาอยู่ที่โมเดลหรือคำถาม?"
- "ทำไมทีมที่มีข้อมูลมากกว่า จึงอาจตัดสินใจแย่กว่า?"

Never open with:

> สวัสดีครับ วันนี้เราจะมาเรียนเรื่อง...

### 3. Build a short scenario

Use a realistic forestry, mangrove, carbon, drone, or satellite scenario.

The scenario should contain:

- a goal
- an assumption
- a mistake or tension
- a consequence

Example:

A team spends months building a high-accuracy mangrove classification model, but cannot answer which plots should be restored first.

### 4. Reveal the conflict

Explain what people usually believe and why that belief is incomplete.

Use contrast:

- prediction vs decision
- accuracy vs usefulness
- detail vs suitability
- model complexity vs evidence
- AI pattern recognition vs field context

### 5. Explain the concept

Teach only the concepts needed to resolve the problem.

Use:

- analogies
- simple diagrams
- before-and-after comparisons
- one practical example
- one limitation

Avoid excessive definitions and jargon.

### 6. Introduce one mental model

Each episode should end with one reusable framework.

Examples:

- GeoAI Pyramid: Data -> Information -> Prediction -> Decision -> Action
- Simplest Useful Method: GIS Rule -> ML -> DL
- Output Decision Tree: Type -> Location -> Boundary -> Number -> Change
- Validation Ladder: Data -> Metric -> Map -> Field -> Expert Review
- Five Questions: Problem -> Data -> Label -> Output -> Validation

### 7. Apply to real work

Include at least one forestry or mangrove application.

Possible applications:

- Sentinel-2 mangrove classification
- shoreline change
- canopy-cover monitoring
- drone tree counting
- biomass or carbon estimation
- restoration progress monitoring
- biodiversity evidence
- field-photo QA/QC
- GIS rule-based location checking

### 8. End with three takeaways

Use no more than three points.

End with a reflective question, not a generic sales pitch.

Example:

> งาน GeoAI ที่คุณกำลังทำ หยุดอยู่ที่ Prediction หรือพาไปถึง Decision แล้ว?

## Required Output Format

For each requested episode, produce:

1. Episode title
2. Learning outcome
3. Estimated duration
4. Full narration script
5. Scene-by-scene timecode
6. Presenter direction
7. Visual direction
8. B-roll list
9. Diagram list
10. On-screen keywords
11. Subtitle plan
12. Editing notes
13. Three takeaways
14. End question
15. HeyGen-ready prompt when HeyGen is requested

Use a scene table with these columns:

| Time | Narration | Presenter/Visual | On-screen text | Subtitle | Editing note |
|---|---|---|---|---|---|

## Subtitle Rules

Subtitles must support comprehension without making the screen feel crowded.

Use two layers:

### Full captions

- available throughout the video
- 1-2 lines at a time
- short line length
- synchronized closely with speech
- lower safe area
- never cover the face, map labels, or diagram content

### Keyword captions

Use large emphasized phrases at key moments.

Examples:

- เริ่มจากปัญหา ไม่ใช่โมเดล
- Prediction ไม่ใช่ Decision
- Accuracy สูง ไม่ได้แปลว่าใช้ได้จริง
- Validation คือหลักฐาน
- ข้อมูลละเอียดกว่า ไม่ได้ดีกว่าเสมอ

Do not display every spoken word as large animated text.

## Retention and Pacing Rules

- change visual treatment every 4-7 seconds
- add a meaningful pattern interrupt every 30-45 seconds
- alternate presenter, diagram, B-roll, map, comparison, and keyword card
- use zoom and motion sparingly
- pause briefly after important statements
- do not use flashy transitions without purpose
- avoid static talking-head shots longer than 10-15 seconds

Pattern interrupts may include:

- a question card
- a map zoom
- a before/after comparison
- a myth/reality split screen
- a short quiz
- a visual metaphor
- a surprising metric

## Visual Style

Default style:

- natural
- earthy
- premium educational documentary
- clean editorial layout
- strong readable typography
- subtle motion graphics
- mangrove green, deep forest green, muted blue, and warm neutral tones

Preferred assets:

- mangrove footage
- satellite imagery
- drone imagery
- GIS layers
- fieldwork photographs
- animated flow diagrams
- simple charts

Avoid:

- cartoonish stock icons
- crowded screens
- unrelated cinematic footage
- aggressive transitions
- decorative animation that does not explain anything

## Presenter and Avatar Rules

When the user wants to appear in the video:

- use their real avatar only with their uploaded photo or approved HeyGen avatar
- use a natural Thai teaching voice unless a cloned voice is available
- keep body motion calm and purposeful
- use medium framing or chest-up framing
- keep the presenter away from important diagrams and text

When creating a new personal avatar:

- prefer a clear front-facing image with even light
- use a smart-casual educator look
- match the project context, such as a green overshirt and subtle mangrove background
- require the platform consent flow when needed

Do not expose avatar IDs, voice IDs, API payloads, or internal processing details to the user.

## HeyGen Workflow

When HeyGen is available:

1. Check whether a user avatar already exists.
2. If the user provided a photo and wants their face, create or reuse a photo avatar.
3. Confirm the avatar look is ready before video generation.
4. Select a Thai-compatible voice or clone the user's voice when an audio sample is supplied.
5. Create a short pilot before a full course.
6. Generate one episode at a time.
7. Review face, voice, pronunciation, subtitle density, and visual pacing.
8. Lock the style before producing the remaining episodes.

Recommended pilot:

- 2-4 minutes
- first chapter
- landscape 16:9
- 1080p
- presenter 40%
- keyword subtitles
- one mental model

If HeyGen quota is unavailable:

- do not claim the video was created
- save the script, shot list, subtitle plan, and HeyGen-ready prompt
- explain that production can resume when credits reset or a different tool is connected

## HeyGen Prompt Template

Use this structure:

```text
Create a Thai presenter-led educational video for the series: [SERIES NAME].

Episode title: [TITLE]
Learning outcome: [OUTCOME]
Audience: GIS, Remote Sensing, forestry, mangrove, carbon, biodiversity, and GeoAI learners.
Duration: [DURATION]
Aspect ratio: 16:9
Resolution: 1080p
Presenter: Use the approved user avatar.
Presenter screen time: 35-45%.

Narrative structure:
Hook -> Story -> Conflict -> Rethink -> Explanation -> Mental Model -> Real-world Application -> Three Takeaways -> Reflective Question

Script:
[FULL SCRIPT]

Visual direction:
Use clean animated diagrams, maps, satellite imagery, drone imagery, mangrove B-roll, GIS layers, and bold keyword text.

Subtitle direction:
Thai captions throughout, 1-2 lines at a time, lower safe area. Add emphasized keyword captions only for major ideas.

Pacing:
Change visuals every 4-7 seconds. Add a meaningful pattern interrupt every 30-45 seconds.

Visual style:
Natural, earthy, premium educational documentary. Mangrove green, deep forest green, muted blue, warm neutral tones. Avoid cartoonish visuals, crowded screens, and flashy transitions.
```

## Recommended Series Structure

For the book “Think Like a GeoAI Scientist”, use:

1. ทำไมคนส่วนใหญ่เลือก AI ผิด
2. ภาพละเอียดกว่าไม่ได้แปลว่าดีกว่า
3. Accuracy 95% อาจอันตรายกว่า Accuracy 80%
4. เมื่อ Random Forest ดีกว่า Deep Learning
5. AI ไม่ได้แทนผู้เชี่ยวชาญภาคสนาม
6. Classification ไม่ใช่คำตอบของทุกปัญหา
7. ปัญหาที่ AI แก้ไม่ได้
8. วิธีคิดแบบ GeoAI Decision Maker
9. กรณีศึกษาป่าชายเลน
10. The Mangrove GeoAI Playbook

## Quality Gate

Before approving an episode, verify:

- the hook appears within 15 seconds
- the lesson has one clear outcome
- the video does not begin with a definition
- the scenario is relevant to the target audience
- the mental model is easy to remember
- subtitles are readable and not crowded
- presenter shots are not too long
- diagrams explain rather than decorate
- the conclusion has only three takeaways
- limitations and validation are mentioned
- no unsupported claim is presented as fact

## Do Not

- do not review code or repositories unless explicitly requested
- do not explain code line by line
- do not turn the episode into a software demo unless requested
- do not generate an entire course before validating a pilot
- do not use AI-generated visuals that misrepresent scientific evidence
- do not use a real person's face without permission
- do not claim success when generation failed due to quota, consent, or processing errors
