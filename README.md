# Welcome to Torch on AMP!
These files allows you to run Space Engineers TorchAPI on the CubeCoders AMP Panel.<br>
https://cubecoders.com/AMP
## You can:
- Edit torch configs
- Add / remove people on whitelist
- Add / remove / configure plugins through File Manager
- Create a fully functioning torch server from start.
## Limitations
- Plugin listing is not available. You will need to manually install plugins and add them in via file manager
- Editing plugin config is not supported.
- You cannot send messages in console, you can only read them. This will be eventually fixed by having a compainion plugin.
- At the current moment, Windows 10/11 Home/Pro won't work because of how torch doesn't like being handled by the Network Service Account AMP Uses to run games. Windows Server 2019/2022 will work fine due to how user permissions are handled. Please note we are working with BishBash777 to get this fixed once and for all.
## Installation
Drag the:`space-engineers-torch.kvp`, `space-engineers-torchconfig.json`, and `space-engineers-torchmetaconfig.json` files into your `C:\AMPDatastore\Instances\{ADS NAME}\Plugins\ADSModule\GenericTemplates` directory.<br>
Then, restart your ADS server, and it should pop up when you create a new instance.<br>
This will soon be on the official AMPTemplates list once all issues are worked out, so stay tuned. 
## Current issues
- On initial install, a premade world will be downloaded from this repository. Torch makes it very annoyingly hard to get a premade world from default means. So until it is fixed on Torch, premade world files are on the repository.
- If creating a new world, you will have to manually copy over the previous world (if applicable) or upload an existing world from either your local world, server, etc. Ensure `File Manager > Saves > LastSession.sbl` is correct.

## Pictures
![Creating a Torch Instance](https://github.com/sam4413/amp-spaceengineers/assets/43707772/b56bc707-4326-45ac-8b69-e6ce45ad03e0)
![Torch Instance Running](https://github.com/sam4413/amp-spaceengineers/assets/43707772/7641041f-c82b-4870-9808-af4da809080e)
![Torch Console](https://github.com/sam4413/amp-spaceengineers/assets/43707772/1bfec400-a1ea-45e7-8d7e-7ca53857207c)
![Torch Config](https://github.com/sam4413/amp-spaceengineers/assets/43707772/a82afde5-0340-4ef8-a0a7-a33c790f9e5c)

<hr>
Please note that these limitations are here mainly due to how AMP works and me being relatively new to making configs.<br>
This project is still experimental! It may not work for some users. The application was tested using Windows Server 2022. Currently Linux on Torch is in a very *very* buggy state, so Linux support is currently not supported.<br>
Feel free to contribute to the github anytime!<br>
<hr>
If you have any questions, contact @sam44 on Discord.<br>
Even better, join my discord: https://discord.gg/nVgdVJ9Kpq<br>
Join the TorchAPI discord: https://discord.gg/trK6sYdcNE<br>

