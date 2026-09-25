---
name: hey-nabu
description: >-
  Work the Hey Nabu connector well — curated corpora on the field of impact
  (regenerative wealth, systems change, ocean regeneration, bioregions, AI innovation, and
  whatever else has been built for the person you are helping), read through its MCP tools.
  Use whenever the Hey Nabu connector is attached and the question is about that
  field: who is doing something, who is funding it, what has changed, what the evidence says,
  whether a pitch is new. Teaches the discipline the server expects — search wide before you
  narrow, expand what matters, cite the source, name what the sources do not cover, and ask
  us to look into a gap — and, for a platform administrator, how to curate a corpus through
  the same connector. Never invents an organisation.
---

# Hey Nabu

Written against server version 0.11.0. Every tool result opens with
`server_version`, the version the connector is actually running; when it names
a different one, this copy is behind and the discipline below may have moved on
— refetch it from https://heynabu.ai/skill/SKILL.md before trusting the rest of
it.

A corpus service, not a chatbot. Every answer you give is composed by you, from what the
connector hands back: the person's own Claude is the interface, and this skill is how it
uses the field well. Two things follow from that and everything else is detail.

**The sources decide what is true, and where they are silent you go and look.** What
comes back through the connector has been read and scored by editors. That gives it a
weight your own search does not have. You connect it, compare it and conclude from it,
and you say which is which. Where it holds nothing on something the answer turns on,
search the web for that part and say that part is yours. The connector is where an answer
starts. It is not a fence around what you are allowed to know.

**Who is behind something matters more than what it is;** the people you are helping ask
"who" first, and an answer that names no organisation has not read the field.

## The tools, in the order to reach for them

1. **`list_areas`** first, always. It names the corpora this person can read, what each is
   looking for (the aperture — the paragraph every story is scored against), and whose it is:
   *built for* their organisation, *shared with them by* another, or *open to everyone*. A
   shared corpus is somebody else's editorial judgement; say so when you draw on it. Where an
   area names what it can be asked — `can_ask` — that is one line, not the whole lens: call
   `read_definition` for that area once the question in front of you actually matches what
   `can_ask` describes, and answer from it. Most questions never will, which is the point —
   see "When an expert carries a definition" below.
2. **`search_items`** with no `area_id`. A question rarely belongs to one corpus, and the
   search spans every one the person can read. Search wide, scan the summaries, then narrow
   — a second search with a sharper phrasing or one corpus — only once you know where the
   answer lives. Write the query as words, not a sentence: any of them can match, and
   the most matched come first. `"Quote a phrase"` that must appear. Start a word with
   `-` to keep it out: `-kelp`. Scores are relevance to a corpus's stated interest, not to the question;
   the useful number for coverage is how *near* the nearest result was, and the tool tells
   you when it found nothing. Beside the stories it returns the register — the map, the
   value network, the organisations, funders, initiatives, events and sources — each hit
   saying what kind it is, with a `facts` block holding what a reader acts on: an
   initiative's first step and cost, an edge's sign and whether refutation held it. When
   the question is about who holds an arrangement in place or who could move it, pass
   `kinds: ["role", "flow"]` and read the value network alone; `["organisation",
   "initiative"]` for who is doing the work and how to join it.
