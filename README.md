# README

[keyhac-win](https://github.com/crftwr/keyhac-win) (now archived) customization.

Environment:

- [CorvusSKK](https://github.com/nathancorvussolis/corvusskk)
- JIS keyboard


## Install

Run [`install.ps1`](./install.ps1) to create junction of `Keyhac` to AppData.

```
powershell .\install.ps1
```

### Optional

Running [`ScheduledTask/install.ps1`](./ScheduledTask/install.ps1) with `keyhac.exe` path copies `ScheduledTask/run.ps1` to `$env:AppData\KeyhacStarter` and registers scheduled task to run it at logon:

```
powershell .\ScheduledTask\install.ps1 "$env:USERPROFILE\Personal\tools\portable_apps\keyhac\keyhac.exe"
```

## Development Setup

This project uses [uv](https://docs.astral.sh/uv/) to match the Python version bundled with keyhac.

To set up the development environment, run:

```
uv sync
```


