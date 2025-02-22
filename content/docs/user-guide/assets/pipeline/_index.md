---
description:  Use the Open 3D Engine Asset Pipeline to convert your source art and other assets into game ready data. 
linktitle: Asset pipeline
title: Working with the Asset Pipeline and asset files
weight: 100
---

{{< preview-migrated >}}

The Asset Pipeline converts source art and other assets into OS-specific, game ready data. To prepare your game to ship, build all your game assets with the Asset Pipeline and package them with your game for your supported operating systems.

The Asset Processor (AP) is a service that runs in the background and monitors a configurable set of input directories for changes in files. When it detects changes, it uses configurable rules to determine its next action. The objective is to end up with game-ready versions of all assets for each OS and each game directory in a location called the asset cache. The asset cache is kept separate from your input directory and can be automatically rebuilt entirely from your source assets by the Asset Processor.

**Note**
The asset cache should not be added to your source control.

![\[Understand the Asset Pipeline and how it processes files for your game project in Open 3D Engine.\]](/images/user-guide/assets/pipeline/asset-pipeline-diagram.png)

The Asset Processor detects changes in the directories that contain input assets, with the game directory being the highest priority. Therefore, if you put assets in the game directory, those assets override assets with the same path in O3DE or other directories with lower priority.

Each output directory in the asset cache represents a full image of all files (except for executables and related files) needed to run the game. The Asset Processor curates the directory to keep it up to date, ensuring that new files are ready to use in the game and O3DE Editor as soon as possible. Game runtimes load assets only from the asset cache and never directly from your input source folders.

**Topics**
+ [Using Asset Processor](/docs/user-guide/assets/pipeline/processor)
+ [Configuring the Asset Pipeline](/docs/user-guide/assets/pipeline/configuring)
+ [Move assets](./move-assets)
+ [Compiling Shaders for Release Builds](/docs/userguide/assets/pipeline/shader-compilation.md)
+ [Shader Compiler Proxy](/docs/userguide/assets/pipeline/shader-compiler.md)
+ [Shader Cache and Generation](/docs/userguide/materials/shaders/custom-dev-cache-intro.md)
+ [Asset Browser](/docs/user-guide/editor/asset-browser.md)
+ [Programming the O3DE AZCore Runtime Asset System](/docs/user-guide/assets/pipeline/asset-system-programming.md)
