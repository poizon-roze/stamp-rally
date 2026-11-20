# stamp-rally
# Stamp Rally 📍

A personal GPS-based stamp rally web app for exploring places, collecting digital stamps, and keeping a small travel journal.

I made this for my walks and day trips. Instead of just visiting places, I wanted a simple way to record where I've been, collect stamps, and make exploring a little more fun.

## How It Works

1. Open the app on your iPhone.
2. Enable GPS to get your current location.
3. Add a place you want to visit, give it a name, and set its GPS radius (50–500 meters).
4. When you visit the place, tap **Verify & Stamp**.
5. If your GPS position is within the allowed radius, you receive a digital stamp.
6. Add a photo of your sketch and some notes to the journal.

You can also set your position manually for testing.

## Stamp Rules

- Maximum **one stamp per location per day**.
- The daily limit resets at **00:00 JST**.
- You can visit the same location again on another day.
- Each stamp card holds **10 stamps**.
- A new card starts when the current card is full or the month ends.
- Your lifetime stamp count remains saved.

## Rewards ☕🥐🍫

Collect stamps to unlock small rewards, including coffee, croissants, and chocolate.

These are just fun notifications and personal achievements, not actual coupons or free products.

## Main Features

- **Rally:** Add locations, check distances, and collect stamps.
- **Map:** View your saved locations on a map.
- **Journal:** Keep a record of visits, dates, photos, and notes.
- **Backup:** Export your data as a JSON file and restore it later.
- **Stamp Cards:** Track monthly progress and lifetime stamps.

## Data and Privacy

The app is designed to store personal data locally on the device using IndexedDB.

Locations, notes, and photos are not included in the website's source code.

There is no cloud sync in this version.

**Important:** Browser data can be lost or cleared. Save a backup regularly, preferably after each trip. Test the restore function before depending on it.

## Notes

- Designed mainly for iPhone and Safari.
- Intended to run as a standalone website using GitHub Pages.
- GPS requires location permission.
- Manual positioning is useful for testing but is not proof of a real visit.
- This is a personal project, not a commercial app.

## Project History

Started in November 2026.

The idea originally came from an iPhone Shortcuts project called **Tzu Stamp Rally**, which used GPS and NFC for location check-ins.

This web version was built with the help of Claude (Anthropic), with the aim of making the rally easier to use without relying on Shortcuts.

Made for personal use, just for fun.
