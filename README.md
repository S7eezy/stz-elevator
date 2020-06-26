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

## Adding points
By default, there are 9 teleport points, from line 2 to 10 in cl_teleports. 

You can edit coords, and add teleport points assuming you follow these 5 simple steps :
- Create a new var on line 11+
- Duplicate one of the buttons in the **RageUI.CreateWhile** loop, and edit SetEntityCoords with your new var coords.
- Init the dist as 10 on line 202
- Duplicate the else statement and make it for your new var on line 233
- Check the distance between your ped and the var coords on line 259

Everything you should know is commented right above important lines.

I know it could be a lot simpler with a **config.lua** and **for** loops, but it was irrelevant for my needs, feel free to do it.

## Editing the menu header

To edit the menu header, you have to open **"/stream/Menus/shopui_title_casino.ytd"** in OpenIV then edit the main asset.
