---
name: geoai-heygen-publisher
description: Publish an approved GeoAI lesson script and production plan through HeyGen using an approved avatar and Thai-compatible voice. Use when the user asks to create or regenerate a HeyGen presenter video, make a pilot episode, create an avatar-based lesson, or resume production after credits are available. Do not use for lesson writing or general editing plans.
---

# GeoAI HeyGen Publisher

Use this skill only after the lesson script and production plan are approved.

## Inputs Required

Before generation, confirm or resolve:

- episode title
- approved narration script
- approved scene and visual plan
- target language
- target duration
- aspect ratio
- presenter/avatar choice
- voice choice
- subtitle style

Default values:

- language: Thai
- aspect ratio: 16:9
- resolution: 1080p
- pilot duration: 2-4 minutes
- standard duration: 7-10 minutes
- presenter screen time: 35-45%

## Avatar Workflow

When the user wants to appear in the video:

1. Reuse an approved private avatar when available.
2. If no avatar exists and the user supplied a photo, create a photo avatar.
3. If the user supplied approved training footage, a digital twin may be created.
4. Confirm the avatar look is fully ready before generation.
5. Complete the platform consent flow when required.

Avatar appearance guidance:

- clear front-facing face
- even lighting
- natural expression
- smart-casual educator look
- medium or chest-up framing
- subtle forestry or mangrove context

Do not expose avatar IDs, group IDs, voice IDs, API payloads, or processing details to the user.

## Voice Workflow

- reuse the user's approved cloned voice when available
- otherwise select a natural Thai male or female teaching voice matching the presenter
- keep pace calm but engaging
- test pronunciation of GIS, GeoAI, Random Forest, Deep Learning, Sentinel-2, Carbon, MRV, and Validation
- create a short preview before producing a long episode when voice quality is uncertain

## Pilot-First Rule

Do not create an entire series before style approval.

Recommended pilot:

- first chapter
- 2-4 minutes
- landscape 16:9
- 1080p
- presenter around 40%
- one mental model
- Thai full captions
- selective keyword captions

Review the pilot for:

- face likeness
- lip sync
- Thai pronunciation
- English technical terms
- subtitle density
- presenter placement
- diagram readability
- visual pacing

Lock the style only after the pilot is accepted.

## HeyGen Generation Prompt

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
[FULL APPROVED SCRIPT]

Visual direction:
Use approved diagrams, maps, satellite imagery, drone imagery, mangrove B-roll, GIS layers, and selective keyword text.

Subtitle direction:
Thai captions throughout, 1-2 lines at a time, lower safe area. Add emphasized keyword captions only for major ideas.

Pacing:
Change visuals every 4-7 seconds. Add a meaningful pattern interrupt every 30-45 seconds.

Visual style:
Natural, earthy, premium educational documentary. Mangrove green, deep forest green, muted blue, and warm neutral tones. Avoid cartoonish visuals, crowded screens, and flashy transitions.
```

## Generation Workflow

1. Confirm avatar readiness.
2. Confirm voice readiness.
3. Create or reuse a pilot session.
4. Submit the approved prompt and full script.
5. Wait for completion without repeated status messages.
6. Deliver the share link and a one-line summary.
7. Collect revision notes.
8. Regenerate only the affected episode.
9. Produce later chapters one at a time.

## Quota and Failure Handling

If credits or quota are unavailable:

- do not claim the video was created
- preserve the approved script, scene plan, subtitle plan, and generation prompt
- record which avatar and voice were selected without exposing private IDs
- explain that production can resume when credits reset
- do not silently switch to another platform without user approval

If avatar generation fails:

- verify consent
- verify the image or footage meets platform requirements
- verify the avatar look is ready
- retry only after identifying the failure reason

If Thai pronunciation is poor:

- adjust punctuation and phonetic spelling
- shorten long sentences
- test a different Thai-compatible voice
- use uploaded human audio when supplied and approved

## Final Quality Gate

Before accepting the video, verify:

- hook appears in the first 15 seconds
- presenter resembles the approved avatar
- voice matches the intended language and tone
- technical terms are understandable
- captions do not cover the face or diagrams
- visual changes feel active but not distracting
- the mental model is readable
- the final three takeaways are clear
- no unsupported factual claim was added during generation
