## Abstract

Mental health apps suffer high session dropout, leaving users unsupported during emotional transitions. Drawing from affective computing and peer-support platforms like Cheeseburger Therapy (Brown HCI Lab), Project Bridge implements **emotion-aware notifications** that adapt timing, tone, and action (vent/chat vs mood log) based on conversation context. Research shows self-monitoring + tailored reminders boost adherence without annoyance.[1][2]

## 1. The Problem: Session Dropout in Mental Health Apps

Users forget to return between sessions, or generic reminders feel robotic, increasing dropout. Alqahtani et al. analyzed 103 apps and found self-monitoring (57%) and reminders (48%) dominate, but **effectiveness hinges on emotional relevance**—poor timing correlates with lower ratings (r=0.153). Cheeseburger Therapy, a peer-chat platform from Brown HCI Lab, achieves 93% helpfulness via structured CBT sessions but still relies on user-initiated returns.[1]

## 2. Research-Backed Solution: Emotion-Aware Adaptive Notifications

Affective computing enables **personalized interventions** that feel supportive:

- **Notification responses as affective sensors**: Kanjo et al. (NotiMind) show interaction patterns reveal emotional state, justifying adaptive timing.[3]
- **Self-monitoring + tailored reminders**: Alqahtani et al. found these drive adherence in anxiety/depression apps; relevance > quantity.[1]
- **LLM empathy at scale**: MindShift uses conversation context for 4.7–22.5% higher acceptance vs generic nudges.[4]

**Project Bridge** has an LLM "Brain" map sessions to states (High Distress → Positive) and generate **Notification Instructions** with empathetic copy + dynamic delays (2h–24h).[5]

## 3. High-Level Architecture: Brain & Body

```
Session End → LLM Brain: {Persistent Memory Blob + Transient Notification Instruction}
                    ↓
Frontend Body: SQLite(blob) + OS.schedule(instruction)
                    ↓
Tap → Deep link (chat/mood log/persona)
```

Mirrors affective platforms separating inference from execution.[1]

**Cheeseburger Therapy Inspiration**: Like their public CBT examples (Thoughts → Feelings → Behaviors → New Thought), we structure notifications around emotional state while automating re-engagement.[1]

## 4. Intelligence Heuristic (LLM Prompt)

| Emotional State | Goal | Delay | Action | Research |
|-----------------|------|-------|--------|----------|
| **High Distress** (Anger/Panic) | Check-in | 2-3h | `reply` (Vent) | Affective sensors[3] |
| **Low Mood** (Sad/Lonely) | Comfort | 6-8h | `reply` (Chat) | Empathetic LLMs[5] |
| **Positive** (Happy/Excited) | Reinforce | ~24h | `log_mood` (Reflect) | Self-monitoring[1] |
| **Neutral/Calm** | Routine | 24h | `deep_link` (Persona) | Adaptive scheduling[6] |

## 5. Related Work

**Cheeseburger Therapy** (Brown HCI Lab, UW, Invisible College): Peer CBT chat ($25/session, pay-if-helps). 93% helpfulness via structured Thoughts/Feelings/Behaviors → New Thought format. Public examples validate our emotional state buckets.[1]

| Reference | Key Finding |
|-----------|-------------|
| **[1]** Alqahtani et al. (2019) | Self-monitoring + reminders = adherence drivers |
| **[3]** Kanjo et al. (2017) | Notifications as affective sensors |
| **[4]** Xu et al. (2023) | LLM interventions: +4.7-22.5% acceptance |
| **[5]** Lee et al. (2025) | Meta-emotion LLMs for empathy |

**[Live Demo](https://cheeseburgertherapy.org/chat)** | **[Research](https://hci.brown.edu/)**[1]

[1](https://cheeseburgertherapy.org/chat)
[2. Survey on Mental Health Apps]
[3](https://ieeexplore.ieee.org/document/8048505/)
[4](https://arxiv.org/html/2309.16639v2)
[5](https://aclanthology.org/2025.emnlp-demos.66.pdf)
[6](https://www.sciencedirect.com/science/article/abs/pii/S1574119217304388)
[7](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/21868902/84410a80-aa3a-412c-9574-17ce2d0036a1/paste.txt)