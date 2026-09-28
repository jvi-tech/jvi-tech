# JVI-TECH Launcher — Phase 1 Analysis Prompt

You are analyzing an existing FYT UI47 launcher. Do NOT build a new launcher from scratch.

The repository contains:
- the original UI47 APK
- decoded Android resources/XML
- classes.dex and a class/method inventory
- selected launcher layouts
- selected UI assets
- a preliminary UI47 component map

A separate reference image named `JVI-TECH_LAUNCHER_MASTER_V1` may be attached to the chat. Treat it only as the target UI reference.

## Phase 1: analysis only

Do not modify files. Do not build an APK. Do not rename the package. Do not replace FYT/SYU services.

Determine:
1. UI47 package, launcher Activity, sharedUserId and HOME behavior.
2. How launcher.xml, custom_layout_one.xml and resolution variants compose the Home screen.
3. Which classes control Workspace, DragLayer, Hotseat, AppsCustomizePagedView, PageIndicator and other Home components.
4. Which FYT/SYU services/providers supply Music, Radio, Clock, Date, Weather, Navigation, Video/DVR and other data.
5. Which drawables/assets create the current Home UI.
6. Which existing components can be reused unchanged.
7. Which files should be modified to reproduce the JVI-TECH MASTER V1 interface.
8. Which changes require code rather than resource/layout changes.
9. Risks and dependencies for every proposed modification.

Return:
- an architecture diagram in text;
- a table: Target UI area | Existing UI47 file/class | Dependency | Reuse? | Required change | Risk;
- a minimal ordered edit list;
- a list of files that must not be changed unless technically necessary;
- any missing source/data needed for a definitive conclusion.

Do not start implementation until the user explicitly confirms the analysis.
