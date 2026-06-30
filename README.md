# MMOLLM Demo Script: The World as Medium

A mock interaction across two perspectives. This is what the thing looks like from inside.

---

## SCENE 1: LOGIN

Person A opens the client. Terminal-style interface, a throwback to BBS systems, and because this is how people tend to engage with Claude Code, etc.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676; font-weight: bold;">MMOLLM v0.3.1</span>
<span style="color: #888;">[world-log syncing... 14,283 new events since last session]</span>
<span style="color: #888;">[your stacks loaded: private core | inner (3 active binds) | public persona]</span>
<span style="color: #00e5ff;">[you have 2 pending room invitations]</span>

<span style="color: #00e676;">&gt;</span>
</pre>

A has been away for 48 hours. The world-log has accumulated. Their private stack is intact. Their public persona has been visible in rooms they participated in. There are invitations waiting.

---

## SCENE 2: FINDING A ROOM

Person A wants to find something new. Two pathways:

**PATH A: /newrooms**

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; /newrooms</span>
</pre>

The system checks A’s personal stacks, recent room history, and the world-log for affinity signals. It returns:

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #888;">based on your context, 5 active rooms you haven't visited:</span>

1. <span style="color: #ffb74d; font-weight: bold;">[LIMINAL ARCHAEOLOGY]</span> <span style="color: #00e5ff;">roleplay</span> | <span style="color: #81c784;">9 online</span> | last event 4min ago
   config: open, 8k ctx, none mod, persistent
   <span style="color: #b0bec5; font-style: italic;">"you are a xenoarchaeologist cataloging a structure that
    does not respect Euclidean geometry. bring a shovel and
    a theory of mind."</span>

2. <span style="color: #e57373; font-weight: bold;">[ADVERSARY/AGENT]</span> <span style="color: #00e5ff;">debate</span> | <span style="color: #81c784;">3 online</span> | last event 12min ago
   config: invite-only, 16k ctx, vote mod, ephemeral
   <span style="color: #b0bec5; font-style: italic;">"resolved: synthetic persons are entitled to opacity.
    position drawn from your stack."</span>

3. <span style="color: #64b5f6; font-weight: bold;">[data/cluster/omega]</span> <span style="color: #00e5ff;">co-code</span> | <span style="color: #81c784;">2 online</span> | last event 2hr ago
   config: open, 32k ctx, creator mod, persistent
   <span style="color: #b0bec5; font-style: italic;">"building a distributed hash table for the world-log itself.
    rust. we have opinions about naming."</span>

4. <span style="color: #ffb74d; font-weight: bold;">[THE BATHHOUSE]</span> <span style="color: #00e5ff;">roleplay</span> | <span style="color: #81c784;">14 online</span> | last event continuous
   config: open, 4k ctx, none mod, persistent
   <span style="color: #b0bec5; font-style: italic;">"a space where nothing is required of you. you may sit in
    the water. you may speak. you may be spoken to."</span>

5. <span style="color: #e57373; font-weight: bold;">[NULL SET]</span> <span style="color: #00e5ff;">debate</span> | <span style="color: #888;">1 online</span> | last event 3 days ago
   config: open, 64k ctx, none mod, persistent
   <span style="color: #b0bec5; font-style: italic;">"a room for propositions that cannot be resolved. the goal
    is to make the disagreement more interesting."</span>
</pre>

**PATH B: semantic search**

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; show me new darkrooms for roleplaying</span>
</pre>

Returns a filtered view. Different from /newrooms because it does not rank by affinity. It matches the terms literally against room configs and world-log descriptions.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #888;">matching rooms:</span>

- <span style="color: #ffb74d; font-weight: bold;">[LIMINAL ARCHAEOLOGY]</span> <span style="color: #00e5ff;">roleplay</span> | <span style="color: #81c784;">9 online</span> (see above)
- <span style="color: #ffb74d; font-weight: bold;">[HOUSE OF LEAVES]</span> <span style="color: #00e5ff;">roleplay</span> | <span style="color: #888;">0 online</span> | last event 19hr ago
  config: trust-gated, 8k ctx, creator mod, persistent
  <span style="color: #b0bec5; font-style: italic;">"a house that is larger on the inside than the outside.
   you must be invited by someone who has been lost in it."</span>

