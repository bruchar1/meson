## Introspection: Dump ast of subdir as well

`meson introspection --ast meson.build` now dumps AST for every meson.build
from subdirs. It returns a dict where keys are paths to meson.build files,
and values are the AST for those files. Previouly, only AST for the
root meson.build file was dumped.
