# FFXIV Quest Tracker

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Platform](https://img.shields.io/badge/platform-Android-green.svg)
![API](https://img.shields.io/badge/API-24%2B-brightgreen.svg)

A comprehensive Android application for tracking, managing, and visualizing Final Fantasy XIV quests and seasonal events. This app allows players to keep track of their in-game progression, monitor time spent on quests, and stay updated on seasonal events.

## Features

### Quest Management
- **Track All Quests**: Main scenario, side quests, job quests, and more
- **Quest Details**: Complete information including location, required level, rewards
- **Time Tracking**: Monitor time spent on each quest
- **Completion Status**: Mark quests as complete/incomplete
- **Filtering & Sorting**: Organize quests by expansion, type, and more

### Seasonal Events
- **Event Calendar**: Keep track of all FFXIV seasonal events
- **Event Details**: View comprehensive information about each event
- **Event Reminders**: Get notifications when events start
- **Calendar Integration**: Add events to your device calendar

### Character Integration
- **Character Search**: Find your FFXIV character via the Lodestone
- **MSQ Progress**: View and import your main scenario quest progress
- **Class/Job Levels**: Track your character's class/job progression

### Dashboard
- **Visual Statistics**: Interactive charts showing quest completion rates
- **Progress Tracking**: Visualized progression through each expansion
- **Recent Activity**: Track recently completed quests

## Architecture & Technical Implementation

This app is built with modern Android development practices:

- **Architecture**: MVVM with Clean Architecture principles
- **UI**: XML-based UI with Material Design components
- **Backend**:
  - Room Database for local storage
  - Retrofit for API communication
  - Kotlin Coroutines + Flow for asynchronous operations
- **Dependency Injection**: Dagger Hilt
- **Navigation**: Jetpack Navigation Component
- **Visualization**: Recharts for React-based charts
- **WebView Integration**: Dashboard visualization with React components

### Key Components

- **Data Layer**:
  - Room Database with Entities for Quests and Seasonal Events
  - Repository pattern for data access
  - TypeConverters for complex data types

- **Domain Layer**:
  - Use Cases for business logic
  - Models representing domain entities

- **UI Layer**:
  - ViewModels for UI state management
  - Fragments for UI presentation
  - Adapters for RecyclerViews
  - Navigation handling

- **Services**:
  - Background service for quest time tracking
  - Notification service for event alerts

## Getting Started

### Prerequisites
- Android Studio Arctic Fox (2021.3.1) or newer
- Android SDK 24 or higher
- Kotlin 1.9.0 or higher

### Setup
1. Clone the repository:
```bash
git clone https://github.com/yourusername/ffxiv-quest-tracker.git
```

2. Open the project in Android Studio

3. Configure your XIVAPI key in `app/build.gradle.kts`:
```kotlin
buildConfigField("String", "XIVAPI_KEY", "\"YOUR_API_KEY\"")
```

4. Build and run the application

## Future Enhancements

- Full character synchronization with FFXIV Lodestone
- Duty/raid tracking functionality
- Achievement tracking
- Crafting & gathering log integration
- Support for multiple characters

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [XIVAPI](https://xivapi.com/) for providing the Final Fantasy XIV data API
- [Square Enix](https://www.square-enix.com/) for creating Final Fantasy XIV
- This app is not affiliated with or endorsed by Square Enix

## Contact

Project Link: [https://github.com/car723/Final_Project_CS377-Clayton_Ramsey_-_Alexandra_Curry](https://github.com/car723/Final_Project_CS377-Clayton_Ramsey_-_Alexandra_Curry)
