# Notice — `bindings.db`

`bindings.db` is published as a release asset of this repository and is
downloaded by DTstudio on first run. It is not part of the DTstudio
application and it is not covered by the DTstudio End User Licence Agreement.

## Third-party content

The database is built from the [Linux kernel](https://www.kernel.org/) tree
(v7.2-rc5): the device tree bindings under
`Documentation/devicetree/bindings/`, the `.dts`, `.dtsi` and
`include/dt-bindings/` sources, and data derived from them.

The kernel files stored in the database keep their own licences — GPL-2.0 and
variants, several of them dual-licensed with MIT or BSD — as stated in the
`SPDX-License-Identifier` header of each file, which is preserved inside the
database and comes out with the file whenever DTstudio extracts it. **Those
licences prevail over anything in this notice or in the DTstudio agreement,
and nothing here restricts a right they grant you.** Where a file offers a
choice of licences, you may take either.

- GNU General Public License, version 2:
  <https://www.gnu.org/licenses/old-licenses/gpl-2.0.html>
- The kernel's own licensing rules and full licence texts:
  <https://www.kernel.org/doc/html/latest/process/license-rules.html>, and the
  `COPYING` and `LICENSES/` files of the kernel tree.
- The original sources:
  <https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git>

Copyright in those files belongs to their respective authors, as stated in
each file.

## Rights in the database itself

The licences above cover the kernel files. They do not cover **this
database** — its selection and arrangement of that material, its schema, its
processed binding schemas, its hardware index and the rest of the work that
turns a kernel tree into it. That compilation is the work of the DTstudio
author, © 2026, all rights reserved, and in the European Union it is also
protected as a database under Directive 96/9/EC, independently of the licence
of its contents.

`bindings.db` is supplied for use with DTstudio. Without written permission
you may not extract or re-use a substantial part of it — by volume or by
value — for anything else, nor redistribute it, republish it, or make it
available as a dataset, service or product of your own, whether whole,
in part, or repackaged in another format.

This does not touch your rights over the kernel files themselves: those you
may take, use and redistribute under their own licences, from here or from
the kernel tree they come from.

## The rest of this repository

The README, the screenshots under `assets/` and the DTstudio packages are part
of DTstudio and are covered by its End User Licence Agreement, shown on first
run and available from *Help → Licence agreement* inside the application.
