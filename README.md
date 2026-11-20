# Stamp Rally 📍

Created by Claude from the brainstorming between me, Watson and Brick.
A personal GPS-based stamp rally web app for collecting digital stamps, tracking visits, and keeping a travel journal.

I made this for my walks and day trips. I wanted a simple way to remember the places I've visited, collect stamps, and make exploring a little more fun.

The project started as an iPhone Shortcuts experiment called **Tzu Stamp Rally**. It later became a web app, and now the plan is to use both together.

## How the Hybrid System Works

The system has two parts:

**Tzu (Apple Shortcuts)**

Tzu acts as a location reminder.

- Detects when I enter a saved area using an iPhone location automation.
- Sends a notification when I arrive.
- The notification is intended to provide a way to open the Stamp Rally web app.
- Does not collect stamps automatically.

**Stamp Rally Web App**

The web app handles the actual stamp collection.

- Opens from Tzu's notification or directly in Safari.
- Checks my current GPS position.
- Lets me verify my location and claim a stamp.
- Saves my stamps, photos, and notes.
- Tracks progress and rewards.

This way, Tzu reminds me when I'm near a location, while the web app manages my stamp collection.

## How to Use

1. Add a location to the web app, including its name, coordinates, and allowed radius (50–500 meters).
2. Set up the matching location in Tzu's iPhone automation.
3. When I arrive, Tzu should send a notification.
4. Tap the notification to access the web app.
5. Tap **Verify & Stamp** to check my GPS position.
6. If the location check passes and I haven't claimed today's stamp, collect it.
7. Add a photo of my sketch and notes to the journal.

I can also open the web app manually without waiting for Tzu.

The notification-to-web-app workflow is still being tested on a real iPhone.

## Stamp Rules

- Maximum **one stamp per location per day**.
- The daily limit resets at **00:00 JST**.
- The same location can be visited and stamped again the next day.
- Previous stamps and journal entries are never removed by the daily reset.
- Each stamp card has **10 slots**.
- A new card starts when the current card is full or a new month begins.
- Lifetime stamp totals are kept separately.

## Rewards ☕🥐🍫

Collect stamps to unlock small achievements, including coffee, croissants, and chocolate.

Rewards are just fun notifications, not real coupons or free products.

## Main Features

**Rally**
- Add and manage stamp locations.
- Check distances and GPS accuracy.
- Verify visits and claim stamps.
- View nearby locations.

**Map**
- See saved locations on a map.

**Stamp Cards**
- Track progress on a 10-stamp card.
- Start a new card when needed.
- Keep a lifetime stamp count.

**Journal**
- Record visit dates and times.
- Attach photos of sketches.
- Add notes about each visit.
- Keep a history of collected stamps.

**Backup**
- Export data to a JSON file.
- Restore saved data from a backup.
- Keep copies in Files or iCloud Drive.

## GPS and Location Checks

The web app uses the iPhone's GPS to check whether I'm within the allowed radius of a saved location.

Manual positioning is available for testing, but it can bypass real-location verification. It should not be treated as proof of a visit.

Tzu's arrival notification is only a reminder. The web app still needs to verify the location before awarding a stamp.

## Data and Privacy

Personal data is stored locally on the device using IndexedDB.

This includes:
- Saved locations and coordinates.
- Stamp history.
- Journal notes and sketch photos.
- Progress and reward records.

The personal data is not included in the GitHub repository.

There is no cloud sync in this version. Browser data may be cleared, so regular backups are important.

**Save a backup after each trip, and test the restore function before relying on it.**

## Technical Notes

- Designed mainly for iPhone and Safari.
- Web app hosted using GitHub Pages.
- Uses HTTPS and browser location permissions.
- Uses IndexedDB for local storage.
- Uses Apple Shortcuts location automations for the planned arrival notifications.
- Tzu and the web app have separate responsibilities.
- NFC was part of the original idea but is no longer required.
- The GPS and notification workflow needs real-device testing.

## Project History

**November 2026**

The project began as **Tzu Stamp Rally**, an iPhone Shortcuts experiment using NFC, GPS, and location-based check-ins.

Later, I asked Claude (Anthropic) to build a standalone web version with stamp cards, rewards, a map, a journal, and backups.

The first version ran inside Claude, but GPS access was a problem. The app was then adapted for hosting through GitHub Pages.

The next step is a **hybrid system**, where Tzu detects arrival and the web app handles verification and stamp collection.

The goal is to keep the app simple, useful, and enjoyable during my walks.

## Current Status

- Web app prototype created.
- GitHub Pages version being tested.
- Stamp cards, rewards, journal, and backup features included.
- Hybrid Tzu notification system planned.
- Full iPhone testing and verification still needed.

Built for personal use, just for fun.
