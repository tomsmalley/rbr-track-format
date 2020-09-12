# Reverse Engineering the RBR track format

This format has already been reverse engineered in order to create the
Wallaby track creation tool, but the knowledge is kept secret.

## Track Files

The following definitions are from the Wallaby manual or Tracks.ini:

- track.bws: Brake wall system, doesn't seem to be present
- track.col: Static colliders, including ground
- track.dls: Scripts (animations) and cameras
- track.fnc: Fence data (tapes, nets, pole fences)
- track.ini: Texture information
- track.lbs: Track geometry and settings
- track.mat: Physical surface definitions based on textures
- track.trk: Driveline definition, dynamic physics objects
- track_textures.rbz: Textures

## Workflow

I'm using the 010 editor for it's hex template capabilities. The `templates` directory contains the templates for a particular file extension.