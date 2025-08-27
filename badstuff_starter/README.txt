Bad Stuff — MCreator Starter Pack
=================================
This ZIP includes placeholder textures, language entries, and two recipes you can import into your MCreator workspace to speed things up.

What’s inside:
- assets/badstuff/textures/item/*.png     (seed, leaves, dried leaves, cigarette, cigar)
- assets/badstuff/textures/block/*.png    (drying rack faces)
- assets/badstuff/lang/en_us.json         (pretty names + creative tab label)
- data/badstuff/recipes/*.json            (cigarette, cigar)

How to use in MCreator:
1) Open your workspace → Resources.
2) Click "Import textures" → point to assets/badstuff/textures/item and block folders. Assign them to the items/blocks when you create them.
3) Click "Import language" → choose assets/badstuff/lang/en_us.json (MCreator will merge keys).
4) Optional: Import the recipes via "Resources → Data pack entries → Import" (or recreate via GUI using these JSONs as reference).

Recommended registry IDs:
- Items: tobacco_seed, tobacco_leaves, dried_leaves, bad_cigarette, bad_cigar
- Block: drying_rack
- Creative tab: bad_tab

Next steps in MCreator (high level):
- Create Plant (tobacco_crop) with 8 stages; seed item = tobacco_seed; drops leaves + chance of extra seeds.
- Create Block (drying_rack) with 2-slot inventory, GUI, and tick procedure: leaves → dried_leaves over ~10s.
- Create Items (bad_cigarette/bad_cigar) with “when eaten” procedure: apply Resistance, wait, then Slowness.
