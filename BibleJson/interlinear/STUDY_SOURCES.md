# Word-study data and modifications

Checked 20 October 2026.

## STEP Bible

Credit: [STEP Bible](https://www.stepbible.org), originally Tyndale House Cambridge.
[Data repository](https://github.com/STEPBible/STEPBible-Data);
[CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).

Existing bundled resources: TAHOT (Hebrew/Aramaic token text and morphology),
TAGNT (Greek amalgamated text with edition flags), TBESH (abridged BDB),
TBESG (corrected Abbott-Smith where available and supplementary entries),
TEHMC/TEGMC (morphology expansions). These are not unabridged standalone BDB or
Abbott-Smith editions. The original import did not record upstream commits.

Existing conversion: compressed positional JSON, source HTML changed to simple
markup, Hebrew cantillation removed, stressed Hebrew transliteration reformatted,
selected NA28/TR variant handling, Psalm headings attached to verse 1 for display.
New indexes preserve the extended identifier and distinguish Greek edition and
Psalm heading. Source bytes are fingerprinted in study_manifest.json.gz.

## Strong / Open Scriptures

[Greek source](https://raw.githubusercontent.com/openscriptures/strongs/master/greek/strongs-greek-dictionary.js)
and [Hebrew source](https://raw.githubusercontent.com/openscriptures/strongs/master/hebrew/strongs-hebrew-dictionary.js).

Greek JSON: Copyright 2009, Open Scriptures. CC-BY-SA. XML preparation:
Ulrik Petersen (2006).
Hebrew JSON: Copyright 2010, Open Scriptures. CC-BY-SA. Hebrew source/corrections:
David Instone-Brewer; editing and Unicode transliterations: David Troidl.

The digital files explicitly carry CC-BY-SA, without a version in their headers.
The old import's blanket “public domain” claim was inaccurate for this edition.
Historical works: James Strong, Greek dictionary (1890), Hebrew dictionary (1894).
Existing derived assets preserve source definitions, pronunciation, derivations
and KJV usage. This upgrade adds attribution and does not reimport these files.
Resolve the digital license version, share-alike obligations and exact original
snapshot before distributing a new release; this audit does not claim clearance.

## Princeton WordNet 3.0

Copyright 2006 Princeton University. The complete notice and disclaimer are in
wordnet_LICENSE.txt. Official archive, checksum, transformation and headword
counts are in wordnet_manifest.json.
[License](https://wordnet.princeton.edu/license-and-commercial-use).

Converted to first-letter gzip JSON shards. Glosses/examples remain verbatim;
underscores in headwords become spaces; lookup keys are lowercase. Used only for
English language assistance, not for assigning biblical lemma meanings.
No external service is required after installation.

## Kiswahili and editorial explanations

Nine paired English/Kiswahili lexical summaries are AI-assisted editorial drafts
based on specific bundled STEP entries, not verified academic translations.
The source wording is retained separately. No reviewer has certified these
summaries. The terminology help is also project-authored and pending review.
Existing Kiswahili token glosses came from a prior gloss-map import; neither
the map's provenance nor a linguistic reviewer was recorded. The UI identifies
this limitation. Presence of a Swahili field is not proof of accurate translation.

[Kalebu/kamusi](https://github.com/Kalebu/kamusi) was evaluated but NOT bundled.
Its MIT repository license does not establish permission from the dictionary
whose content the README says was scraped from kamusi.appsmata.com. General
Kiswahili dictionary coverage remains limited to the installed study glossary.

## Reviewed occurrence notes

No reviewed contextual or historical notes are installed. The occurrence layer
is deliberately empty. Future records must identify the source token, attached
part, extended lexeme and edition; reviewed status requires reviewer and evidence.
Source glosses and morphology remain usable offline in the meantime.
