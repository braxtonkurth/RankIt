# Rank It!

Rank It! is a full-stack media-ranking application that allows users to create, organize, reorder, and share personalized ranked lists.

The application is designed for ranking movies, games, books, shows, manga, music, or any other collection of items a user wants to compare.

## Live Application

[View Rank It!](https://www.braxtonkurth.com/#/rankit)

## Features

### Ranked Lists

- Create multiple personalized ranking lists
- Add and remove ranked items
- Reorder items through drag-and-drop controls
- Reorder lists from the sidebar
- Automatically maintain consistent item positions
- Manage up to 10 lists per user

### Real-Time Updates

- Synchronize list changes through Firebase Firestore
- Update the interface when ranking data changes
- Apply ordering changes using batched database writes
- Automatically shift surrounding item ranks after an insertion or deletion

### Sharing and Privacy

- Create public lists that other users can browse
- Keep selected lists private
- Browse shared rankings without modifying the owner's data
- Control the visibility of each list

### Guest Browsing

- Explore the application without creating a permanent account
- Maintain a guest session between visits
- Test ranking and browsing functionality before signing in

### Data Export

- Export ranking data as a downloadable text backup
- Preserve a portable copy of personal lists
- Generate the backup directly from the browser

## Technology Stack

### Frontend

- React
- TypeScript
- dnd-kit

### Backend and Data

- Firebase
- Cloud Firestore
- Firebase Authentication

## Technical Highlights

- Firestore `onSnapshot` subscriptions provide real-time data updates
- Batched writes keep item ordering consistent across database operations
- Inserting or deleting an item automatically shifts the ranks of surrounding items
- dnd-kit supports drag-and-drop ordering for both individual items and the list sidebar
- Updated list positions are synchronized with Firestore
- Guest sessions persist between browser sessions
- Client-side export generates a downloadable text backup without requiring a separate export service

## Project Status

Rank It! is a completed personal full-stack project and is available through the live application linked above.

## Source Code

The source code for Rank It! is maintained in a private GitHub repository.

This public repository provides project documentation, release information, and access to the deployed application. The production source code is not publicly distributed.

## Author

Braxton Kurth

[View My Portfolio](https://www.braxtonkurth.com/)
