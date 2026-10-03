# Hey Nabu, for a platform administrator

Read this only when your token lists tools that change experts. A reader's token
does not, and nothing here applies to one. The rest of the discipline is in
`SKILL.md` beside this file, and it still holds.

## Curating a corpus

A platform administrator's token lists fourteen more tools, and nobody else's does:
`list_organisations`, `create_area`, `rename_area`, `update_aperture`, `update_definition`,
`update_rubrics`, `import_sources`, `proposed_sources`, `accept_source`, `dismiss_source`,
`set_feed_status`, `list_clips`, `file_clip`, `discard_clip`. Three more let you go through what an expert holds
and change it: `read_register`, `revise_record`, `review_records`. Four disciplines:

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
