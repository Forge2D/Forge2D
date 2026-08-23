# Forge2D Project Format

Forge2D projects use a `project.forge` configuration file.

A basic project can look like this:

```text
forge_project MyGame
standard c++17
output MyGame

sources
    src/main.cpp
end
```

## `forge_project`

Defines the project name.

Example:

```text
forge_project MyGame
```

## `standard`

Defines the C++ language standard used to compile the project.

Supported standards include:

```text
c++17
c++20
c++23
```

Example:

```text
standard c++17
```

## `output`

Defines the name of the generated game executable.

Example:

```text
output MyGame
```

## `sources`

Lists the source files belonging to the project.

Example:

```text
sources
    src/main.cpp
    src/player.cpp
    src/game.cpp
end
```

Source files should remain inside the project directory.

## Example project

```text
MyGame/
├── project.forge
└── src/
    ├── main.cpp
    ├── player.cpp
    └── game.cpp
```
