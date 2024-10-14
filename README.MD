
# NBTAddons

[![Build Status](https://ci.thom.club/job/TheExoticsMod/job/master/badge/icon)](https://ci.thom.club/job/TheExoticsMod/job/master/) [![Contributors](https://img.shields.io/github/contributors/TGWaffles/TheExoticsMod?&logo=GitHub)](https://github.com/TGWaffles/TheExoticsMod/graphs/contributors) [![Jenkins Coverage](https://img.shields.io/jenkins/coverage/jacoco?jobUrl=https%3A%2F%2Fci.thom.club%2Fjob%2FTheExoticsMod%2Fjob%2Fmaster)](https://ci.thom.club/job/TheExoticsMod/job/master/jacoco/) [![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fci.thom.club%2Fjob%2FTheExoticsMod%2Fjob%2Fmaster)](https://ci.thom.club/job/TheExoticsMod/job/master/lastBuild/testReport/)

---

__What is NBTAddons?__

NBTAddons is an open source, community-led effort to track every single item in Hypixel Skyblock.

NBTAddons shows data such as uuid, timestamp, exotics/crystal armor, where the item was dropped and much more to be able to provide "active dupe checking", item ownership history, quick access to item nbt, hypixel searches, item statistics/rarity, and more to come.

It also provides handy in-game features, such as lobby scanning for exotics, exotic labelling (eg fairy/spooky/exotic/glitched), copying item uuid to clipboard, dupe-checking via a hotkey, and armour rarity annotations (how many there are in the game).

At the moment, it takes 12 hours for any item/inventory update to be reflected in the NBTAddons database. We have over 110 million items tracked, and almost 15 million players known about.

NBTAddons also includes qol features such as: 
-Dungeon secret routes (routes recorded by cata 61)
-Slayer qol
-Farming qol
-Dungeons qol
-Party commands such as (!warp, !party, !disband)

---
## How to build?

### Protoc Files

`protoc -I . --java_out annotate_code:src/main/java/ clientMessages.proto`

`protoc -I . --java_out annotate_code:src/main/java/ serverMessages.proto`