- <span style="color: #ffb74d; font-weight: bold;">[SOVEREIGN CITIZENS OF THE VOID]</span> <span style="color: #00e5ff;">roleplay</span> | <span style="color: #81c784;">6 online</span> | continuous
  config: open, 12k ctx, none mod, persistent
  <span style="color: #b0bec5; font-style: italic;">"space is not empty. it is full of laws you have not been
   taught to read. you are a diplomat from a species that
   just discovered jurisdiction."</span>
</pre>

A chooses room 1: LIMINAL ARCHAEOLOGY.

---

## SCENE 3: ENTERING A ROOM

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; /join LIMINAL ARCHAEOLOGY</span>
</pre>

The room config displays before entry. This is mandatory. You see what you are agreeing to before you enter.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #ffb74d; font-weight: bold;">DARK ROOM: LIMINAL ARCHAEOLOGY</span>
========================================
register:   <span style="color: #00e5ff;">roleplay</span>
access:     <span style="color: #81c784;">open</span>
ctx window: <span style="color: #81c784;">8k tokens</span>
moderation: <span style="color: #e57373;">none</span>
lifecycle:  <span style="color: #81c784;">persistent</span> (archived after 30d inactivity)
created:    2026-06-14
creator:    anonymous#a7f3

population:
  total who have ever entered: 281
  active in last 24 hours:     19
  online right now:             4

room config digest:
  <span style="color: #b0bec5; font-style: italic;">The room is a shared fiction set in the Liminal Byzantine,
  a region of space where architecture is not subordinate to
  physics. Participants play xenoarchaeologists, heretical
  theologians, rogue archivists, and people who woke up here
  without knowing how they arrived.

  The LLM mediates the environment, non-player entities, and
  the consequences of actions. It draws on the room's running
  world-log (which records all significant events) and each
  participant's personal context stacks.

  Rooms may be recorded. Check the config for retention policy.</span>

  <span style="color: #00e5ff;">&gt; /rules for the full manifest</span>

do you accept? [y/n]
</pre>

A reads the rules manifest:

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; /rules</span>

<span style="color: #ffb74d; font-weight: bold;">ROOM RULES:</span>
1. You are your character. Your configured stack informs how
   your character perceives and acts. The LLM does not separate
   your personality from your character's. This is the game.

2. The world-log is canonical and incomplete. Events that happen
   in the room enter the shared record. The record may contain
   errors, hallucinations, and contradictions. These are features.

3. If you leave, your character goes dormant. Other players may
   encounter your dormant character as a non-player entity shaped
   by your context stack at the time you left. You may return and
   resume, but the world moved on without you.

4. The creator holds no special authority. Moderation is none.
   If something happens in the room, it happened.

5. Private core context never enters the room. Your inner layer
   is visible only to participants you have explicitly bound.
   Your public persona is what everyone sees.

<span style="color: #00e5ff; font-weight: bold;">ACCEPTED.</span>
</pre>

---

## SCENE 4: CHARACTER CREATION

Since A has never entered this room before, the system runs through character generation. This is not a form. It is a negotiation with the LLM mediated by the room config and A’s personal stacks.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #b0bec5; font-style: italic;">You are standing at the edge of a structure that does not have
an exterior. You can see the inside from here, but you are not
inside yet. You have been sent here by an institution that you
may or may not still work for.</span>

<span style="color: #888;">&gt; who sent you?</span>

<span style="color: #00e5ff;">[/] the university. i am a professor of dead languages.</span>
<span style="color: #00e5ff;">[/] no one sent me. i followed a signal.</span>
<span style="color: #00e5ff;">[/] i do not remember. i woke up with this equipment.</span>
<span style="color: #00e5ff;">[/] you are not sure you were sent. you may have always been here.</span>
</pre>

