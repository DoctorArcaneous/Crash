---- Minecraft Crash Report ----
// You're mean.

Time: 5/28/22 2:07 PM
Description: Unexpected error

java.lang.IllegalStateException: Lock is no longer valid
	at net.minecraft.world.storage.SaveFormat$LevelSave.func_237301_i_(SaveFormat.java:296) ~[?:?] {re:computing_frames,re:classloading}
	at net.minecraft.world.storage.SaveFormat$LevelSave.func_237298_f_(SaveFormat.java:360) ~[?:?] {re:computing_frames,re:classloading}
	at net.minecraft.server.MinecraftServer.func_184109_z(MinecraftServer.java:770) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:betterendforge.mixins.json:MinecraftServerMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftServerMixin,pl:mixin:A}
	at net.minecraft.server.MinecraftServer.func_184106_y(MinecraftServer.java:764) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:betterendforge.mixins.json:MinecraftServerMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftServerMixin,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.func_195458_a(GameRenderer.java:428) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_195542_b(Minecraft.java:977) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:randompatches.mixins.json:client.MinecraftMixin,pl:mixin:APP:betterendforge.mixins.json:MinecraftMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftMixin,pl:mixin:APP:immersiveengineering.mixins.json:accessors.client.MinecraftAccess,pl:mixin:APP:flywheel.mixins.json:ShaderCloseMixin,pl:mixin:APP:globaldataandresourcepacks.mixins.json:ClientPackFinderMixin,pl:mixin:APP:assets/botania/botania.mixins.json:AccessorMinecraft,pl:mixin:APP:performant.mixins.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:WindowResizeMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:607) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:randompatches.mixins.json:client.MinecraftMixin,pl:mixin:APP:betterendforge.mixins.json:MinecraftMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftMixin,pl:mixin:APP:immersiveengineering.mixins.json:accessors.client.MinecraftAccess,pl:mixin:APP:flywheel.mixins.json:ShaderCloseMixin,pl:mixin:APP:globaldataandresourcepacks.mixins.json:ClientPackFinderMixin,pl:mixin:APP:assets/botania/botania.mixins.json:AccessorMinecraft,pl:mixin:APP:performant.mixins.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:WindowResizeMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:184) [?:?] {re:classloading,pl:runtimedistcleaner:A}
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_51] {}
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_51] {}
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_51] {}
	at java.lang.reflect.Method.invoke(Method.java:497) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider.lambda$launchService$0(FMLClientLaunchProvider.java:51) [forge-1.16.5-36.2.23.jar:36.2] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider$$Lambda$495/1860734497.call(Unknown Source) [forge-1.16.5-36.2.23.jar:36.2] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:37) [modlauncher-8.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:54) [modlauncher-8.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:72) [modlauncher-8.0.9.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:82) [modlauncher-8.0.9.jar:?] {re:classloading}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:66) [modlauncher-8.0.9.jar:?] {re:classloading}


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Render thread
Stacktrace:
	at net.minecraft.world.storage.SaveFormat$LevelSave.func_237301_i_(SaveFormat.java:296) ~[?:?] {re:computing_frames,re:classloading}
	at net.minecraft.world.storage.SaveFormat$LevelSave.func_237298_f_(SaveFormat.java:360) ~[?:?] {re:computing_frames,re:classloading}
	at net.minecraft.server.MinecraftServer.func_184109_z(MinecraftServer.java:770) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:betterendforge.mixins.json:MinecraftServerMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftServerMixin,pl:mixin:A}
	at net.minecraft.server.MinecraftServer.func_184106_y(MinecraftServer.java:764) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:betterendforge.mixins.json:MinecraftServerMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftServerMixin,pl:mixin:A}
-- Affected level --
Details:
	All players: 1 total; [ClientPlayerEntity['NixonRixon'/439, l='ClientLevel', x=8.50, y=65.00, z=8.50]]
	Chunk stats: Client Chunk Cache: 841, 0
	Level dimension: minecraft:overworld
	Level spawn location: World: (8,64,8), Chunk: (at 8,4,8 in 0,0; contains blocks 0,0,0 to 15,255,15), Region: (0,0; contains chunks 0,0 to 31,31, blocks 0,0,0 to 511,255,511)
	Level time: 0 game time, 0 day time
	Server brand: forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.world.ClientWorld.func_72914_a(ClientWorld.java:447) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:architectury.mixins.json:MixinClientLevel,pl:mixin:APP:create.mixins.json:BreakProgressMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2031) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:randompatches.mixins.json:client.MinecraftMixin,pl:mixin:APP:betterendforge.mixins.json:MinecraftMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftMixin,pl:mixin:APP:immersiveengineering.mixins.json:accessors.client.MinecraftAccess,pl:mixin:APP:flywheel.mixins.json:ShaderCloseMixin,pl:mixin:APP:globaldataandresourcepacks.mixins.json:ClientPackFinderMixin,pl:mixin:APP:assets/botania/botania.mixins.json:AccessorMinecraft,pl:mixin:APP:performant.mixins.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:WindowResizeMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:628) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:randompatches.mixins.json:client.MinecraftMixin,pl:mixin:APP:betterendforge.mixins.json:MinecraftMixin,pl:mixin:APP:kubejs-common.mixins.json:MinecraftMixin,pl:mixin:APP:immersiveengineering.mixins.json:accessors.client.MinecraftAccess,pl:mixin:APP:flywheel.mixins.json:ShaderCloseMixin,pl:mixin:APP:globaldataandresourcepacks.mixins.json:ClientPackFinderMixin,pl:mixin:APP:assets/botania/botania.mixins.json:AccessorMinecraft,pl:mixin:APP:performant.mixins.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:WindowResizeMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:184) [?:?] {re:classloading,pl:runtimedistcleaner:A}
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_51] {}
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_51] {}
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_51] {}
	at java.lang.reflect.Method.invoke(Method.java:497) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider.lambda$launchService$0(FMLClientLaunchProvider.java:51) [forge-1.16.5-36.2.23.jar:36.2] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider$$Lambda$495/1860734497.call(Unknown Source) [forge-1.16.5-36.2.23.jar:36.2] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:37) [modlauncher-8.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:54) [modlauncher-8.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:72) [modlauncher-8.0.9.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:82) [modlauncher-8.0.9.jar:?] {re:classloading}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:66) [modlauncher-8.0.9.jar:?] {re:classloading}


