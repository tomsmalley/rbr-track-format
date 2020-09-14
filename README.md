# Reverse Engineering the RBR track format

This format has already been reverse engineered in order to create the
Wallaby track creation tool, but the knowledge is kept secret.

## Progress

The following definitions are from the Wallaby manual or Tracks.ini:

track.bws
: [Not Started]
: Brake wall system, doesn't seem to be present

track.col
: [Not Started]
: Static colliders, including ground

track.dls
: [WIP] The rough structure is done. Haven't figured out the purpose of all structures yet.
: Scripts (animations) and cameras

track.fnc
: [Not Started]
: Fence data (tapes, nets, pole fences)

track.ini
: [Not Started]
: Texture information

track.lbs
: [Not Started]
: Track geometry and settings

track.mat
: [WIP]
: Physical surface definitions based on textures

track.trk
: [Not Started]
: Driveline definition, dynamic physics objects

track_textures.rbz
: Textures

## Workflow

I'm using the 010 editor for it's hex template capabilities. The `templates` directory contains the templates for a particular file extension.

At some point, when enough is figured out, I intend to write some tools for working with these formats.