# Verification summary — R1

KiCad CLI 10.0.5 DRC: zero reported items for these designs. An independent Gerbonara parser imported all manufacturing layers and drills. Shapely comparisons checked the source artwork against the exported Gerber polygons. Dimensions below are measured from native outline centerlines.

| Design | DRC items | Min. copper to edge mm | Min. silkscreen to mask opening mm | Material between hanging hole and edge mm | Lowest source/Gerber vector IoU |
| --- | --- | --- | --- | --- | --- |
| DIYIPCB Christmas Tree PCB Badge | 0 | 2.426 | 0.220 | 1.560 | 0.99999895 |
| DIYIPCB Reindeer PCB Badge | 0 | 1.589 | 1.330 | 2.032 | 0.99999878 |
| DIYIPCB Snowman PCB Badge | 0 | 0.549 | 0.220 | 1.573 | 0.99999882 |

There is one Ø3.2 mm NPTH per design and no PTH holes. Both copper layers contain decorative artwork; the layers do not require an electrical interconnection.

KiCad skill PCB and Gerber analyzers were also run. Their layer-envelope alignment warnings were reviewed: local copper artwork intentionally has a different bounding box on each side. Exact coordinate/polygon comparison and visual overlay checks passed, so these bounding-box warnings were treated as false positives. Source artwork and manufacturing data are aligned.

These checks cover file consistency and geometry, not physical sampling or a particular factory's complete DFM process. Router capability, white ink coverage, small negative legend detail, final colors, surface durability and mounting strength have not been tested on physical boards. Artwork cleanup parameters were 0.30 mm copper and 0.15 mm silkscreen circular morphology; these are cleanup parameters rather than a certified minimum width at every local point. Use factory CAM review before production.

No schematic/ERC, SPICE, EMC, thermal or component lifecycle analyses were applicable: these passive decorations contain no electronics, signal nets or power circuits. No reuse license has been selected.
