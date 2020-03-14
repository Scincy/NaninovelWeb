﻿# Adventure Creator

[Adventure Creator](https://www.adventurecreator.org/) lets you make traditional 2D, 2.5D and 3D adventure games - those that emphasize storytelling, exploration and puzzles - such as Monkey Island, Grim Fandango, The Longest Journey, and Telltale's The Walking Dead. 

![](https://i.gyazo.com/74a12fa535198cb26a87a5037b15a988.jpg)

You can use Naninovel to handle dialogue scenes in AC or load AC from a Naninovel-based game for some custom gameplay.

## Setup

Install both Adventure Creator and Naninovel (the order doesn't matter).

Download and import [Adventure Creator extension package](https://github.com/Elringus/NaninovelAdventureCreator/raw/master/NaninovelAdventureCreator.unitypackage).

Set `NaninovelAdventureCreator/Runtime/Actions` as the source for custom actions in AC settings. Consult [AC guide](https://www.adventurecreator.org/tutorials/writing-custom-action) for more info on custom actions.

![](https://i.gyazo.com/59a162751411ec60a7cf5ad89e9a66ec.png)

You should now see "Play Naninovel Script" action available under "Custom" category.

![](https://i.gyazo.com/faf33afa1df8ff98ea04ef9cf1a44f8f.png)

Depending on the setup, you may need to assign a special layer for Naninovel objects to prevent them from being rendered by AC cameras and vice-versa. This can be done via Naninovel's Engine configuration window. 

![](https://i.gyazo.com/ed765928c0420ec2b1e26d6bf4a66e6c.png)

When using Naninovel as a drop-in system from AC-based game, you may also want to disable `Initialize On Application Load` and `Show Title UI` options in the Engine configuration.

## Usage

Use `Play Naninovel Script` custom AC action to (optionally) turn-off AC, initialize Naninovel engine (when required) and load specified Naninovel script. By default, the AC and Naninovel cameras will also swap automatically, but you can prevent that by disabling `Swap Cameras` property.

Use `@turnOnAC` custom Naninovel command in a Naninovel script to enable AC, reset Naninovel engine state (optionally) and swap the cameras back (also optionally). State reset is controlled with `reset` and camera swap with `swapCameras` parameters.

The following video demonstrates AC's demo scene integrated with Naninovel to handle a dialogue.

<div class="video-container">
    <iframe src="https://www.youtube-nocookie.com/embed/7tOIFZRSAec" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

## Example Project

See the [GitHub project](https://github.com/Elringus/NaninovelAdventureCreator) for an integration example. When opening the project for the first time you'll get errors due to missing Adventure Creator and Naninovel packages. Just import them from Asset Store and the errors will go away.