# BoardGameCollector
A project for Ubiquitous classes at the PUT.

## Table of contents
* [General Info](#general-info)
* [How to Launch](#how-to-launch)
* [Additional Info](#additional-info)

# General Info
This is an Android application that stores data about user's games and extension packs on [BoardGameGeek](https://boardgamegeek.com). Each panel of this app is described below.

I used SQLite DB for data storage.

## Type username panel
<p align="center">
  <img src="https://user-images.githubusercontent.com/72743103/185386200-5456f098-a365-4959-8e26-57699c706bc1.png" width="300">
</p>

The panel only appears at startup and if the database is empty. Allows you to enter a username and check if that user exists. If a user with this username exists forwards to [Sync panel](#sync-panel).

## Sync panel
<p align="center">
  <img src="https://user-images.githubusercontent.com/72743103/185386871-85b13c04-2367-4d8a-a84d-c276934b64f1.png" width="300">
</p>

This panel shows the username and last sync date. You can sync the database with the service, but if time since last sync is less than 24h the app will ask you if still want to do so. While syncing, a progress bar will appear in place of the synchornize button. After whole process you will be redirected to the Main Menu panel.

## Main Menu panel
<p align="center">
  <img src="https://user-images.githubusercontent.com/72743103/185387619-dc8f2bdb-2fe1-4b87-a3b7-1c521c51b7f7.png" width="300">
</p>

The Main Menu panel appears at the start of the application when database is not empty. From this panel you can:
- see all user games ("Games" button) [Games panel](#games-panel)
- see all user extension packs ("Extension packs" button) [Extension packs panel](#extension-packs-panel)
- update the database by synchronizing with the service [Sync panel](#sync-panel)
- delete all data ("Wipe out data" button, you will be asked if you are sure about this)

## Games panel
<p align="center">
  <img src="https://user-images.githubusercontent.com/72743103/185388695-4cf9842f-2b7b-42b1-b176-9977dc846d33.png" width="300">
</p>

This panel shows the data (ordinal number, image, title, year published, rank) about each user's game. The user can sort the games by rank, title or year of publication. After clicking on the game you will be moved to the [Game Ranking panel](#game-ranking-panel). 

## Game ranking panel
<p align="center">
  <img src="https://user-images.githubusercontent.com/72743103/185389665-21c31ace-4fba-40ec-9733-3398bdd2e692.png" width="300">
</p>

The game ranking panel shows up the image, title and year of publication of the game and how ranking of this game has changed over syncs.

## Extension packs panel
<p align="center">
  <img src="https://user-images.githubusercontent.com/72743103/185390333-082a768f-3baa-4394-be6f-9a33da84cf63.png" width="300">
</p>

Similar to the [Games panel](#games-panel) this panel presents the data (ordinal number, image, title and year of publication) of each extension pack. The user  can also sort these extension packs by title or year of publication.

# How to launch
The easiest way to run this project is to download it and [Android Studio](https://developer.android.com/studio?gclid=CjwKCAjwo_KXBhAaEiwA2RZ8hPP6GtBza_vfZtw41dKXdoDqJfAlvgunOwd8aEB7j9gbAeT-b1n36RoCwJsQAvD_BwE&gclsrc=aw.ds). Then open the project in the downloaded IDE. Next you have to create a device emulator or connect a phone to IDE. Finally, select device and run project on it - after some time (about 1 minute) the application will be installed on your phone/emulator.

# Additional Info
The app has only been tested on Android 11

