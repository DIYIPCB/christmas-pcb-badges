# DIYIPCB Christmas PCB Badges

Design and fabrication files for 3 decorative Christmas PCB badges. Revision R1, 2026-11-25.

These are passive, double-sided FR-4 ornaments with decorative copper on both sides, white silkscreen, and a hanging hole. They have no electronic components or powered functions. Product pictures below are renderings generated from the exported fabrication layers.

| Design | Outline envelope, W × H | Solder mask / silkscreen | Files |
| --- | --- | --- | --- |
| DIYIPCB Christmas Tree PCB Badge | 51.97 × 64.94 mm | green / white | [KiCad](designs/diyipcb-tree) · [Gerber ZIP](gerbers/diyipcb-tree-gerbers.zip) |
| DIYIPCB Reindeer PCB Badge | 61.98 × 60.82 mm | red / white | [KiCad](designs/diyipcb-reindeer) · [Gerber ZIP](gerbers/diyipcb-reindeer-gerbers.zip) |
| DIYIPCB Snowman PCB Badge | 38.38 × 64.84 mm | red / white | [KiCad](designs/diyipcb-snowman) · [Gerber ZIP](gerbers/diyipcb-snowman-gerbers.zip) |

## Fabrication

- 2 copper layers, FR-4, nominal 1.6 mm finished thickness.
- 1 oz copper per side, OSP on exposed copper. No HASL or ENIG substitution.
- Same solder mask color on both sides; WHITE silkscreen only on both sides.
- One Ø3.2 mm non-plated hanging hole per badge; routed outline, not a rectangle.
- Concave outline details require a 1.0 mm or smaller router tool. Ask the factory to review the profile and large white legend fills in CAM.
- Front/back copper, mask openings and silkscreen are supplied, plus board outline and drills. No component assembly, solder paste or stencil is needed.
- Files use normal top-view PCB coordinates. Do not manually mirror bottom Gerber files. Back images are shown from the outside after flipping the physical board.
- Cord, lanyard, pin backing and other mounting hardware are not included in this design.

The snowman is RED soldermask with WHITE silkscreen filling the white body areas. Its red outlines, face and DIYIPCB lettering are gaps in the white ink, revealing the red soldermask underneath. There is no red silkscreen and no white soldermask. Copper buttons remain OSP openings. Preserve the large white ink polygons and negative details during CAM preparation.

## Folder guide

- `designs/`: editable KiCad 10 PCB and project files.
- `fabrication/`: individual manufacturing layers, drills and factory notes for each design.
- `gerbers/`: one ready-to-submit fabrication ZIP per design.
- `images/`: front/back previews of manufacturing output.
- `docs/verification.md`: check summary and limitations.
- `SHA256SUMS.txt`: checksums for the design and fabrication files.

The design files require KiCad 10 or newer. The Gerber files can be used independently of KiCad. Submit each design ZIP separately; no combined factory panel is included.

## Finished badges

- [DIYIPCB Christmas Tree PCB Badge](https://www.diyipcb.com/product/diyipcb-tree-pcb-badge/)
- [DIYIPCB Reindeer PCB Badge](https://www.diyipcb.com/product/diyipcb-reindeer-pcb-badge/)
- [DIYIPCB Snowman PCB Badge](https://www.diyipcb.com/product/diyipcb-snowman-pcb-badge/)

## 中文说明

本仓库提供圣诞 PCB badge 的 KiCad 设计源文件和 Gerber 制造文件。采用双面 FR-4、1.6 mm、双面 1 oz 铜、OSP、白色丝印和 Ø3.2 mm 非金属化挂孔。正反两面均有图案，无电子元件及通电功能。请按异形板框铣边，不要按矩形外框加工，也不要删除装饰铜岛或大面积丝印。图中铜色和油墨颜色为示意，以样板为准。

雪人采用红油白字，白色区域用白丝印铺底，轮廓、表情和文字通过丝印留空露红油实现，不使用红色丝印。

PCB 源文件与制造层已经过 KiCad DRC 和独立 Gerber 几何一致性检查；尚未实物打样，生产前须由板厂 CAM 确认白墨覆盖、负形细节和异形轮廓加工能力。每款 Gerber ZIP 分别提交，没有工厂拼板及佩戴配件。

## License

No license has been specified for this repository. Public availability of files does not by itself grant a reuse license. Brand names and marks belong to their respective owners.