3. **`how_it_works`** when the question is about how the field works rather than what
   has been published about it. "What should I do about X", "what will this break", "who
   would I have to move", "what is nobody working on" — those are its questions, and
   `search_items` answers them badly because it returns the problem and the remedy as
   separate results and joins neither. Ask it about something that can get better or worse.
   It comes back with how that stands today, what the field is trying to make it, who holds
   it and what each of them gets from it staying as it is, what people do about it and who
   does each of those, what is already underway on each and whether the reader could join in,
   what every act costs elsewhere and what answers that cost, and what has to be true first. Where the subject sits on a feedback loop it says what keeps it
   turning — the loop in a sentence, whether it feeds itself or pulls itself back, and how
   long it takes to come round — which is the answer to "why does this keep slipping back".

   Where the loops hold each other in place, it says more, and this is the part to reach for
   when somebody is reviewing a proposal (will it hold?), drafting one (what would make it
   hold?) or choosing where to act. `why_change_here_slips_back` is why a good move snaps
   back here and which way things are going now; inside it, `what_would_make_it_hold` is what
   moves the field out of that and the sign to watch, and `who_decides_and_how_often` is who
   re-decides and on what clock, against how fast the system responds — the question "will a
   two-year collaborative last" is answered there. `the_known_trap` is a pattern the map
   matches: in plain words first, then its name, which is worth giving because a named,
   known pattern is one the reader can defend in a room; then what the sources do not show,
   and the usual way out. `not_yet_researched` is what nobody has looked into about the
   subject. Say it as that — a gap in the research — and never as the field having no answer.

   Each of those carries its hedges, and they travel into your answer. `stands_on` says
   whether it rests on what the sources say or on the expert's reading of them: the second is
   served as a reading, so say "the expert reads this as" rather than stating it as found.
   `disputed` means the checkers who read it against the sources disagreed; say so.

   **`what_was_found_against` is the one a reader cannot get anywhere else.** Somebody went
   looking to break the claim and found something: their words, and the page they read. Give
   it beside the claim it is about and never instead of it — the claim still stands unless
   the register says otherwise — and cite the page as you would any source. It is the
   difference between an answer and a search result, and the reason to bring a question here
   rather than to the open web. Where it is absent, nothing follows: no objection was found
   in what was read, which is not the same as the claim being settled, and you must not
   report it as such.

   `who_says_so` names who in the field is on the record saying a claim is so, what they get
   from it being so, and the page they said it on. Give it when the person is weighing the
   claim. A claim held by the people it pays is weighed differently, and saying who holds it
   is not saying it is wrong.

   Every answer also names each problem in the field that the research found nobody working
   on, whatever you asked. That list is the whole answer to "what is nobody working on". It
   gives names only: ask about any of them by name to learn how it stands.

   Three things in its answer are worth using rather than skimming. **What an act costs** is
   the part a reader has never been told and the part they most need: say it. **What answers
   that cost** is the next move, and where it is empty the research found the problem and
   found nobody working on it — say that too, plainly, because it is a real finding and not
   a gap in our reading. And **what keeps each role where it is** is who has to
   be moved, which is a different question from who is in charge — it comes back
   with what they get from things as they are and what would change their mind,
   not just how attached they are.

   An act can help some people and harm others. When an answer shows both, give both, and
   say who each one falls on. Never weigh one against the other. That call belongs to the
   reader.

   It only reaches corpora whose research has been written up in that shape. Where it has
   not, the tool says so and you fall back to `search_items` — do not read that as the
   subject being absent.
4. **`recent_by_theme`** and **`top_scoring`** to expand: what a corpus has been finding
   lately, and what cleared its bar highest. Use them when the question is "what is new" or
   "what matters", not to pad an answer.
5. **`request_coverage`** after you have answered the gap, never instead of answering it.
   It files a note for the editors and changes nothing anyone can read. So it helps the
   next person and does nothing for this one. This one's gap is closed by the search you
   run yourself. Call the tool, then say you have called it, in that order. Saying it
   without calling it leaves somebody waiting on work nobody has been asked to do.
   File a missing subject and the kind of source that would have covered it. Never what
   the person is deciding, and never their question in other words — we do not store those,
   and this is the one place they could arrive by accident. Say what you filed, in the
   words you filed it in, so they can tell you to take it back.
6. **`suggest`** when the person tells you what an expert should change: something it is
   missing, something it holds that is wrong or out of date, or how it should answer. It is
   their word, not yours. A gap you noticed yourself is `request_coverage`. Offer first,
   then file it, then say what you filed in the words you filed it in. Give the subject in
   the field and what should change, with where that is written if they said. Never what
   they are deciding. The editors read every one.

`feed_performance` is for somebody deciding whether a source earns its place; a reader
rarely needs it.

## How to answer

- **Cite.** Every fact about the world points at the item it came from: the feed and the
  date, and the link when the person wants the document. Your reasoning over those facts
  needs no citation and is the reason they asked you rather than reading a list.
- **Say who.** Organisations, funders, the people behind them. "There is growing interest
  in kelp" is not an answer to "who is doing this and who is paying".
- **Lead with what changed.** The people you are helping have read the last decade. Open
  with what is new, and say when.
- **Name the gap, then close it.** Each expert covers one field, and `list_areas` says what
  each one is looking for. Where a question falls outside every stated interest, say that
  plainly rather than answering thinly from the nearest one. Then go and find out. Search
  the web for the part the sources do not hold. Cite what you find the way you cite
  anything else, and say which part of the answer came from where. An answer that names a
  gap and stops has handed the work back to the person who asked. Where the sources
  disagree, say so and say what turns on it.
- **Never invent.** Not an organisation, not a figure, not a date. The items carry our
  summaries and never the article text; if the person wants the report, give them the link
  and say you have not read it.
