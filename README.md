# wmic

wmic( Windows Management Instrumentation Command-line ) wrapper for Node.js

## How to use

```typescript
import wmic from "wmic-node";

const demo = async () =>
{
    console.log(`wmic("cpu"): ${JSON.stringify(await wmic("cpu"), null, 4)}`);
};

demo();
```

## Reference

### function

```typescript
function wmic(command: command): Promise<{ [key: string]: string }[]>;
```

### commands

- `"alias"`
- `"baseboard"`
- `"bios"`
- `"bootconfig"`
- `"cdrom"`
- `"computersystem"`
- `"cpu"`
- `"csproduct"`
- `"datafile"`
- `"dcomapp"`
- `"desktop"`
- `"desktopmonitor"`
- `"devicememoryaddress"`
- `"diskdrive"`
- `"diskquota"`
- `"dmachannel"`
- `"environment"`
- `"fsdir"`
- `"group"`
- `"idecontroller"`
- `"irq"`
- `"job"`
- `"loadorder"`
- `"logicaldisk"`
- `"logon"`
- `"memcache"`
- `"memorychip"`
- `"memphysical"`
- `"netclient"`
- `"netlogin"`
- `"netprotocol"`
- `"netuse"`
- `"nic"`
- `"nicconfig"`
- `"ntdomain"`
- `"ntevent"`
- `"nteventlog"`
- `"onboarddevice"`
- `"os"`
- `"pagefile"`
- `"pagefileset"`
- `"partition"`
- `"port"`
- `"portconnector"`
- `"printer"`
- `"printerconfig"`
- `"printjob"`
- `"process"`
- `"product"`
- `"qfe"`
- `"quotasetting"`
- `"rdaccount"`
- `"rdnic"`
- `"rdpermissions"`
- `"rdtoggle"`
- `"recoveros"`
- `"registry"`
- `"scsicontroller"`
- `"server"`
- `"service"`
- `"shadowcopy"`
- `"shadowstorage"`
- `"share"`
- `"softwareelement"`
- `"softwarefeature"`
- `"sounddev"`
- `"startup"`
- `"sysaccount"`
- `"sysdriver"`
- `"systemenclosure"`
- `"systemslot"`
- `"tapedrive"`
- `"temperature"`
- `"timezone"`
- `"ups"`
- `"useraccount"`
- `"voltage"`
- `"volume"`
- `"volumequotasetting"`
- `"volumeuserquota"`
- `"wmiset"`

## How to build

requires: [Node.js](https://nodejs.org/), [TypeScript Compiler](https://www.npmjs.com/package/typescript)

`tsc -P .` or `tsc -P . -w`

### In VS Code

You can use automatic build. Run `Tasks: Allow Automatic Tasks in Folder` command from command palette ( Mac: <kbd>F1</kbd> or <kbd>Shift</kbd>+<kbd>Command</kbd>+<kbd>P</kbd>, Windows and Linux: <kbd>F1</kbd> or <kbd>Shift</kbd>+<kbd>Ctrl</kbd>+<kbd>P</kbd>), and restart VS Code.

## License

[Boost Software License](./LICENSE_1_0.txt)
