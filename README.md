# Interlinked

## A Sophisticated Roblox Branch Monitor

Interlinked is an advanced tool for monitoring branch instructions and control flow in Roblox, with a particular focus on understanding the behavior of anti-cheat systems.

## Inspiration

I was inspired to create this project after realizing that all anti-cheats, regardless of their complexity, ultimately come down to simple conditional checks. Even the most sophisticated kernel-level and virtualized anti-cheat systems eventually must make binary decisions based on observed conditions:

- Is memory being modified?
- Has a specific pattern been detected?
- Is a blacklisted program running?
- Has control flow deviated from expected paths?

At their core, these systems rely on branches and jumps in the code - the very instructions that Interlinked is designed to monitor. By tracking these fundamental building blocks of program execution, we can gain deeper insights into how anti-cheat systems make their decisions.

## Features

- **Real-time branch monitoring** of Roblox processes
- **Advanced pattern detection** for identifying anti-cheat triggers
- **Multiple output formats** (CSV, JSON) for detailed analysis
- **Auto-update system** ensuring you always have the latest version
- **Thread tracking** to monitor all execution paths
- **Hot address identification** to find critical code regions
- **Suspicious activity detection** including:
  - Branches to non-executable memory
  - Jumps to addresses outside known modules
  - Changes in execution patterns

## Usage

```
Interlinked.exe [options]
```

### Options

- `-h, --help`: Show help message
- `-f, --focus ADDRESS`: Focus on a specific address
- `-s, --hidden`: Run with hidden console
- `--format FORMAT`: Set output format (csv/json)
- ...and many more

## Requirements

- Windows 10/11
- Administrator privileges (for process access)

## Technical Background

Interlinked works by tracking the execution of branch instructions (jumps, calls, returns) in the target process. These instructions are fundamental to program flow control and are essential for implementing conditional logic in all software, including anti-cheat systems.

When a condition is checked in an anti-cheat, it ultimately results in a branch instruction deciding which path to follow. By monitoring these branches, we can observe the decision-making process in real-time.

## Disclaimer

This tool is created for educational and research purposes only. Understanding how anti-cheat systems function helps improve security practices and fosters knowledge about software protection mechanisms.

## License

Copyright © 2025 