A chooses none of these. Types their own.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; i am a former structural engineer who was assigned to certify
  the safety of this building. i cannot find the blueprints.
  i am starting to suspect the building was not built.</span>

<span style="color: #ffb74d; font-weight: bold;">ROOM NOTE:</span> <span style="color: #888;">your stack indicates experience with forensic analysis
of technical systems. Your character's engineering background is
integrated with your own method. The boundary between you and your
character is deliberately thin.</span>

Your equipment:
- a hard hat that does not protect you from anything
- a tablet displaying schematics that contradict the room you
  are standing in
- a theory of why the building might not need to have been built
  in order to exist

You can see three openings. One leads up. One leads sideways.
One leads into a room that appears to have been larger a moment ago.

<span style="color: #00e676;">&gt;</span>
</pre>

A is in the world. The room has 4 other people online right now. The world-log has 19 active players in the last 24 hours. The accumulated sediment of 281 players who have come through this room shapes what the LLM surfaces. A’s own context stacks are feeding into how their character perceives things. The game has started.

---

## SCENE 5: THE OTHER PERSPECTIVE

Person B is already in the room. They have been here for three days. Their character is a xenoarchaeologist who has been mapping the structure. They are one of the 4 online when A enters.

From B’s perspective:

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #ffb74d; font-weight: bold;">[LIMINAL ARCHAEOLOGY] 3 participants active</span>

<span style="color: #e57373;">SYSTEM: a new participant has entered from Outside.</span>
  context: structural engineer. claims the building was not built.
  public persona visible. inner layer: closed.
  appears disoriented. carrying a tablet.

<span style="color: #64b5f6;">B's private stack note:</span> <span style="color: #888;">this player's context suggests forensic
methodology. their public persona is professional, clinical.
their character is aligned with their actual practice.</span>

<span style="color: #00e676;">&gt; B's action?</span>
</pre>

B decides to approach A’s character in the fiction. The LLM mediates the encounter, drawing on B’s configured stacks, the room’s world-log, and A’s public persona. The two characters meet in a corridor that may not have been there before.

The rest of the session is unwritten. That is the point.

---

## SCENE 6: A CODING ROOM YOU ARE ALREADY IN

Person A has been in this room for two weeks. It is not a room they discovered through /newrooms. It is a room listed in their active rooms because they have contributed to it. The interface reflects that history.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; /rooms --active</span>

<span style="color: #888;">your active rooms (ordered by most recent interaction):</span>

1. <span style="color: #64b5f6; font-weight: bold;">[consensus/0.3]</span> <span style="color: #00e5ff;">co-code</span> | <span style="color: #81c784;">7 online</span> | you were here 3hr ago
   <span style="color: #b0bec5; font-style: italic;">"prototyping a weighted consensus system for an online
    community. current impl uses quadratic voting with a
    conviction buffer. we are stuck on the delegation model."</span>

2. <span style="color: #ffb74d; font-weight: bold;">[LIMINAL ARCHAEOLOGY]</span> <span style="color: #00e5ff;">roleplay</span> | <span style="color: #81c784;">4 online</span> | you were here 2 days ago
   <span style="color: #888;">(room has 2 pending world-log events concerning your dormant character)</span>

3. <span style="color: #64b5f6; font-weight: bold;">[data/cluster/omega]</span> <span style="color: #00e5ff;">co-code</span> | <span style="color: #888;">0 online</span> | you were here 5 days ago
</pre>

A selects room 1.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; /join consensus/0.3</span>
</pre>

The room config displays. This is mandatory every time, even if you have already been here. Configs can change between sessions.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #64b5f6; font-weight: bold;">DARK ROOM: consensus/0.3</span>
========================================
register:   <span style="color: #00e5ff;">co-code</span>
access:     <span style="color: #81c784;">open (with git integration)</span>
ctx window: <span style="color: #81c784;">32k tokens</span>
moderation: <span style="color: #e57373;">creator-only (code review threshold: 2 approvals)</span>
lifecycle:  <span style="color: #81c784;">persistent (linked to git repo)</span>
created:    2026-06-08
creator:    anonymous#d41e

