# Imani za Msingi — app content

Content for the **Imani za Msingi** and **SDA Fundamental Beliefs** apps.

To keep the apps small, most Bible versions, the Greek/Hebrew study tools,
the English dictionaries and the hymn sheets are not built into the apps.
The apps download them from this repository's releases the first time
they're needed (or in the background on Wi-Fi), check each file's SHA-256
against the list built into the app, and keep them for offline use.

The rest of the app content is also stored here as a backup.

**Do not edit, replace or delete files in a published release.** Each app
version pins one release (`content-v1`, `content-v2`, …) by file checksum.
To change content, publish a new release with
`tools/content/build_content.py --tag content-vN --publish` in the app
repository.

## Layout

| Folder | Content |
| --- | --- |
| `BibleJson/versions/` | Bible versions (gzipped JSON) |
| `BibleJson/interlinear/` | Greek/Hebrew interlinear, lexicons, concordances, WordNet shards |
| `BibleJson/headings/`, `BibleJson/crossrefs/` | Section headings and cross-references |
| `webster/` | Webster's Unabridged Dictionary (1913) |
| `kamusi/` | Kamusi ya Kiswahili |
| `Songs/` | Hymnal indexes and Nyimbo za Kristo hymn sheets (PDF) |
| `beliefs/` | The 28 Fundamental Beliefs (English and Kiswahili) |

## Sources and licences

The licences below come from the original sources. Texts shared under
Creative Commons keep that licence here.

**Bibles**

- King James Version, American Standard Version (1901), Young's Literal
  Translation (1898), World English Bible, Berean Standard Bible, Biblia
  Takatifu 1850 (Kimvita): public domain.
- Neno: Bibilia Takatifu: Copyright © 1984, 1989, 2009, 2015 Biblica, Inc.
  CC BY-SA 4.0. Text from eBible.org.
- Neno: Maandiko Matakatifu: Copyright © 2018, 2024 Biblica, Inc.
  CC BY-SA 4.0. Text from eBible.org.
- Swahili Unlocked Literal Bible: Copyright © 2019 Door43 World Missions
  Community. CC BY-SA 4.0. Text from eBible.org.
- Biblia Takatifu (Swahili Union Version).

**Study tools** (details in `BibleJson/interlinear/STUDY_SOURCES.md`)

- STEP Bible data (Tyndale House Cambridge): CC BY 4.0.
- Strong's dictionaries, Open Scriptures digital edition: CC BY-SA.
- Princeton WordNet 3.0: © 2006 Princeton University, see
  `BibleJson/interlinear/wordnet_LICENSE.txt`.

**Dictionaries**

- Webster's Revised Unabridged Dictionary (1913): public domain.
