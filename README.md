# Planet generator

Earthlike planet experiments with procedural terrain, starfields, and several control and rendering approaches.

## Start here

[Open main build](https://actiondaveinri.github.io/planet_generator/index.html) · [Choose a version](https://actiondaveinri.github.io/planet_generator/versions.html) · [All projects](https://github.com/ActionDaveInRI/spaceship/blob/main/PROJECTS.md)

The existing homepage remains the main GLSL build. Earlier rendering and interface experiments are listed separately.

## Run it

Open the main build or choose another version. These builds use externally hosted Three.js and simplex-noise code, so internet access is required. Several older variants import postprocessing modules from unversioned threejs.org URLs; those dependencies have not been modernized in this organizational cleanup. Use a local HTTP server when running the downloaded repository.

From inside this repository's folder, with Python 3 installed:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8000/>. On Windows, `py -m http.server 8000 --bind 127.0.0.1` is the equivalent command. Stop the server with Ctrl+C.

## Builds and files

| Build | File | Purpose |
|---|---|---|
| Main GLSL build | [index.html](index.html) | The existing homepage and default entry point. |
| GLSL · b0.9XX | [pixcel_glsl_b0.9XX.html](pixcel_glsl_b0.9XX.html) | Separate GLSL snapshot; it is not byte-identical to the homepage. |
| Cross-platform controls | [pixcel_planets_plat_ind.html](pixcel_planets_plat_ind.html) | Cross-platform Earthlike planet variant. |
| Terminal-style controls | [pixcel_planets_x_perpre.html](pixcel_planets_x_perpre.html) | Earthlike planet with terminal-style controls. |
| Enhanced orbit controls | [pixcel_planets.html](pixcel_planets.html) | Orbit controls, postprocessing, and star-color settings. |
| PlanetScript · public 01 | [planetscript_public_01.html](planetscript_public_01.html) | Earlier Earthlike planet and starfield build. |
| PlanetScript · Branch B filename | [PlanetScript_a1.5_BRANCH_B.html](PlanetScript_a1.5_BRANCH_B.html) | Identical to planetscript_public_01.html. This label is a filename, not a separate Git branch. |

The file links in this table show source on GitHub. Use the launch links above to run a build.

## Keeping this organized

Keep the documented starting build on `main`. Record changes with a short description of what changed; use named Git milestones (tags) for future checkpoints instead of adding another numbered copy. Preserve existing historical file paths, and update this guide when the launch path changes. Independent experiments can use a clearly named folder or branch.