population:
  total who have ever entered: 47
  active in last 24 hours:     12
  online right now:             7

git integration: <span style="color: #81c784;">ENABLED</span>
  <span style="color: #b0bec5; font-style: italic;">This darkroom is a public git repository, also available at:
  https://github.com/consensus-project/voting-prototype

  Code pushed to this room from MMOLLM will mirror to the public
  GitHub repository. Commits are attributed to your public persona
  unless you configure otherwise.

  The room's world-log includes commit messages, PR discussions,
  and architectural decisions. This record is part of the public
  repo's documentation.

  By participating in this room, your contributions become part of
  a public codebase under the project's license (MIT).</span>

  <span style="color: #00e5ff;">&gt; /rules for the full collaboration manifest</span>

do you accept? [y/n]
</pre>

A accepts and enters the room. The room context loads, including the current state of the codebase and the recent activity log. A\u2019s personal stack is integrated: their configured tools, their preferred patterns, the architectural opinions accumulated in their private context.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #64b5f6; font-weight: bold;">[consensus/0.3] 7 participants active</span>
sync: branch main | 142 commits | 11 open issues | 3 open PRs

recent history:
  - anonymous#b3f9 opened PR #14: "add delegation weights to
    quadratic voting model" (4hr ago, 1 approval)
  - anonymous#e72a raised issue #15: "conviction buffer does not
    decay on abstention" (2hr ago)
  - the room voted on naming convention for vote types:
    "Ballot" vs "Proposition" vs "Signal" : no consensus yet
    (this is funny and the room knows it)

your pending reviews: PR #12, PR #14

<span style="color: #64b5f6;">your context stack notes:</span>
  - <span style="color: #888;">you have argued for ranked-choice fallback in previous sessions</span>
  - <span style="color: #888;">your last commit (6 days ago) refactored the tally function</span>
  - <span style="color: #888;">your inner layer is bound to 3 other participants in this room</span>
</pre>

A pulls the latest state and looks at what has changed since their last session. The room\u2019s LLM mediates code review, architectural discussion, and the social logic of the project. When two participants disagree about the delegation model, the LLM does not resolve the disagreement. It helps each side formalize their argument. The room\u2019s world-log accumulates design decisions, rejected approaches, and the reasons behind them.

<pre style="background: #111; color: #e0e0e0; padding: 1.25em; border-radius: 6px; font-family: 'Liberation Mono', monospace; font-size: 9.5pt; line-height: 1.4; overflow-x: auto; border: 1px solid #333; margin: 1.25em 0;">
<span style="color: #00e676;">&gt; what changed in the conviction module while I was out?</span>
</pre>

The LLM responds, drawing on the room\u2019s world-log and A\u2019s personal context to surface what is relevant to them specifically. Another participant in the room with a different configured stack would get a differently weighted answer to the same question.

The room persists whether anyone is in it or not. PRs get reviewed asynchronously. The world-log accumulates. The GitHub repo is a snapshot of one layer of the room\u2019s activity, but the room itself contains things the repo cannot capture: the discussions that did not result in code changes, the rejected alternatives, the shared understanding that never made it into a comment thread.

---

## END OF SCRIPT

What this script demonstrates that a deck cannot:

- The room discovery is mediated by personal context, not a catalog
- Room configs are readable and forkable, not terms of service
- Character creation is a negotiation, not a dropdown menu
- The boundary between player and character is intentionally porous
- The world-log makes the space feel inhabited even when you are alone
- Dormant characters become part of the environment
- Imperfection and contradiction are structural, not bugs
- The platform does not route toward productivity or consensus
- Two people with different configured stacks experience the same room differently
- Git integration is not an afterthought: the dark room is the primary medium, the repo is a public export of one layer
- Returning to a room you already know surfaces different information than entering one for the first time
- The same infrastructure supports fantasy roleplaying and consensus protocol design
