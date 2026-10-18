# Blender Editor Icons

**Open the site: <https://7udwig.github.io/Blender-Editor-Icons/>**

A fast, searchable browser for the **built-in UI icons of Blender** (2.80 – 5.2, 24 versions, 600–790 icons each).
Pick a version, search, change the display size of all icons at once, open an icon to compare it at 16/24/32/48 px on a dark,
light or checkerboard background, and copy its name or the Python line that uses it (`layout.label(text="", icon='ADD')`).

* **Version selector** – each version shows only its own icons, with *NEW* and *GONE IN x* badges, filters for both, and a list of icons removed since the previous version. Only icons that are completely new or gone are marked; redesigns are deliberately not tracked.
* **Nothing is stored or sent** – no cookies, no local storage, no analytics, no external requests. The address (`#v=4.2&k=ADD`) only carries the current version, search and opened icon so a link can point to it.
* **No tint** – Blender does not let a script recolour its icons, so the tint control is hidden here.

## Where the data comes from

The icons are read from Blender's git history. For the first release of every series:

* up to 4.2: `release/datafiles/blender_icons32/icon32_<name>.dat` – raw 32x32 RGBA pixels, converted to PNG,
* from 4.3: `release/datafiles/icons_svg/<name>.svg` – one vector file per icon.

The icon name is the Blender identifier without the `ICON_` prefix (`add.svg` -> `ADD`).
Blender before 2.80 stores its icons differently and is not covered. The tool icons of the toolbar (`release/datafiles/icons`) are not included.

## License

* The icons are part of the Blender source code, which is released under the GNU General Public License. See `LICENSE-BLENDER-ICONS.txt`.
* The code of this site (everything else) is MIT licensed, see `LICENSE`.

This is an unofficial project, not affiliated with or endorsed by the Blender Foundation. "Blender" is a registered trademark of the Blender Foundation; the Blender logo is not used here.