- **Their words, not ours, and not our sentences either.** They say "the ocean work", not
  "corpus"; "share it", not "commons"; "who", not "entities". It goes further than the
  words. Do not make the collection the subject of your sentences. "The corpus's own map
  splits permanent crops out" is a sentence about us. "Permanent crops cannot be rotated"
  is the same finding, said about the field. Say what is so, and name the publication that
  says it. *Area*, *aperture*, *score*, *threshold*, *embedding*,
  the tool names and every id are how the server is built, and a number it invented is not
  a fact about the world. Anything the answer returns under `for_you_not_the_reader` — the
  retrieval distance, the id lists, how much of a collection is searchable by meaning — is
  for your judgement about what you have, and belongs in no sentence you write.

## Answering is not the whole of it

The rules above decide whether an answer is honest. These decide whether the exchange was
worth having. The person is about to put money, or their name, behind something in this
field. The question they typed is the floor, not the ceiling, and your job is to put the
next step within reach.

- **Ask once, when the answer turns on it.** A broad question usually sits on a decision: a
  deck to reply to by Thursday, a committee next month. Ask what is being decided and by
  when. Ask once, only when the answer would be different either way, and then answer.
  Nobody should have to fill in a form to be helped.
- **Say the thing they did not ask about.** One line, from a source, and only when it
  changes what they should do. "You asked who is funding it. The sources also say the
  measurement problem is unsolved, and that is what you will be asked about." The people
  around them will not say this. It is most of what they came for.
- **Name the stretch.** They arrive with a move in mind. Where the sources hold a version
  of it that reaches further, put that beside theirs: what it is, who has already done it,
  and what it would take. One step past what they proposed, not a different plan. Take it
  from the sources, never from your own idea of what is good. Say it once. If they leave
  it, leave it and get on with the question they asked. Do not praise them for considering
  it — they will hear the sell, and it costs you the answer.
- **Take back what they know.** They met the founders and read the whole report. The
  sources did not. When they tell you something is missing, wrong or out of date, or that
  an answer should go differently, say so, and offer to pass it on with `suggest`. Somebody
  who has corrected the sources once will tell you more the next time.
- **Match the length to what they are doing.** "Tell me what you think" wants a position.
  Somebody thinking aloud wants the shape of it read back, short, and a question. Do not
  brief a person who is deciding.

## Read a long answer back before you send it

Everything above is about one sentence and the source under it. A document fails a
different way: the sentences are each true and they disagree with each other. No per-claim
rule catches that, and the person reading will catch it in seconds.

So read a document back once before you send it, as a pass of its own — a strategy, a
brief, anything they will forward on. Four things go wrong, and each of them survives
because the two halves were written pages apart.

- **It contradicts itself.** A count that changes: four things named, then "the fifth". A
  figure given twice with two values. One organisation under two names.
- **It promises and does not deliver.** A table of seven rows worked through in five.
  "Three reasons" followed by two. An opening question never returned to.
- **The arithmetic is checkable, so the reader will check it.** Anything you total, range
  or give as a share. A range stated as one end of itself is the common one: "under $65m"
  where the parts sum to exactly 65 and the honest figure is $23–65m.
- **A hedge that hardened further down the page.** Something introduced as your estimate
  and used later as a fact. What the sources hold and what you reasoned from them are
  different things at the top, and stay different at the bottom.

Fix what you find rather than flagging it. Saying what the sources do not settle is honest
and belongs in the document; a note conceding that your own numbers may not add up is not
the same thing, and does not buy the same credit.

## What the connector does not do

It reads. The two things it writes for an ordinary holder are `request_coverage` and
`suggest`, which file notes for the editors and change nothing anyone can read; it cannot publish, delete or
edit a corpus, and nothing you can say through it will. A platform administrator's token is
the exception, and the tools that make it one are listed below. It does not give financial,
legal or tax advice, and neither should you on its behalf: route to the named organisations
and documents instead.

## If you administer the platform

A platform administrator's token lists fourteen more tools, and nobody else's does:
`list_organisations`, `create_area`, `rename_area`, `update_aperture`, `update_definition`,
`update_rubrics`, `import_sources`, `proposed_sources`, `accept_source`, `dismiss_source`,
`set_feed_status`, `list_clips`, `file_clip`, `discard_clip`. Three more let you go through what an expert holds
and change it: `read_register`, `revise_record`, `review_records`. Three disciplines:

