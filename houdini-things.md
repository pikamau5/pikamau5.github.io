# Potati's Houdini Things

- [VEX - cheat sheet](https://www.tokeru.com/cgwiki/VexCheatSheet)

- [VEX - attributes](https://www.sidefx.com/docs/houdini/vex/snippets.html#attributes)

- [HDA - Populating an  ordered menu with a script](https://brendandawes.com/blog/creating-houdini-menus)

- [VEX - more vex snippets](https://github.com/Kuchavo/VEX-Snippets)

- [HOUDINI - event callbacks](https://80.lv/articles/template-flag-kitty-using-event-callbacks-in-houdini/)

## Vex snippets
### list detail attributes
`s[]@detailattribs = detailintrinsic(0,"detailattributes");`
### group attr
`@group_name == 1`

## Expressions (needs backticks?)
### Input
`opinputpath(".", 0)`
### The last point
`npoints(opinputpath(".", 0))-1`
### input node detail attrib
`detail(opinputpath(".", 0), "_upstream_error", 0)`
### Use cop node as texture path
``op:`opfullpath("../cop")` `` 
### reference another node / objnet
`opfullpath("../objnet1")`
### files embedded to hda
`opdef:.?filename.png`
`opdef:../..?leaf.png`
### not sure what this is, might be useful?
`run("opglob @smart_bundle_object")`

### Syntax
*,^N = all except N
