# Module 7 Activity 7.1 — Find Your Community Connection

A self-contained, accessible GitHub Pages activity for the Climate-Resilient Gardening mini course.

## Publish on GitHub Pages

1. Create or open the repository for this activity.
2. Upload `index.html` to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Deploy from the `main` branch and `/ (root)` folder.

No build step or external libraries are required.

## Garden Journal integration

When the learner completes the activity, the activity automatically writes a structured entry to browser `localStorage`.

Primary journal object key:

`climateResilientGardenJournal`

Entry ID inside `journal.entries`:

`module7_activity7_1_community_connection`

A second copy is also written directly under the key:

`module7_activity7_1_community_connection`

The stored entry contains:

- Module and activity number
- completion timestamp
- selected interests
- discovery route used
- selected group/project/network
- what people are doing together
- why the work matters to the learner
- whether the connection is broader than local

Because GitHub Pages repositories under the same `https://USERNAME.github.io` domain share an origin, a Garden Journal hosted under another repository path on that same GitHub Pages domain can read this entry from `localStorage`.

The Garden Journal will need a corresponding Module 7 reader/display component for this entry. This package saves the data now so the journal can be updated separately without changing the learner activity.
