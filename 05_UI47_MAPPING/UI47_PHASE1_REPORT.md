# JVI-TECH UI47 — Phase 1 resource package

## Status
The original UI47 APK has been structurally inspected and the resource/UI layer has been mapped.
This package is intended for the first analysis pass in Google AI Studio.

## Key facts
- Package: com.android.launcher47
- HOME Activity: com.android.launcher47.Launcher
- sharedUserId: android.uid.system
- DEX: classes.dex, 1162 class definitions
- Main UI root: res/layout-land/launcher.xml
- Primary custom home UI: res/layout-land/custom_layout_one.xml
- Important FYT/SYU integration classes:
  - com.fyt.car.MusicService
  - com.fyt.widget.DigitClock
  - com.fyt.widget.Date
  - com.fyt.widget.WeekDay
  - com.fyt.widget.HorizontalListView
  - com.syu.widget.music.DateMusicProvider
  - com.syu.widget.music.DateTimeProvider1

## Important limitation
This package contains the original APK, decoded XML resources, raw DEX, and a targeted class/string inventory. It does NOT claim to contain a full Java decompilation produced by JADX. The purpose of this phase is to give Google AI Studio a clean, bounded representation of the original launcher before any modification.

## Rule
Do not create a new launcher architecture. Treat UI47 as the technical base. Keep FYT/SYU system integration intact and modify the existing UI/resources first.
