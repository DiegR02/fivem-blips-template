# fivem-blips-template

A reusable [FiveM](https://fivem.net/) Lua template for adding custom map blips to your game server resource. Clone or fork this starter to skip the boilerplate and focus on your own blip configuration.

---

## Features

- Pre-wired FiveM resource structure (`fxmanifest.lua` / `__resource.lua`)
- Client-side Lua script with a clean blip registration pattern
- Minimal dependencies — pure Lua, no external libraries required
- Easy to extend: add sprites, colours, scales and labels in one place

---

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Lua |
| Platform | FiveM (CitizenFX) |
| Project type | Game-server resource / Template |

---

## Getting Started

### Prerequisites

- A running [FiveM server](https://docs.fivem.net/docs/server-manual/setting-up-a-server/)
- Basic knowledge of Lua and FiveM resource structure

### Installation

1. Clone or download this repository into your server's `resources` folder:

   ```bash
   git clone https://github.com/DiegR02/fivem-blips-template.git resources/blips-template
   ```

2. Add the resource to your `server.cfg`:

   ```
   ensure blips-template
   ```

3. Restart your server or run `refresh` followed by `ensure blips-template` in the server console.

---

## Usage

Open the client-side Lua file and edit the blip definitions to match your needs:

```lua
-- Example blip entry
local blip = AddBlipForCoord(441.0, -983.0, 30.0)
SetBlipSprite(blip, 1)        -- sprite ID
SetBlipDisplay(blip, 4)       -- display type
SetBlipScale(blip, 0.8)       -- size
SetBlipColour(blip, 2)        -- colour index
SetBlipAsShortRange(blip, true)
BeginTextCommandSetBlipName("STRING")
AddTextComponentString("My Location")
EndTextCommandSetBlipName(blip)
```

Refer to the [FiveM Blip documentation](https://docs.fivem.net/docs/game-references/blips/) for all available sprite and colour IDs.

---

## Project Status

This is a **learning / practice project** intended as a reusable starter template. It is not production software. Contributions, suggestions and forks are welcome.

---

## Topics

`blips` `fivem` `game-server-resource` `learning-project` `lua` `template`

---

## License

See [LICENSE](LICENSE) for details.
