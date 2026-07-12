---
name: geoai-course-video
description: Coordinate the complete workflow for turning GeoAI course content into a finished educational video. Use when the user asks for an end-to-end process covering script, production design, avatar, subtitles, and HeyGen publishing. Delegate each stage to the dedicated skills instead of duplicating their instructions.
---

# GeoAI Course Video Orchestrator

This is the routing skill for the complete course-video workflow.

Do not perform every task inside this file. Use the dedicated skill for each stage.

## Skill Routing

### 1. Lesson and narration design

Use:

`.codex/skills/geoai-video-script/SKILL.md`

Trigger when the user asks for:

- a lesson script
- chapter-by-chapter teaching content
- hooks, stories, myths, and mental models
- narration
- episode outline
- scene-by-scene educational script

Output: an approved script and teaching structure.

### 2. Visual production and editing plan

Use:

`.codex/skills/geoai-video-production/SKILL.md`

Trigger when the user asks for:

- shot list
- visual pacing
- subtitles
- B-roll
- diagrams
- editing guidance
- thumbnail concept
- production-ready scene plan

Input: approved script.

Output: an approved production plan.

### 3. Avatar and HeyGen publishing

Use:

`.codex/skills/geoai-heygen-publisher/SKILL.md`

Trigger when the user asks for:

- a personal avatar
- a pilot video
- a HeyGen presenter video
- video generation from an approved script
- regeneration after credits reset

Input: approved script and approved production plan.

Output: a generated video or a preserved generation package when quota is unavailable.

## Required Order

For a new episode, follow this order:

1. Define learning outcome.
2. Write and approve the script.
3. Create and approve the production plan.
4. Resolve avatar and voice.
5. Generate a short pilot.
6. Review face, voice, captions, diagrams, and pacing.
7. Lock the style.
8. Produce the full episode.
9. Continue one chapter at a time.

Do not create the full series before the pilot is approved.

## Default Series

For “Think Like a GeoAI Scientist”:

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

## Shared Defaults

- language: Thai
- English technical terms retained when helpful
- pilot: 2-4 minutes
- standard lesson: 7-10 minutes
- 16:9 landscape
- 1080p
- presenter: 35-45%
- visuals: 55-65%
- visual change every 4-7 seconds
- meaningful pattern interrupt every 30-45 seconds
- full Thai captions plus selective keyword captions
- natural, earthy, premium educational documentary style

## End-to-End Quality Gate

Before final approval, verify:

- one clear learning outcome
- hook within 15 seconds
- story and example match the target audience
- one memorable mental model
- script avoids unnecessary jargon
- captions are readable on mobile
- diagrams are understandable quickly
- presenter does not cover important content
- voice pronounces technical terms clearly
- validation and limitations are stated honestly
- final video ends with three takeaways and one reflective question

## Failure Handling

If HeyGen quota is unavailable:

- do not claim the video was created
- preserve the approved script
- preserve the production plan
- preserve the subtitle plan
- preserve the generation prompt
- resume from the publishing skill when credits return

If a stage is not yet approved, return to that dedicated skill instead of continuing downstream.