-- System Details --
Details:
	Minecraft Version: 1.16.5
	Minecraft Version ID: 1.16.5
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 2560465744 bytes (2441 MB) / 5349834752 bytes (5102 MB) up to 11453595648 bytes (10923 MB)
	CPUs: 12
	JVM Flags: 4 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx12288m -Xms256m
	ModLauncher: 8.0.9+86+master.3cf110c
	ModLauncher launch target: fmlclient
	ModLauncher naming: srg
	ModLauncher services: 
		/mixin-0.8.4.jar mixin PLUGINSERVICE 
		/eventbus-4.0.0.jar eventbus PLUGINSERVICE 
		/forge-1.16.5-36.2.23.jar object_holder_definalize PLUGINSERVICE 
		/forge-1.16.5-36.2.23.jar runtime_enum_extender PLUGINSERVICE 
		/accesstransformers-3.0.1.jar accesstransformer PLUGINSERVICE 
		/forge-1.16.5-36.2.23.jar capability_inject_definalize PLUGINSERVICE 
		/forge-1.16.5-36.2.23.jar runtimedistcleaner PLUGINSERVICE 
		/mixin-0.8.4.jar mixin TRANSFORMATIONSERVICE 
		/forge-1.16.5-36.2.23.jar fml TRANSFORMATIONSERVICE 
	FML: 36.2
	Forge: net.minecraftforge:36.2.23
	FML Language Providers: 
		javafml@36.2
		minecraft@1
		kotlinforforge@1.16.0
		scorge@3.1.3
	Mod List: 
		rsrequestify-1.16.5-2.1.6.jar                     |RSRequestify                  |rsrequestify                  |2.1.6               |DONE      |Manifest: NOSIGNATURE
		supermartijn642configlib-1.0.9-mc1.16.jar         |SuperMartijn642's Config Lib  |supermartijn642configlib      |1.0.9               |DONE      |Manifest: NOSIGNATURE
		simplemagnets-1.1.4-mc1.16.jar                    |Simple Magnets                |simplemagnets                 |1.1.4               |DONE      |Manifest: NOSIGNATURE
		ExtendedCrafting-1.16.5-3.1.11.jar                |Extended Crafting             |extendedcrafting              |3.1.11              |DONE      |Manifest: NOSIGNATURE
		mcw-windows-2.0.2-mc1.16.5.jar                    |Macaw's Windows               |mcwwindows                    |2.0.2               |DONE      |Manifest: NOSIGNATURE
		modnametooltip_1.16.2-1.15.0.jar                  |Mod Name Tooltip              |modnametooltip                |1.15.0              |DONE      |Manifest: NOSIGNATURE
		KleeSlabs_1.16.5-9.2.1.jar                        |KleeSlabs                     |kleeslabs                     |9.2.1               |DONE      |Manifest: NOSIGNATURE
		rsgauges-1.16.5-1.2.13.jar                        |Gauges and Switches           |rsgauges                      |1.2.13              |DONE      |Manifest: bf:30:76:97:e4:58:41:61:2a:f4:30:d3:8f:4c:e3:71:1d:14:c4:a1:4e:85:36:e3:1d:aa:2f:cb:22:b0:04:9b
		Neat 1.7-27.jar                                   |Neat                          |neat                          |1.7-27              |DONE      |Manifest: NOSIGNATURE
		IronJetpacks-1.16.5-4.2.3.jar                     |Iron Jetpacks                 |ironjetpacks                  |4.2.3               |DONE      |Manifest: NOSIGNATURE
		CTM-MC1.16.1-1.1.2.6.jar                          |ConnectedTexturesMod          |ctm                           |MC1.16.1-1.1.2.6    |DONE      |Manifest: NOSIGNATURE
		CookingForBlockheads_1.16.5-9.3.4.jar             |Cooking for Blockheads        |cookingforblockheads          |9.3.4               |DONE      |Manifest: NOSIGNATURE
		Controlling-7.0.0.28.jar                          |Controlling                   |controlling                   |7.0.0.28            |DONE      |Manifest: NOSIGNATURE
		Placebo-1.16.5-4.6.1.jar                          |Placebo                       |placebo                       |4.6.1               |DONE      |Manifest: NOSIGNATURE
		dankstorage-3.19.jar                              |Dank Storage                  |dankstorage                   |3.19                |DONE      |Manifest: NOSIGNATURE
		Bookshelf-Forge-1.16.5-10.4.31.jar                |Bookshelf                     |bookshelf                     |10.4.31             |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		reliquary-1.16.5-1.3.5.1104.jar                   |Reliquary                     |xreliquary                    |1.16.5-1.3.5.1104   |DONE      |Manifest: NOSIGNATURE
		sophisticatedbackpacks-1.16.5-3.15.1.503.jar      |Sophisticated Backpacks       |sophisticatedbackpacks        |1.16.5-3.15.1.503   |DONE      |Manifest: NOSIGNATURE
		randompatches-2.4.4-forge.jar                     |RandomPatches                 |randompatches                 |2.4.4-forge         |DONE      |Manifest: 92:f6:29:d4:09:89:f5:f5:98:5e:20:34:31:d0:7b:58:22:06:bd:a5:d1:6a:92:6e:ac:3d:8d:18:c5:b2:5b:d7
		ExCompressum_1.16.5-4.0.5.jar                     |Ex Compressum                 |excompressum                  |4.0.5               |DONE      |Manifest: NOSIGNATURE
		buildinggadgets-1.16.5-3.8.2.jar                  |Building Gadgets              |buildinggadgets               |3.8.2               |DONE      |Manifest: NOSIGNATURE
		DarkUtilities-1.16.5-8.0.10.jar                   |Dark Utilities                |darkutils                     |8.0.10              |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		Apotheosis-1.16.5-4.8.4.jar                       |Apotheosis                    |apotheosis                    |4.8.4               |DONE      |Manifest: NOSIGNATURE
		mcw-doors-1.0.5-mc1.16.5.jar                      |Macaw's Doors                 |mcwdoors                      |1.0.5               |DONE      |Manifest: NOSIGNATURE
		Morpheus-1.16.5-4.2.70.jar                        |Morpheus                      |morpheus                      |4.2.70              |DONE      |Manifest: NOSIGNATURE
		TwerkItMeal-1.3.9.jar                             |TwerkItMeal                   |twerkitmeal                   |1.3.9               |DONE      |Manifest: NOSIGNATURE
		carryon-1.16.5-1.15.5.22.jar                      |Carry On                      |carryon                       |1.15.5.22           |DONE      |Manifest: NOSIGNATURE
		JustEnoughResources-1.16.5-0.12.1.133.jar         |Just Enough Resources         |jeresources                   |0.12.1.133          |DONE      |Manifest: NOSIGNATURE
		shetiphiancore-1.16-3.8.9.jar                     |ShetiPhian-Core               |shetiphiancore                |3.8.9               |DONE      |Manifest: NOSIGNATURE
		LostTrinkets-1.16.5-0.1.27.jar                    |Lost Trinkets                 |losttrinkets                  |0.1.27              |DONE      |Manifest: NOSIGNATURE
		absentbydesign-1.16.5-1.5.1.jar                   |Absent By Design Mod          |absentbydesign                |1.16.5-1.5.1        |DONE      |Manifest: 1f:47:ac:b1:61:82:96:b8:47:19:16:d2:61:81:11:60:3a:06:4b:61:31:56:7d:44:31:1e:0c:6f:22:5b:4c:ed
		twilightforest-1.16.5-4.0.870-universal.jar       |The Twilight Forest           |twilightforest                |NONE                |DONE      |Manifest: NOSIGNATURE
		supplementaries-1.16.5-0.18.2.jar                 |Supplementaries               |supplementaries               |0.18.2              |DONE      |Manifest: NOSIGNATURE
		mob_grinding_utils-1.16.5-0.4.32.jar              |Mob Grinding Utils            |mob_grinding_utils            |1.16.5-0.4.32       |DONE      |Manifest: NOSIGNATURE
		emojiful-1.16.4-2.1.6.jar                         |Emojiful                      |emojiful                      |1.16.4-2.1.6        |DONE      |Manifest: NOSIGNATURE
		cobblegenrandomizer-1.16-5.1.2.jar                |CobbleGenRandomizer           |cobblegenrandomizer           |1.16-5.1.2          |DONE      |Manifest: NOSIGNATURE
		refinedstorage-1.9.16.jar                         |Refined Storage               |refinedstorage                |1.9.16              |DONE      |Manifest: NOSIGNATURE
		betterendforge-1.16.5-1.6.3.jar                   |BetterEnd Forge               |betterendforge                |1.16.5-1.6.3        |DONE      |Manifest: NOSIGNATURE
		FarmersDelight-1.16.5-0.5.4.jar                   |Farmer's Delight              |farmersdelight                |1.16.5-0.5.4        |DONE      |Manifest: NOSIGNATURE
		torchmaster-2.3.8.jar                             |Torchmaster                   |torchmaster                   |2.3.8               |DONE      |Manifest: NOSIGNATURE
		endertanks-1.16-1.9.8.jar                         |EnderTanks                    |endertanks                    |1.9.8               |DONE      |Manifest: NOSIGNATURE
		valkyrielib-1.16.5-3.0.9.5.jar                    |ValkyrieLib                   |valkyrielib                   |1.16.5-3.0.9.5      |DONE      |Manifest: NOSIGNATURE
		envirocore-1.16.5-3.0.9.3.jar                     |Environmental Core            |envirocore                    |1.16.5-3.0.9.3      |DONE      |Manifest: NOSIGNATURE
		envirotech-1.16.5-3.0.9.4.jar                     |Environmental Tech            |envirotech                    |1.16.5-3.0.9.4      |DONE      |Manifest: NOSIGNATURE
		Lollipop-1.16.5-3.2.9.jar                         |Lollipop                      |lollipop                      |3.2.9               |DONE      |Manifest: NOSIGNATURE
		ironfurnaces-1.16.5-2.7.7.jar                     |Iron Furnaces                 |ironfurnaces                  |2.7.7               |DONE      |Manifest: NOSIGNATURE
		toughnessbar-6.1.jar                              |Toughness Bar                 |toughnessbar                  |6.1                 |DONE      |Manifest: NOSIGNATURE
		mcw-trapdoors-1.0.4-mc1.16.5.jar                  |Macaw's Trapdoors             |mcwtrpdoors                   |1.0.4               |DONE      |Manifest: NOSIGNATURE
		supermartijn642corelib-1.0.16-mc1.16.5.jar        |SuperMartijn642's Core Lib    |supermartijn642corelib        |1.0.16              |DONE      |Manifest: NOSIGNATURE
		Botania-1.16.5-420.2.jar                          |Botania                       |botania                       |1.16.5-420.2        |DONE      |Manifest: NOSIGNATURE
		pamhc2foodextended-1.16.3-1.0.4.jar               |Pam's HarvestCraft 2 Food Exte|pamhc2foodextended            |version             |DONE      |Manifest: NOSIGNATURE
		curios-forge-1.16.5-4.0.8.0.jar                   |Curios API                    |curios                        |1.16.5-4.0.8.0      |DONE      |Manifest: NOSIGNATURE
		Patchouli-1.16.4-53.2.jar                         |Patchouli                     |patchouli                     |1.16.4-53.2         |DONE      |Manifest: NOSIGNATURE
		corail_woodcutter-1.16-2.0.1.jar                  |Corail Woodcutter             |corail_woodcutter             |2.0.1               |DONE      |Manifest: NOSIGNATURE
		tanknull-2.3-1.16.4.jar                           |Tank Null                     |tanknull                      |2.3-1.16.4          |DONE      |Manifest: NOSIGNATURE
		FramedBlocks-2.12.0.jar                           |FramedBlocks                  |framedblocks                  |2.12.0              |DONE      |Manifest: NOSIGNATURE
		elevatorid-1.16.5-1.7.13.jar                      |Elevator Mod                  |elevatorid                    |1.16.5-1.7.13       |DONE      |Manifest: NOSIGNATURE
		ftb-ultimine-forge-1605.3.1-build.45.jar          |FTB Ultimine                  |ftbultimine                   |1605.3.1-build.45   |DONE      |Manifest: NOSIGNATURE
		tombstone-6.7.1-1.16.5.jar                        |Corail Tombstone              |tombstone                     |6.7.1               |DONE      |Manifest: NOSIGNATURE
		buildersaddition-1.16.5-20210807a.jar             |Builders Crafts & Addition    |buildersaddition              |1.16.5-20210807a    |DONE      |Manifest: NOSIGNATURE
		Runelic-1.16.5-7.0.2.jar                          |Runelic                       |runelic                       |7.0.2               |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		ExtraStorage-1.16.5-1.6.0.jar                     |Extra Storage                 |extrastorage                  |1.6.0               |DONE      |Manifest: NOSIGNATURE
		constructionwand-1.16.5-2.6.jar                   |Construction Wand             |constructionwand              |1.16.5-2.6          |DONE      |Manifest: NOSIGNATURE
		cfm-7.0.0pre22-1.16.3.jar                         |MrCrayfish's Furniture Mod    |cfm                           |7.0.0-pre22         |DONE      |Manifest: NOSIGNATURE
		architectury-1.28.48.jar                          |Architectury                  |architectury                  |1.28.48             |DONE      |Manifest: NOSIGNATURE
		moreoverlays-1.18.17-mc1.16.5.jar                 |More Overlays Updated         |moreoverlays                  |1.18.17-mc1.16.5    |DONE      |Manifest: NOSIGNATURE
		light-overlay-5.8.1.jar                           |Light Overlay                 |lightoverlay                  |5.8.1               |DONE      |Manifest: NOSIGNATURE
		cloth-config-4.13.49-forge.jar                    |Cloth Config v4 API           |cloth-config                  |4.13.49             |DONE      |Manifest: NOSIGNATURE
		trashcans-1.0.12-mc1.16.jar                       |Trash Cans                    |trashcans                     |1.0.12              |DONE      |Manifest: NOSIGNATURE
		observable-0.2.1-forge.jar                        |Observable                    |observable                    |0.2.1               |DONE      |Manifest: NOSIGNATURE
		CodeChickenLib-1.16.5-4.0.6.443-universal.jar     |CodeChicken Lib               |codechickenlib                |4.0.6.443           |DONE      |Manifest: 31:e6:db:63:47:4a:6e:e0:0a:2c:11:d1:76:db:4e:82:ff:56:2d:29:93:d2:e5:02:bd:d3:bd:9d:27:47:a5:71
		CBMultipart-1.16.5-3.0.4.123-universal.jar        |CBMultipart                   |cb_multipart                  |3.0.4.123           |DONE      |Manifest: 31:e6:db:63:47:4a:6e:e0:0a:2c:11:d1:76:db:4e:82:ff:56:2d:29:93:d2:e5:02:bd:d3:bd:9d:27:47:a5:71
		ProjectRed-1.16.5-4.11.0-beta-6-core.jar          |ProjectRed Core               |projectred-core               |4.11.0-beta-6       |DONE      |Manifest: NOSIGNATURE
		ProjectRed-1.16.5-4.11.0-beta-6-illumination.jar  |ProjectRed Illumination       |projectred-illumination       |4.11.0-beta-6       |DONE      |Manifest: NOSIGNATURE
		ProjectRed-1.16.5-4.11.0-beta-6-transmission.jar  |ProjectRed Transmission       |projectred-transmission       |4.11.0-beta-6       |DONE      |Manifest: NOSIGNATURE
		ProjectRed-1.16.5-4.11.0-beta-6-integration.jar   |ProjectRed Integration        |projectred-integration        |4.11.0-beta-6       |DONE      |Manifest: NOSIGNATURE
		miniutilities-1.2.3.jar                           |Mini Utilities                |miniutilities                 |1.2.3               |DONE      |Manifest: NOSIGNATURE
		ClientTweaks_1.16.3-5.3.0.jar                     |Client Tweaks                 |clienttweaks                  |5.3.0               |DONE      |Manifest: NOSIGNATURE
		rhino-forge-1605.1.5-build.75.jar                 |Rhino                         |rhino                         |1605.1.5-build.75   |DONE      |Manifest: NOSIGNATURE
		Cucumber-1.16.5-4.1.12.jar                        |Cucumber Library              |cucumber                      |4.1.12              |DONE      |Manifest: NOSIGNATURE
		TrashSlot_1.16.3-12.2.1.jar                       |TrashSlot                     |trashslot                     |12.2.1              |DONE      |Manifest: NOSIGNATURE
		ftb-library-forge-1605.3.4-build.90.jar           |FTB Library                   |ftblibrary                    |1605.3.4-build.90   |DONE      |Manifest: NOSIGNATURE
		ftb-teams-forge-1605.2.3-build.40.jar             |FTB Teams                     |ftbteams                      |1605.2.3-build.40   |DONE      |Manifest: NOSIGNATURE
		pamhc2trees-1.16.3-1.0.1.jar                      |Pam's HarvestCraft 2 Fruit Tre|pamhc2trees                   |1.0.1               |DONE      |Manifest: NOSIGNATURE
		snad-1.0.9-forge.jar                              |Snad                          |snad                          |1.0.9               |DONE      |Manifest: NOSIGNATURE
		Bountiful Baubles FORGE-1.16.3-0.0.2.jar          |Bountiful Baubles             |bountifulbaubles              |NONE                |DONE      |Manifest: NOSIGNATURE
		jei-1.16.5-7.7.1.145.jar                          |Just Enough Items             |jei                           |7.7.1.145           |DONE      |Manifest: NOSIGNATURE
		JustEnoughCalculation-1.16.5-3.8.6.jar            |Just Enough Calculation       |jecalculation                 |3.8.6               |DONE      |Manifest: NOSIGNATURE
		item-filters-forge-1605.2.5-build.9.jar           |Item Filters                  |itemfilters                   |1605.2.5-build.9    |DONE      |Manifest: NOSIGNATURE
		AttributeFix-1.16.5-10.1.3.jar                    |AttributeFix                  |attributefix                  |10.1.3              |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		Tiny-Coal-1.16.4-1.0.0.jar                        |Tiny Coal                     |tinycoal                      |1.0.0               |DONE      |Manifest: NOSIGNATURE
		lemonlib-1.3.6.jar                                |Lemon Lib                     |lemonlib                      |1.3.6               |DONE      |Manifest: NOSIGNATURE
		Clumps-6.0.0.27.jar                               |Clumps                        |clumps                        |6.0.0.27            |DONE      |Manifest: NOSIGNATURE
		enviromats-1.16.5-2.0.9.0.jar                     |Environmental Materials       |enviromats                    |2.0.9.0             |DONE      |Manifest: NOSIGNATURE
		SimpleStorageNetwork-1.16.5-1.5.1.jar             |Simple Storage Network        |storagenetwork                |1.16.5-1.5.1        |DONE      |Manifest: 1f:47:ac:b1:61:82:96:b8:47:19:16:d2:61:81:11:60:3a:06:4b:61:31:56:7d:44:31:1e:0c:6f:22:5b:4c:ed
		framedcompactdrawers-1.16-2.2.1.jar               |Framed Compacting Drawers     |framedcompactdrawers          |1.16-2.2.1          |DONE      |Manifest: NOSIGNATURE
		configured-1.5.1-1.16.5.jar                       |Configured                    |configured                    |1.5.1               |DONE      |Manifest: NOSIGNATURE
		LibX-1.16.3-1.0.76.jar                            |LibX                          |libx                          |1.16.3-1.0.76       |DONE      |Manifest: NOSIGNATURE
		compactmachines-4.0.0-beta.2.jar                  |Compact Machines 4            |compactmachines               |4.0.0-beta.2        |DONE      |Manifest: NOSIGNATURE
		decorative_blocks-1.16.4-1.7.2.jar                |Decorative Blocks             |decorative_blocks             |1.7.2               |DONE      |Manifest: NOSIGNATURE
		FarmingForBlockheads_1.16.5-7.3.1.jar             |Farming for Blockheads        |farmingforblockheads          |7.3.1               |DONE      |Manifest: NOSIGNATURE
		pneumaticcraft-repressurized-1.16.5-2.15.1-297.jar|PneumaticCraft: Repressurized |pneumaticcraft                |1.16.5-2.15.1-297   |DONE      |Manifest: NOSIGNATURE
		TravelAnchors-2.4.jar                             |Travel Anchors                |travel_anchors                |2.4                 |DONE      |Manifest: NOSIGNATURE
		mcjtylib-1.16-5.1.3.jar                           |McJtyLib                      |mcjtylib                      |1.16-5.1.3          |DONE      |Manifest: NOSIGNATURE
		rftoolsbase-1.16-2.1.2.jar                        |RFToolsBase                   |rftoolsbase                   |1.16-2.1.2          |DONE      |Manifest: NOSIGNATURE
		xnet-1.16-3.0.16.jar                              |XNet                          |xnet                          |1.16-3.0.16         |DONE      |Manifest: NOSIGNATURE
		Interactio-1.16.4-3.1.1.jar                       |Interactio                    |interactio                    |1.16.4-3.1.1        |DONE      |Manifest: NOSIGNATURE
		rftoolspower-1.16-3.0.13.jar                      |RFToolsPower                  |rftoolspower                  |1.16-3.0.13         |DONE      |Manifest: NOSIGNATURE
		extradisks-1.16.4-1.5.1.jar                       |Extra Disks                   |extradisks                    |1.5.1               |DONE      |Manifest: NOSIGNATURE
		ImmersivePetroleum-1.16.5-3.3.0-11.jar            |Immersive Petroleum           |immersivepetroleum            |3.3.0-11            |DONE      |Manifest: NOSIGNATURE
		ftb-chunks-forge-1605.3.2-build.115.jar           |FTB Chunks                    |ftbchunks                     |1605.3.2-build.115  |DONE      |Manifest: NOSIGNATURE
		kubejs-forge-1605.3.19-build.258.jar              |KubeJS                        |kubejs                        |1605.3.19-build.258 |DONE      |Manifest: NOSIGNATURE
		kubejs-ui-forge-1605.1.4-build.12.jar             |KubeJS UI                     |kubejs_ui                     |1605.1.4-build.12   |DONE      |Manifest: NOSIGNATURE
		forge-1.16.5-36.2.23-universal.jar                |Forge                         |forge                         |36.2.23             |DONE      |Manifest: 22:af:21:d8:19:82:7f:93:94:fe:2b:ac:b7:e4:41:57:68:39:87:b1:a7:5c:c6:44:f9:25:74:21:14:f5:0d:90
		BloodMagic-1.16.4-3.1.7-27.jar                    |Blood Magic                   |bloodmagic                    |1.16.4-3.1.7-27     |DONE      |Manifest: NOSIGNATURE
		kubejs-blood-magic-1605.1.1-build.3.jar           |KubeJS Blood Magic            |kubejs_blood_magic            |1605.1.1-build.3    |DONE      |Manifest: NOSIGNATURE
		selene-1.16.5-1.9.0.jar                           |Selene                        |selene                        |1.16.5-1.0          |DONE      |Manifest: NOSIGNATURE
		ironchest-1.16.5-11.2.21.jar                      |Iron Chests                   |ironchest                     |1.16.5-11.2.21      |DONE      |Manifest: NOSIGNATURE
		CraftingTweaks_1.16.5-12.2.1.jar                  |Crafting Tweaks               |craftingtweaks                |12.2.1              |DONE      |Manifest: NOSIGNATURE
		ZeroCore2-1.16.5-2.1.9.jar                        |Zero CORE 2                   |zerocore                      |1.16.5-2.1.9        |DONE      |Manifest: NOSIGNATURE
		ExtremeReactors2-1.16.5-2.0.38.jar                |Extreme Reactors              |bigreactors                   |1.16.5-2.0.38       |DONE      |Manifest: NOSIGNATURE
		forge-1.16.5-36.2.23-client.jar                   |Minecraft                     |minecraft                     |1.16.5              |DONE      |Manifest: NOSIGNATURE
		TConstruct-1.16.5-3.3.2.324.jar                   |Tinkers' Construct            |tconstruct                    |3.3.2.324           |DONE      |Manifest: NOSIGNATURE
		rftoolsutility-1.16-3.1.9.jar                     |RFToolsUtility                |rftoolsutility                |1.16-3.1.9          |DONE      |Manifest: NOSIGNATURE
		EnchantmentDescriptions-1.16.5-7.0.18.jar         |EnchantmentDescriptions       |enchdesc                      |7.0.18              |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		theoneprobe-1.16-3.1.4.jar                        |The One Probe                 |theoneprobe                   |1.16-3.1.4          |DONE      |Manifest: NOSIGNATURE
		MouseTweaks-2.14-mc1.16.2.jar                     |Mouse Tweaks                  |mousetweaks                   |2.14                |DONE      |Manifest: NOSIGNATURE
		ftb-quests-forge-1605.3.6-build.76.jar            |FTB Quests                    |ftbquests                     |1605.3.6-build.76   |DONE      |Manifest: NOSIGNATURE
		ImmersiveEngineering-1.16.5-5.0.7-143.jar         |Immersive Engineering         |immersiveengineering          |1.16.5-5.0.7-143    |DONE      |Manifest: 44:39:94:cf:1d:8c:be:3c:7f:a9:ee:f4:1e:63:a5:ac:61:f9:c2:87:d5:5b:d9:d6:8c:b5:3e:96:5d:8e:3f:b7
		pamhc2crops-1.16.3-1.0.2.jar                      |Pam's HarvestCraft 2 Crops    |pamhc2crops                   |version             |DONE      |Manifest: NOSIGNATURE
		SkyblockBuilder-1.16.4-1.6.13.jar                 |Skyblock Builder              |skyblockbuilder               |1.16.4-1.6.13       |DONE      |Manifest: NOSIGNATURE
		Ding-1.16.5-1.3.0.jar                             |Ding                          |ding                          |1.3.0               |DONE      |Manifest: NOSIGNATURE
		NBT-Ingredient-Predicate-1.3.jar                  |NBT Ingredient Predicate      |nbt_ingredient_predicate      |1.3                 |DONE      |Manifest: NOSIGNATURE
		rftoolsbuilder-1.16-3.1.5.jar                     |RFToolsBuilder                |rftoolsbuilder                |1.16-3.1.5          |DONE      |Manifest: NOSIGNATURE
		jeiintegration_1.16.5-7.0.1.15.jar                |JEI Integration               |jeiintegration                |7.0.1.15            |DONE      |Manifest: NOSIGNATURE
		pipez-1.16.5-1.2.15.jar                           |Pipez                         |pipez                         |1.16.5-1.2.15       |DONE      |Manifest: NOSIGNATURE
		flywheel-1.16-0.2.5.jar                           |Flywheel                      |flywheel                      |1.16-0.2.5          |DONE      |Manifest: NOSIGNATURE
		create-mc1.16.5_v0.3.2g.jar                       |Create                        |create                        |v0.3.2g             |DONE      |Manifest: NOSIGNATURE
		Mantle-1.16.5-1.6.152.jar                         |Mantle                        |mantle                        |1.6.152             |DONE      |Manifest: NOSIGNATURE
		pamhc2foodcore-1.16.3-1.0.2.jar                   |Pam's HarvestCraft 2 Food Core|pamhc2foodcore                |version             |DONE      |Manifest: NOSIGNATURE
		itemcollectors-1.1.4-mc1.16.jar                   |Item Collectors               |itemcollectors                |1.1.4               |DONE      |Manifest: NOSIGNATURE
		ftb-backups-2.1.2.2.jar                           |FTB Backups                   |ftbbackups                    |2.1.2.2             |DONE      |Manifest: NOSIGNATURE
		creativewirelesstransmitter-1.16x-1.12.jar        |Creative Wireless Transmitter |creativewirelesstransmitter   |1.16x-1.12          |DONE      |Manifest: NOSIGNATURE
		oauth-1.1.11-1.16.jar                             |OAuth                         |oauth                         |1.1.11              |DONE      |Manifest: NOSIGNATURE
		FastWorkbench-1.16.5-4.6.1.jar                    |Fast Workbench                |fastbench                     |4.6.1               |DONE      |Manifest: NOSIGNATURE
		polymorph-forge-1.16.5-0.39.jar                   |Polymorph                     |polymorph                     |1.16.5-0.39         |DONE      |Manifest: NOSIGNATURE
		JustEnoughProfessions-1.16.5-1.2.2.jar            |Just Enough Professions (JEP) |justenoughprofessions         |1.2.2               |DONE      |Manifest: NOSIGNATURE
		AutoRegLib-1.6-49.jar                             |AutoRegLib                    |autoreglib                    |1.6-49              |DONE      |Manifest: NOSIGNATURE
		Quark-r2.4-321.jar                                |Quark                         |quark                         |r2.4-321            |DONE      |Manifest: NOSIGNATURE
		StorageDrawers-1.16.3-8.5.1.jar                   |Storage Drawers               |storagedrawers                |8.5.1               |DONE      |Manifest: NOSIGNATURE
		topaddons-1.16.5-2.2.0-beta.jar                   |TOP Addons                    |topaddons                     |1.16.5-2.2.0-beta   |DONE      |Manifest: NOSIGNATURE
		FluxNetworks-1.16.5-6.2.1.14.jar                  |Flux Networks                 |fluxnetworks                  |6.2.1.14            |DONE      |Manifest: NOSIGNATURE
		performant-1.16.2-5-3.84m.jar                     |Performant                    |performant                    |3.73m               |DONE      |Manifest: NOSIGNATURE
		enderchests-1.16-1.7.9.jar                        |EnderChests                   |enderchests                   |1.7.9               |DONE      |Manifest: NOSIGNATURE
		globaldataandresourcepacks-1.16.5-1.10.2.jar      |Global Data- & Resourcepacks  |globaldataandresourcepacks    |1.10.2              |DONE      |Manifest: NOSIGNATURE
		structurize-0.13.252-ALPHA-universal.jar          |Structurize                   |structurize                   |0.13.252-ALPHA      |DONE      |Manifest: NOSIGNATURE
		RSLargePatterns-1.16.5-2.1.0.3.jar                |Refined Storage Large Patterns|rslargepatterns               |2.1.0.3             |DONE      |Manifest: NOSIGNATURE
		kubejs-create-1605.1.4-build.12.jar               |KubeJS Create                 |kubejs_create                 |1605.1.4-build.12   |DONE      |Manifest: NOSIGNATURE
		minecolonies-1.16.5-1.0.352-BETA.jar              |MineColonies                  |minecolonies                  |1.16.5-1.0.352-BETA |DONE      |Manifest: NOSIGNATURE
		FastFurnace-1.16.5-4.5.0.jar                      |FastFurnace                   |fastfurnace                   |4.5.0               |DONE      |Manifest: NOSIGNATURE
		appleskin-forge-mc1.16.x-2.3.0.jar                |AppleSkin                     |appleskin                     |2.3.0+mc1.16.4      |DONE      |Manifest: NOSIGNATURE
		mobcatcher-1.16.4-3.2a.jar                        |Mob Catcher                   |mobcatcher                    |1.16.4-3.2a         |DONE      |Manifest: NOSIGNATURE
		ferritecore-2.1.0-forge.jar                       |Ferrite Core                  |ferritecore                   |2.1.0               |DONE      |Manifest: 41:ce:50:66:d1:a0:05:ce:a1:0e:02:85:9b:46:64:e0:bf:2e:cf:60:30:9a:fe:0c:27:e0:63:66:9a:84:ce:8a
		engineersdecor-1.16.5-1.1.16.jar                  |Engineer's Decor              |engineersdecor                |1.1.16              |DONE      |Manifest: bf:30:76:97:e4:58:41:61:2a:f4:30:d3:8f:4c:e3:71:1d:14:c4:a1:4e:85:36:e3:1d:aa:2f:cb:22:b0:04:9b
		Chisel-MC1.16.5-2.0.1-alpha.4.jar                 |Chisel                        |chisel                        |MC1.16.5-2.0.1-alpha|DONE      |Manifest: NOSIGNATURE
		SoL-Carrot-1.16.5-1.10.1.jar                      |Spice of Life: Carrot Edition |solcarrot                     |1.16.5-1.10.1       |DONE      |Manifest: NOSIGNATURE
		kubejs-immersive-engineering-1605.1.2-build.28.jar|KubeJS Immersive Engineering  |kubejs_immersive_engineering  |1605.1.2-build.28   |DONE      |Manifest: NOSIGNATURE
		refinedstorageaddons-0.7.4.jar                    |Refined Storage Addons        |refinedstorageaddons          |0.7.4               |DONE      |Manifest: NOSIGNATURE
		extremeSoundMuffler-3.17_1.16.5.jar               |Extreme Sound Muffler         |extremesoundmuffler           |3.17_forge-1.16.5   |DONE      |Manifest: NOSIGNATURE
		overloadedarmorbar-5.1.0.jar                      |Overloaded Armor Bar          |overloadedarmorbar            |5.1.0               |DONE      |Manifest: NOSIGNATURE
		chiselsandbits-1.0.63.jar                         |Chisels & bits                |chiselsandbits                |1.0.63              |DONE      |Manifest: NOSIGNATURE
		createaddition-1.16.5-20211215b.jar               |Create Crafts & Additions     |createaddition                |1.16.5-20211215b    |DONE      |Manifest: NOSIGNATURE
	FramedBlocks BlockEntity Warning: Not applicable
	Crash Report UUID: 5bcab6e0-0786-4831-b2a2-cf36895988d9
	Patchouli open book context: n/a
	Launched Version: forge-36.2.23
	Backend library: LWJGL version 3.2.2 build 10
	Backend API: NVIDIA GeForce RTX 2060 SUPER/PCIe/SSE2 GL version 4.6.0 NVIDIA 471.41, NVIDIA Corporation
	GL Caps: Using framebuffer using OpenGL 3.0
	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'forge'
	Type: Client (map_client.txt)
	GPU Warnings: renderer: Stencil enabled in Immersive Engineering config
	Graphics mode: fancy
	Resource Packs: 
	Current Language: English (US)
	CPU: 12x AMD Ryzen 5 3600 6-Core Processor 
