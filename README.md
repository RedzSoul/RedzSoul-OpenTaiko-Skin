# RedzSoul-OpenTaiko-Skin

Fork of [Moshir's OpenTaiko Skin](https://github.com/MoshirMoshir/Moshir-OpenTaiko-Skin), updated to support **OpenTaiko 0.6.0.107** and customized by RedzSoul.

See [CREDITS.md](CREDITS.md) for full credits.

## Requirements

- **OpenTaiko version 0.6.0.107** exactly. Other versions (earlier or later) may not be compatible: this skin includes fixes specific to bugs introduced in this version (`Modules/` system, texture parsing). To check your version, look at the game window title or the `OpenTaiko.log` file.

## How to install

1. Download the latest release from [Releases](https://github.com/RedzSoul/RedzSoul-OpenTaiko-Skin/releases) (`.zip` file), or click the green `Code` button → `Download ZIP` on this page.
2. Extract the zip. If you downloaded from the `Code` button, you'll get a folder like `RedzSoul-OpenTaiko-Skin-main`: open that folder, step 3 refers to its **contents**, not the folder itself.
3. Copy the following two things into your OpenTaiko installation folder:
   - the `System/RedzSoul-OpenTaiko-Skin/` folder → into OpenTaiko's `System/` folder (final result: `OpenTaiko/System/RedzSoul-OpenTaiko-Skin/`)
   - the contents of the `Global/` folder → into OpenTaiko's `Global/` folder, **merging** the files (do not overwrite/delete what's already there: this skin adds extra characters and Puchichara, it doesn't replace them)
4. Launch OpenTaiko, go to settings and select **RedzSoul-OpenTaiko-Skin** as the active skin.
5. **Fully restart the game** (close and reopen it): OpenTaiko requires a restart to correctly apply the new skin.
6. Enjoy!

### Where is the OpenTaiko folder?

It depends on how you installed the game. Common paths on Windows:
- `%LocalAppData%\OpenTaiko Hub\OpenTaiko\` (installed via OpenTaiko Hub)
- the folder where you manually extracted/installed OpenTaiko

If you're not sure, look for the folder that contains `OpenTaiko.exe` and a `System/` subfolder: that's the right one.

## Troubleshooting

| Problem | Likely cause | Fix |
|---|---|---|
| The skin doesn't show up in the game's skin list | You copied the entire repository folder instead of just `System/RedzSoul-OpenTaiko-Skin/` | Check that the final path is `OpenTaiko/System/RedzSoul-OpenTaiko-Skin/SkinConfig.ini` (not nested deeper) |
| `CLuaModalScript`/`CLuaNamePlateScript` errors at boot | You're using an OpenTaiko version other than 0.6.0.107 | Check/update your game version |
| Missing extra characters or Puchichara | You didn't copy the contents of `Global/` | Repeat step 3, Global section |
| Skin changes don't show up after an update | The game wasn't restarted | Fully close OpenTaiko and reopen it |

For any other issue, open an [issue](https://github.com/RedzSoul/RedzSoul-OpenTaiko-Skin/issues) with the exact error message (visible in `OpenTaiko.log`, in the game's installation folder).

## FAQ

1. What are the `.kra` files?
> Krita working files used to create the corresponding `.png` assets. Not needed for the skin to work, included for anyone who wants to edit the assets.

## More Information

To report bugs or suggestions, open an issue on this repository.
<br><br>
If Namco or asset owners have an issue with me distributing this skin or their assets, please contact me and I will immediately make this repository private.
