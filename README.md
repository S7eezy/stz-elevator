# stz-elevator
*Welcome, this is my first ever release*. 

This script will allow you to simply setup a RageUI Elevator or Teleport script.

# Why is this thing even existing
By default, it is setup to work for VespucciPD MLO, but you can easily edit coords to fit your needs.

It was made to reach a very low resource consumption.
- Whenever your ped stands at a distance of over 50 meters from the Lobby elevator, the main loop will idle long enough to save resources.
- Whenever distance reaches 100, 200 or 500 meters between you and the elevator, the resource will adjust its wait time on the main loop even longer.

I thought it would be interesting to share this even if you absolutely don't need this specific elevator, because of the way it works with distances.

# Demo
https://streamable.com/fncf45

# Credits
**RageUI by iTexZoz:**
https://github.com/iTexZoz/RageUI
**RageUI Wiki:**
https://github.com/iTexZoz/RageUI/wiki

# Editing this resource
Feel free to edit this resource to fit your needs.

- By default, there are 9 teleport points, from line 2 to 10 in cl_teleports. You can edit coords, and add teleport points assuming you duplicate one of the buttons in the **RageUI.CreateWhile** loop.
Everything you should know is commented right above important lines.

- To edit the menu header, you have to open **"/stream/Menus/shopui_title_casino.ytd"** in OpenIV then edit the main asset.