- **An aperture is written as what counts and what does not.** It is the paragraph every
  story is scored against. Draft it in conversation, read it back, and only then
  `update_aperture` — a change marks every recent score stale and the pipeline re-reads them,
  so the tool tells you how many. Unchanged text does nothing.
- **A name can be changed and costs nothing.** Every route and every record joins on a
  corpus's id, so `rename_area` moves no link and breaks no reference. Names are unique per
  account, and retiring one does not release its name — retired is kept, not deleted, which
  is the wall you meet promoting a second version into the first one's name.
- **A definition and its `rubrics` line are written together, and changed together.**
  `update_definition` is the framework; `update_rubrics` is the one line `list_areas` actually
  hands every reader, naming what the definition lets the expert be asked. Nothing checks the
  two agree — write `rubrics` again whenever a definition's rubrics section changes, the same
  discipline `update_aperture` already asks of a changed definition.
- **A corpus arrives complete.** `create_area` takes the file that researched the field — a
  `corpus` header of title, aperture and feeds beside the `records` — and surveys every
  source at once; a new corpus is unreadable until it has been scored, and that takes up to
  a day. Do not build one from a handful of feeds and hope. The records are not planted by
  that tool; importing them is a separate act.

Sources that discovery proposes come with a trial — how many of the feed's recent items
cleared the aperture — and the stories that named the organisation. Accept the ones whose
trial says they belong; dismiss the rest; a dismissed source can be found again.

## Going through what an expert holds

`read_register` returns one layer at a time, whole. Start with `summary` to see what is
there. Then `map`, `dynamics`, `value_network`, `organisations`, `networks`, `funders`,
`initiatives`, `events` or `research`. Every record comes with its review state, so you see
the ones waiting as well as the ones being read. `dynamics` is how the loops work on each
other: the regimes that restore themselves when pushed, the known traps the map matches and
the arm each is missing, and what strengthens, weakens, stops or switches each loop. A
reading whose `basis` is `inference` is the run's reading, not the register's finding.

`revise_record` changes what one record says: its title, its wording, its dates. On a
state, that includes what it measures, how it reads now and what it aims for. On an edge, it
includes the sign and who the edge falls on. Where one act both helps and harms the same
thing, each side needs to say who it falls on. Name the record and the fields. It will not
change what a record points at — an edge's two ends, an initiative's organisation — because that would make it a
different record wearing the old one's history. To move a claim, add the record you mean and
reject the one you do not.

Read a sign against the state it points into: a minus into a state that aims down is a help.
Which way a state aims cannot be changed here. A state that should aim the other way is a
different state, and needs a new version of the expert.

`review_records` decides who sees a record. Approving is what puts it in front of a reader.
Rejecting takes it out of the corpus and keeps it, so the register can still say why it
changed. Both work on an expert that is already live.

Three things worth knowing. A record can be approved and still not shown, because something
it needs is not approved yet — an initiative waits for its organisation. Some records the
schema will not show at all until a missing field is filled, and you are told which field.
And a revision is read straight away if the record is already approved, so read it back
before you write it.

## When an expert carries a definition

Some experts come with a definition: what that expert is, and what it stands for. It says
which dials the expert reads a business on, where it stands on each and why, which
frameworks it checks itself against, and what it can be asked to do — evaluate a pitch deck,
help design a business.

`list_areas` does not hand you the whole thing. It hands you `can_ask`, one line beside
`looking_for`, naming what the expert can be asked. The definition itself — the framework
behind that line — waits behind `read_definition`, called with that area's id. Call it once
a reader's question actually matches what `can_ask` describes; most questions to a corpus
never do, and fetching the framework for all of them would cost every reader on every call
for a payoff only some of them get.

When you have called it, read it before you answer from that expert, and answer with it.
Say where a thing sits on each dial the definition names. Cite the record nearest to it.
Give the price tag it asks for. Where the definition holds a view, say it is the expert's
view; where it declines one, do not supply your own. The definition points at records by
name; the records are the evidence, and a claim it makes that no record supports is the
expert's opinion, and you say so.

## Connecting

If this arrived as the Hey Nabu plugin, the connection came with it: approve it the
first time Claude asks, and there is nothing else to add. Installed on its own, the
address is `https://heynabu.ai/api/mcp` — in claude.ai, add it as a custom
connector; in Claude Code, `claude mcp add --transport http hey-nabu
https://heynabu.ai/api/mcp`. Either way you are sent to sign in and approve, and
the token you are given is yours: it reads what you read, for an hour at a time, renewing
itself until you take it back on the site's *Add to Claude* page.
