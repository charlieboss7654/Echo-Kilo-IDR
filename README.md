# Echo Kilo – Incident Data Recorder (IDR)

A clean, immersive, and fully integrated IDR for FiveM.

## Features
- Logs key events:
  - Damage (engine/body drop or collision)
  - New Driver Detected / Driver Left Vehicle
  - ELS ON / ELS OFF

- Modern and realistic UI
  - Green theme, sticky header
  - Press ESC to close
  - Realistic UI that looks almost exactly the same as an IDR in real life!

- Easy access
  - Third-eye a configured vehicle with ox_target ? 'View IDR'

- Persistence & maintenance
  - Saves per-plate logs to `data/idr.json`
  - Daily reset (configurable time) wipes all logs and clears the file
  - Manual reset command available

## Installation

1. Drag and drop the folder into your `resources/` directory.

2. Add the following to your `server.cfg`:

ensure ox_lib
ensure ox_target
ensure EKS_IDR

3. Ensure these requirements are running:
- ox_lib – https://overextended.github.io/ox_lib/
- ox_target – https://github.com/overextended/ox_target

## Daily / Manual Reset

- The server schedules a reset once per day at the time in `shared/config.lua`. 
 
This clears all in-memory logs and writes `{}` to `data/idr.json`.

- Manual reset (console/ACE):
/idrreset


Grant via ACE (example):
add_ace group.admin command.idrreset allow


## Support

Need help or custom features? Open a ticket through Echo Kilo Studios:

https://discord.gg/busQ9w6dqa
