# JR_Rebreather

A simple FiveM ESX resource that adds a rebreather item.
 This script allows players to breathe underwater longer, displays an oxygen UI with animated bubbles, and automatically removes the rebreather when oxygen runs out.

---

## Features

* Equip a rebreather mask using **Illenium Appearance** or **Skinchanger**.
* Track underwater oxygen with a **TextUI** indicator.
* Animated **bubble HUD** while underwater.
* Oxygen tracking works only underwater.
* TextUI automatically hides when the mask is removed or oxygen runs out.
* Bubble HUD is purely cosmetic and client-side.
* Auto-removes rebreather from inventory when oxygen is depleted.
* Notifications for equipping, removing, and empty oxygen via **ox\_lib**.
* Compatible with the latest **ESX (es\_extended)**.

---

## Requirements

* [ESX Framework](https://esx-framework.org/)
* [ox\_lib](https://overextended.github.io/ox_lib/)
* **illenium-appearance** or **skinchanger** for clothing support

---

## Installation

1. Add this item to your inventory
	["rebreather"] = {
		label = "Rebreather",
		weight = 1000,
		stack = false,
	},
2. Add the item image located in the `install` folder.
3. Place this resource in your `resources` folder.
4. Configure the `config.lua` to your preference.
5. Add it to your `server.cfg`: make sure it's started after Requirements

```cfg
ensure JR_Rebreather
```

## Usage

* Use the rebreather item (`rebreather`) from your inventory.
* While underwater, a **TextUI** shows remaining oxygen with animated bubbles.
* When oxygen reaches **0**, the rebreather is removed from the player and the inventory, with a notification.
* Players can manually remove the rebreather; UI and bubbles hide automatically.
