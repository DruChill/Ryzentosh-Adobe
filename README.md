# AMDFriend

### As a Node module installed globally on the system

You will need:
- Node.js: `brew install nodejs`
- Yarn (optional, used for contributions): `brew install yarn`

Install (and update) AMDFriend on your system with this command:
```
npm install -g amdfriend
```

Or, if you've installed yarn
```
yarn global add amdfriend
```

Use it with:
```
amdfriend "/path/to/your/library.dylib"
```


## Tips and tricks

Scan for patchable files in a directory:
```
amdfriend --dry-run --directories /path/to/dir /path/to/another/dir | grep "Routines found"
```

Scan for patchable files and patch them (NOT recommended, might use `sudo` in front of the command if patching directories not owned by the current user):
```
amdfriend --in-place --backup --sign --directories /path/to/dir /path/to/another/dir
```

## License

Refer to the LICENSE file.

## Credits

Tomnic, Tomnic and Tomnic again. You don't know him? He's [this guy](https://www.macos86.it/profile/69-tomnic/) [NyaomiDEV](https://github.com/NyaomiDEV/AMDFriend).
.
