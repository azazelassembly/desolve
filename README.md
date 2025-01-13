# Desolve.decomp

Desolve.decomp is a customized and improved saveinstance project inspired by Universal Syn Save Instance (USSI) and similar tools. The goal of Desolve.decomp is to provide a high-performance, flexible, and user-friendly way to save instances without modifying anything in the target game, reducing detection vectors and enhancing compatibility with various executors.

---

## Key Features

- **Safe Mode**: A detection-free mode to bypass any restrictions and save **ANY** game.
- **Custom Decompiler**: Added support for executors without native decompilers.
- **Performance Optimizations**: Utilizes Lua’s latest performance enhancements for faster operations.
- **Extensive Executor Compatibility**: Designed to work with as many executors as possible.
- **Support for Both XML and Binary Formats**: Save instances in RBXMX (XML) or RBXM (binary) formats.
- **Flexible Options**: Configurable options for decompilation, instance isolation, and more.
- **Error Handling**: Includes fixes for common errors encountered during saveinstance operations.

---

## Installation

1. Copy the script below into your executor:
   ```lua
   local Params = {
     RepoURL = "https://raw.githubusercontent.com/azazelassembly/desolve/main/",
     SSI = "saveinstance",
   }
   local desolve_decomp = loadstring(game:HttpGet(Params.RepoURL .. Params.SSI .. ".luau", true), Params.SSI)()
   local Options = {} -- Customize options here
   desolve_decomp(Options)
   ```
2. For detailed configuration options, refer to the [Documentation](https://github.com/azazelassembly/desolve).

---

## Usage Tips

- **Binary Format**: Use the `Binary` option to save instances in RBXM format for reduced file sizes.
- **Error Recovery**: Restart saveinstance from the point of a crash using skip options.
- **Safe Mode**: Enable `SafeMode` for the safest saving experience.
- **Performance Tuning**: Benchmark the script in your executor to find optimal settings.

---

## To-Do List

### Planned Features

- Add support for advanced binary format output (RBXL/RBXM).
- Improve compatibility with custom properties and hidden values.
- Add support for special property serialization (e.g., BinaryStrings).
- Extend the API to include advanced type-checking and mode-specific optimizations.

### Completed Features

- Support for XML format (RBXMX).
- Custom decompiler for unsupported executors.
- Error handling and fallbacks for missing executor functionality.
- Optimized property serialization for speed and accuracy.
- Documentation for all options and use cases.

---

## Contribution Guidelines

Contributions are welcome! If you’d like to contribute:

1. Fork the [GitHub Repository](https://github.com/azazelassembly/desolve).
2. Submit a pull request with detailed descriptions of your changes.
3. Ensure that all changes adhere to the [License Agreement](https://github.com/azazelassembly/desolve/blob/main/LICENSE).

---

## License

This project is licensed under the [MIT License](https://github.com/azazelassembly/desolve/blob/main/LICENSE). **You must always include the following credit string:**

```
Desolve.decomp https://discord.gg/wx4ThpAsmw
```

Failure to include proper attribution violates the terms of use.

---

## Acknowledgments

This project is based on efforts from multiple contributors and tools:

- **Universal Syn Save Instance**: Base inspiration for the project.
- **[@Anaminus](https://github.com/Anaminus)** and **[@Dekkonot](https://github.com/Dekkonot)**: For their work on Roblox Format Specifications.
- **Synapse X Source 2019**: Extended by **[@mblouka](https://github.com/mblouka)** and **[@Acrillis](https://github.com/Acrillis)**.
- **Moon/LorekeeperZinnia**: Original creator of saveinstance functionality.

---

## Join the Community

Have questions, need help, or want to contribute? Join our Discord server:



---

## Support Us

If you find Desolve.decomp helpful, consider supporting us to keep the development alive:



discord.gg/invite
