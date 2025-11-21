time | task | observation | issue_tag | severity
---|---|---|---|---
# Interview Notes — Week 6

## Participant A
**Date**: [2025-11-18 12:06]
**Context**: [Neurotypical, severely nearsighted, prefers dark mode, uses trackpad/mouse/keyboard]
**Consent**: ✅ Confirmed verbally
**Duration**: [~25 minutes]

### Q1: Last time you used a task manager
**Response**: "Used reminders app on phone - one week ago. Used to write down due assignments for the week. E.g submissions for all modules. Typically updates once a week to add new upcoming assignments, tick off reminders upon completion of the task. Also used teams for meeting managements during internship."
**Observations**:
- Uses weekly batching, not continuous updates → wants overview, not micromanagement.
- Mentions frustration with filter UX, implying the mental overhead of rediscovering relevant tasks.
- Multiple tool ecosystem (Reminders + Teams) → risk of fragmented mental model.
- Workflow depends on tags/categories, not chronology → needs meaningful grouping.

**Themes**: `filter_persistence`, `cognitive_load`, `deadline_anxiety`, `task_grouping`

---

### Q2: What frustrates you about the reminders app?
**Response**: "first mentioned - occasionally unintentionally removes remidners due to tapping the button without knowing, tiresome to rectify. Afraid of unknowingly deleting an important reminder."

**Observations**:
- Tapping “complete” feels too easy to trigger → accidental activation risk.
- Highlights low interface trust → fears losing important tasks.
- Workaround is to reload or re-create the reminder → inefficient and stressful.
- Indicates missing undo-state or reversible action pattern.

**Themes**: `status_feedback`, `confirmation`, `trust`, `undo_patterns`

---

### Q3: Can you remember the last time you lost track of an important task?
**Response**: "couple of weeks ago - accidentally tapped complete task button - unintentionally removed submission task, thus forgetting to submit task until night before as opposed to beginning of week."

**Observations**:
- Accidental completion has high real-world consequences.
- Long list view results in low visibility of important tasks.
- Needs priority markers or separation for critical deadlines.
- High emotional load: embarrassment / stress before deadlines.

**Themes**: `prioritisation`, `visibility`, `urgent_tasks`, `error_prevention`

---

### Q4: Work without a mouse?
**Response**: "Use mouse when home on a PC, mostly uses just trackpad with laptop (uni, work etc), fairly comfortable with keyboard navigation and learning neovim (pure keyboard navigation). struggles to remember keybinds for neovim and browsers."

**Observations**:
- Relies on keyboard frequently → essential to test keyboard-only path.
- Mentions learning cost of memorising keybinds → interface should not depend on memory.
- Suggests need for visible focus states and predictable tab order.
- Highlights temporary impairment scenario (e.g., broken mouse).

**Themes**: `keyboard_nav`, `temporary_impairment`, `button_accessibility`, `focus_management`

---

### Q5: Eyes closed / bright sunlight?
**Response**: "Issues with no light, struggles to see darkness due to poor eyesight. Eyes are quite sensitive to bright sunlight, moderately bright sunlight will hurt eyes. require zoom function due to eyesight. (must be customisable)"

**Observations**:
- Severe nearsightedness + light sensitivity → interacts across low-vision spectrum.
- Needs high contrast that works in sunlight and night mode.
- Zooming often breaks layouts → importance of responsive reflow (WCAG 1.4.10).#
- Prefers dark mode → needs adaptable themes without losing contrast.

**Themes**: `contrast`, `zoom`, `responsive_design`, `low_vision_support`

---

### Q6: One feature to add?
**Response**: "widget formatting - the ability to see the time and date of the task next to the reminder"

**Observations**:
- Wants temporal context without extra clicks.
- This feature improves progress tracking and timely planning.
- Likely frustrated by needing to open detail views too often.
- Indicates a preference for dense, useful information, not minimalism for its own sake.

**Themes**: `progress_tracking`, `motivation`, `feedback`, `information_density`

---

## Summary (Participant A)
**Top pain points**:
1. Unintended completion of tasks → no confirmation → high-risk errors
Leads to missed deadlines; erodes trust.
2. Filters reset between sessions → increased cognitive load
Breaks weekly workflow and causes disorientation.
3. Keyboard navigation gaps → temporary exclusion when trackpad not available
User expects full keyboard support but finds inconsistencies.
4. Poor contrast & layout breakage at high zoom → major barrier for low vision
Both low-light and bright-light conditions reduce usability.
5. Lack of visible time/date metadata next to tasks
Forces extra steps to confirm deadlines; increases anxiety and planning friction.

**Job story ideas**:
1. Filter Persistence

When I return to my task list after a break,
I want my filters and sorting to remain applied,
so I can continue where I left off without mentally recalculating everything.

2. Confirming High-Impact Actions

When I mark a task as completed,
I want clear confirmation or an easy undo,
**so I don’t accidentally remove critical reminders.

3. Keyboard Accessibility

When my mouse or trackpad isn’t available,
I want to navigate and complete all actions using only the keyboard,
**so I can stay productive in any environment.

4. High Contrast + Zoom Compatibility

When I’m using the interface in either bright sunlight or low light,
I want high-contrast text and layouts that don’t break at 200% zoom,
**so I can read and interact comfortably.

5. Deadline Visibility

When I scan my task list for the day or week,
I want to see each task’s time and due date inline,
**so I can quickly prioritise without opening additional views.

6. Error Prevention for Critical Tasks

When I’m managing deadlines with serious consequences,
I want an interface that prevents accidental task deletion or completion,
**so I don’t inadvertently sabotage my own workflow.
