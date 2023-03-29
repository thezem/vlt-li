## `vlt`

`vlt` is a Node.js CLI package that allows you to save and execute commands globally from anywhere on your system. With `vlt`, you can save frequently used commands under unique names, making them easy to remember and execute with just a few keystrokes.

## Installation

To use `vlt`, you'll need to have Node.js installed on your system. Once you have Node.js installed, you can use npm to install `vlt` globally:

```
npm install -g vlt
```

## Usage

To save a command, use the `set` command with the `-i` option for the input command name and the `-o` option for the output command to be executed when the input command is called:

```
vlt set -i "adbrev" -o "adb reverse tcp:8081 tcp:8081"
```

To execute a saved command, simply use the command name as the first argument to the script followed by any additional arguments: `vlt [command] [args...]`

```
> vlt adbrev

# output
adb reverse tcp:8081 tcp:8081
```

Use the `config` command to view a list of all saved commands:

```
> vlt config

Saved commands:
{ adbrev: 'adb reverse tcp:8081 tcp:8081' }
```

## License

`vlt` is released under the [MIT License](https://opensource.org/licenses/MIT).

```

```