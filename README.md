# bazel-cmakelists

The workaround script to generate a `CMakeLists.txt` from [Bazel](https://bazel.io) C++ target.

## Usage

```
bazel-cmakelists --targets <bazel-target>
```

e.g.

```
bazel-cmakelists --targets //test/...
```

- Do not use generated `CMakeLists.txt` to build, use bazel.
- Only tested with CLion, might work for other IDEs that understand `CMakeLists.txt`
- After a change to `BUILD` or `WORKSPACE` files, re-run the script to get `CMakeLists.txt` updated.

## Requirements
- Python 2.7
- Bazel 0.17+
