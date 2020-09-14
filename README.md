# Reverse Engineering the RBR track format

This format has already been reverse engineered in order to create the
Wallaby track creation tool, but the knowledge is kept secret.

## Progress

The following definitions are from the Wallaby manual or Tracks.ini:

__track.bws__\
Brake wall system\
[Not Started] Doesn't seem to be present. I also don't know what this means, but I've seen references to it in ghidra.

__track.col__\
Static colliders, including ground\
[Not Started]

__track.dls__\
Scripts (animations) and cameras\
[WIP] The rough structure is mostly done. Haven't figured out the purpose of all structures yet.

__track.fnc__\
Fence data (tapes, nets, pole fences)\
[Not Started]

__track.ini__\
Texture information\
[Not Started]

__track.lbs__\
Track geometry and settings\
[Not Started]

__track.mat__\
Physical surface definitions based on textures\
[WIP] This is a small file, just needs some extra testing. The 16x16 arrays define material IDs across the surface of a texture.

__track.trk__\
Driveline definition, dynamic physics objects\
[Not Started]

__track_textures.rbz__\
Textures

## Workflow

I'm using the 010 editor for its hex template capabilities. The `templates` directory contains the templates for a particular file extension.

At some point, when enough is figured out, I intend to write some tools for working with these formats.