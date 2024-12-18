# Travel Diary App

The Travel Diary App is a mobile application designed for users to document and preserve their travel experiences, including locations, photos, and personal notes, with a focus on privacy and simplicity.

## Overview

This app is ideal for travellers who value a personal and organized way to document their journeys.

## Team Members
| Group Member | Student ID | Contribution |
|--------------|------------|--------------|
|Kevin Chua|100927701| Everything related to Calendar, Local Storage, Everything related to Tags, Save images to Cloudinary | 
|YuChen Huang|100869400|Homepage Entry display, Diary Editor, Multi Image Saving |
|Dante Cornelius|100882223| Localizations Files,Languages Translation,Accessibility,Theme,Notification |
|Zhenghao Liao|100649902| code abstraction (some Utils and Service); Everything related to Map, Location and Address |
|Oluwateniola Adegbite|100861337|  UI styler, Settings, some code optimization, accessibilty features. Everything related to UI and some Localization.|

## HomePage

The `HomePage` is the main interface of the Travel Diary app, where users can view, create, and edit diary entries. It provides an intuitive interface for managing and displaying travel records.

### Features

- **Tag Filtering**: Filter diary entries by tags to quickly find entries by specific topics or moods.
- **Diary Display**: Entries are displayed in chronological order, with support for deletion and editing. Each entry shows the date, time, content summary, weather, and mood icons.
- **New Entry Creation**: Click the button to create a new diary entry and enter the `DiaryEditor` for editing.

### Instructions

#### Creating an Entry

1. Click the "New Entry" button on the homepage.
2. Fill in the diary content in the `DiaryEditor`.
3. Click the save button to return to the homepage.

#### Editing an Entry

1. Click on a diary entry on the homepage.
2. Modify the content in the `DiaryEditor`.
3. Click the save button to update the entry.

#### Deleting an Entry

1. On the homepage, swipe the diary entry you want to delete to the left.
2. A delete icon will appear on the right side.
3. The entry will be removed from the list and deleted from the database.

#### Diary Display

- Shows the date, time, content summary, weather, and mood icons.
- Displays a thumbnail of the first image (if available).
- Supports swipe-to-delete functionality.

#### Status Bar

- Displays the current filter tags.
- Click tags to select or deselect filters.

The `HomePage` provides a clean and powerful interface to help users easily manage and browse their travel diaries.


## Atlas (Map view)

### Features

- **Markers Layer**: shows an interactable pin for each journal that has a location attribute
- **Tile Layer**: use Thunderforest API to show the map in atlas style
- **Attribution Layer**: shows attribution information for Thunderforest and OpenStreetMap
- **Interaction**: Familiar navigation style of Pinching and Dragging

### Interactive Features
The map have gestures for quick access:
| Action | Gesture | Result |
|--------|---------|--------|
| View entry details | Tap Pin Marker | Opens detailed view with photos |
| Edit entry | Long press Pin Marker | Opens Diary Editor for existing entry |

## Diary Editor

The `DiaryEditor` is a key component of the Travel Diary app, providing users with an intuitive interface to create and edit diary entries. It offers a range of features to enhance the documentation of travel experiences.

### Features

- **Simple Text Editing**: Write and edit diary entries with ease.
- **Date and Time Selection**: Select and update the date and time for each entry.
- **Image Management**: Add multiple images from the camera, gallery, or via URL. Images can be viewed in full screen or deleted with confirmation.
- **Location Tagging**: Tag entries with a location using a map interface. Users can pick from map, use current location, edit, or delete locations.
- **Weather, Activity, and Feeling Icons**: Customize entries with icons representing the weather, activities, and feelings.
- **Tagging System**: Add and manage tags for each entry, with a dynamic filter chip interface.

The `DiaryEditor` is designed to enhance the user experience by providing a comprehensive and intuitive interface for managing diary entries.

## Tags
Tags provide a powerful way to organize and filter your journal entries. By adding tags to your entries, you can:
- Quickly categorize entries by topic, mood, or any custom category
- Filter entries on the Home page using one or multiple tags
- Track patterns and themes in your journaling practice

## Calendar View
The `Calendar` offers an intuitive chronological view of your journaling history with multiple interactive features.
### View Options
- Monthly View: Traditional calendar layout showing the full month
- 2-Week View: Focused view of the current and next week
- Weekly View: Detailed view of the current week with expanded entry previews

### Interactive Features
The `Calendar` supports various gestures for quick access:
| Action | Gesture | Result |
|--------|---------|--------|
| View date entries | Tap date | Shows entries for selected date below |
| Create new entry | Long press date | Opens Diary Editor for new entry |
| View entry details | Tap entry card | Opens detailed view with photos |
| Edit entry | Long press entry card | Opens Diary Editor for existing entry |

## Customization
All customization settings are persisted locally for a personalized experience across sessions.

### Theme Options
- Dark Mode: Comfortable viewing in low-light conditions
- High Contrast Mode: Enhanced readability with increased contrast ratios
- Theme Colors: Personalize the app's color scheme


## Run instructions
1. `cd travel_diary`
2. `flutter clean`
3. `flutter pub get`
4. `flutter gen-l10n`
5. `flutter build apk`
6. `flutter install`
