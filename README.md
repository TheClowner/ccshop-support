# ccShop - Modern Player Shops 
### Modern Sign / Chest based player shops. GUI based. 
ccShop is a **premium** Spigot/Paper plugin that adds player shops. The shops require in-world storage (ie chest, barrel) and a sign, with GUI-menus for buying/selling and managing the shop that open from the sign.

Spigot and Paper **1.14 to 1.17** are supported. Only **Java 16** is supported.

## Links:
- [Buy on Spigot](#)
- [Buy on MCMarket](#)
- [Join the Support Discord Server](https://discord.gg/zy3MaPq)
- [Issue Tracker](https://github.com/TheClowner/ccshop-support/issues)

## Setup / Wiki Pages
- [Wiki Home](https://github.com/TheClowner/ccshop-support/wiki)
- [**Installation / Getting Started**](https://github.com/TheClowner/ccshop-support/wiki/Getting-Started)
- [Commands and Permissions](https://github.com/TheClowner/ccshop-support/wiki/Commands-Permissions)
- [Shop Limits](https://github.com/TheClowner/ccshop-support/wiki/Limits)
- [Language System](https://github.com/TheClowner/ccshop-support/wiki/Language)

## Basic Shop Setup *(Instructions for players)*
Each Player shop still needs a sign and a container (eg. Chest, Barrel, etc.).   
Customers will need to come to the physical location of the shop in order to buy/sell from it.    

Setting up a shop is as simple as placing a sign near a container.

Sign Format:   
> **Line 1:** `[shop]`   
> *optional* **Line 2:** Item Name or `auto`   
> *optional* **Line 3:** Item Price - the price for **each** item.   
> *optional* **Line 4:** `buy` or `sell` - whether this is a buy or sell shop   
> `auto` as an item name will add the items found in the shops storage.   
> The first line is required, but all other options can be set in the GUI instead.    

Right clicking on the sign will open a Shop manager GUI, which allows you to change some of the shop settings, as well as open it to allow customers to use it.

## Plugin Features:
### General:
- **Vault Economy Integration**   
ccShop uses Vault to link to your economy, so it will work with any economy plugin that supports Vault.

- **Multi-Lingual system**    
You can setup multiple languages for all command and GUI text, and allow your players to select their preferred language.     
*This feature is disabled by default, and does not apply to sign text, currency and date formats*    
All text seen by your players is editable.     
  > NOTE: only **English** translations are supplied with the plugin.

- **Multiple container support**    
Each shop can have multiple containers as it's storage.     
Default limit for containers is 4, this is configurable.   

- **Not just Chests!**   
All containers in the game are supported, from Chests, Barrels, Shulkers to furnaces!

- **Multiple item support**   
Each shop can buy and sell multiple item types. Up to a configurable limit.    
By default shops can have up to 5 items, each of which can be to buy/sell, with it's own price and other settings.    

### Customer Interaction
- **Buy in your desired quantity.**    
In the customer GUI you can pick how much of an item you wish to buy or sell, No spamming a sign when you need a lot of an item!

- **See how much you can afford**   
Quantities you can't afford will show as barriers (by default) in the GUI. No need to click to check if you have enough. The same is also true when a shop is short on stock. 

### Shop Management
- **Stock Checking**    
View how much stock your shop has remotely.    
`/ccshop stockcheck` will show you the last known stock for all items in all your shops!

- **Stats and Logs**    
Each shop records some stats about how much you've bought/sold of each item, as well as a number of transactions so you can see who your customers have been!

- **Change settings without remaking your shop**    
The management GUIs allow you to change many aspects of your shop, without needing to break and replace the sign.     
Some of the options include:
  > - Changing the shop items    
  > - Changing item prices    
  > - Updating sign text
  > - Adding/Removing extra storage

- **Customisable sign text**    
Each shop's sign text can be completely customised once setup. No need for slightly cryptic shop signs!    
Each player can also setup a default format for their shops that will apply to each new shop they create. 

- **Trust other players**    
You can allow other players to access your shops storage, to add/take stock at will.

- **Built-In chest and sign protection**    
Shops storage is always locked so only the shop owner and those they trust can access it.

- **Toggleable messages**    
Messages when someone buys/sells from you, as well as your shop being out of stock can be disabled by each player in `/ccshop manage`

- **Confirmation Screens**    
We wont let you delete your shop by accident! Several more 'risky' options will show you a confirm screen before taking action. 

### Administration Features
- **Item Price Limits**    
You can set Maximum and Minimum prices for buying/selling certain items.

- **Block items from sale**    
Ban items from being bought/sold in player shops entirely. 

- **Bypass permissions**    
Admins are able to bypass protection to access shop storage, or delete shops they don't own. 

- **Configurable Limits**    
You can customise limits on a number of shop features:
  - How many containers can be linked to a shop (default 3)
  - How many signs can be linked to a shop (default 1)
  - The maximum distance a container or sign can be from the first shop sign. (default 16 blocks)
  - The number of items per shop (default 5)
  - The number of shops each player can create (default unlimited)
