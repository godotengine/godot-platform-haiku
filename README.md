## Godot Engine platform port for Haiku

This is the platform port of [Godot Engine](https://godotengine.org) for the
[Haiku](https://www.haiku-os.org) operating system.

Haiku is not an officially supported platform in the main tree of Godot, so
this port is kept separate so that it can be contributed to independently of
Godot's main release cycle.

It may imply that this port might not be functional for the latest versions of
Godot. For the time being, neither the `3.2` branch nor the `master` branch are
functional out-of-the-box on Haiku.

We welcome all contributions from Haiku developers to ensure that each branch
and Git tag of this repository work as expected with the matching branches and
tags of the [Godot repository](https://github.com/godotengine/godot/).

## Usage

This code is meant to be copied as `platform/haiku` in the Godot Engine
[source repository](https://github.com/godotengine/godot/) to make builds of
Godot for Haiku.

It can also be cloned as a Git submodule:

```
git clone https://github.com/godotengine/godot
cd godot
git submodule add https://github.com/godotengine/godot-haiku-platform platform/haiku
```

Be sure to use compatible branches for the Godot repository and the Haiku port.

You can then compile Godot for Haiku with:

```
# Editor build, optimized.
scons p=haiku tools=yes target=release_debug

# Export template, debug.
scons p=haiku tools=no target=release_debug
# Export template, release.
scons p=haiku tools=no target=release
```

## License

This port is distributed under the MIT license, with the same copyright as the
main Godot source repository.

See [LICENSE.txt](/LICENSE.txt) for details, and
[AUTHORS.md](https://github.com/godotengine/godot/blob/master/AUTHORS.md) in
the Godot repository for a list of contributors.
