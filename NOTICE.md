# Notice — third-party content in `bindings.db`

`bindings.db` is published as a release asset of this repository and is
downloaded by DTstudio on first run. **It is not part of the DTstudio
application and it is not covered by the DTstudio End User Licence
Agreement.** The content described below keeps its own licences, and those
licences prevail; nothing in the EULA restricts a right they grant you.

## What is inside

The database is built from the [Linux kernel](https://www.kernel.org/) tree,
at **v7.2-rc5** (commit `fc46aed51f6280801f43a2cf4b5060cc33b572f9`,
2026-07-29):

| What | Where it comes from | How many |
|---|---|---|
| Device tree sources, stored **verbatim** (compressed), each with its own SPDX header intact | `arch/*/boot/dts/**` and `include/dt-bindings/**` — 3 627 `.dts`, 2 722 `.dtsi`, 1 241 headers | 7 590 files |
| Binding schemas, processed into JSON, keeping the binding's own description text | `Documentation/devicetree/bindings/**.yaml` | 5 663 schemas, 5 349 bindings, 25 458 declared compatibles |
| Hardware index (SoCs and boards) derived from those sources | the same `.dts`/`.dtsi` files | 703 SoCs, 2 980 boards |

## Licences

The stored files carry the licence stated in their own SPDX header. Over the
7 590 files, the identifiers found are, most common first:

```
1468  GPL-2.0                        396  (GPL-2.0 OR MIT)
1254  (GPL-2.0+ OR MIT)              356  GPL-2.0-or-later OR MIT
 762  GPL-2.0-only                   355  BSD-3-Clause
 441  (GPL-2.0-only OR BSD-2-Clause) 327  GPL-2.0+
 407  GPL-2.0-or-later               674  no SPDX header
```

Where a file offers a choice of licences, you may take either.

- GNU General Public License, version 2:
  <https://www.gnu.org/licenses/old-licenses/gpl-2.0.html>
- The kernel's own licensing rules and full licence texts:
  <https://www.kernel.org/doc/html/latest/process/license-rules.html> and the
  `COPYING` and `LICENSES/` files of the kernel tree.

Copyright in these files belongs to their respective authors, as stated in
each file. Extracting any of them from the database — which is what DTstudio
does when it opens a tree from the catalogue or compiles one — gives you the
file as it is in the kernel, headers and all.

## Where to get the originals

<https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git>, at the
commit above.

## The rest of this repository

The README, the screenshots under `assets/` and the DTstudio packages are
part of DTstudio and are covered by its End User Licence Agreement, shown on
first run and available from *Help → Licence agreement* inside the
application.
