# Setup for RetroMCP

1. Clone and compile [RelativityMC's stich fork](https://github.com/RelativityMC/stitch)

2. Run this commands in a command promt window in a folder with the compiled stich jar and the mappings 

```Shell
java -jar stitch-0.6.4+local-all.jar reorderTinyV2 intermediary-cypress-clientv2.tiny intermediary-flipped.tiny intermediary official

java -jar stitch-0.6.4+local-all.jar mergeTinyV2 intermediary-flipped.tiny mappings-clientv2.tiny mappings-merged.tiny

java -jar stitch-0.6.4+local-all.jar reorderTinyV2 mappings-merged.tiny mapping-client-merged-flipped.tiny official intermediary named
```
3. Download [RetroMCP](https://github.com/MCPHackers/RetroMCP-Java) and run setup for Alpha 1.1.2_01 

4. Copy mapping-client-merged-flipped.tiny to the RetroMCP folder and rename it to client.tiny

5. Open RetroMCP and run the Merge Mappings task, then move the merged.tiny to the conf folder and rename it mappings.tiny

6. Copy all the files in the rmcp-config folder in this repo to the RetroMCP conf folder

7. In RetroMCP set Options->Side->Client, then go Options->Recompile->Set a specific source version and change it from -1 to 7, do the same for Options->Recompile->Set a specific target version, set Options->Decompile->Keep Resources (The last one allows you to edit the textures, sounds, ect)

8. Download the cypress client copy it to the RetroMCP jars folder and rename it to minecraft.jar 

9. Click decompile
