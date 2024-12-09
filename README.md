# cs5520_group2

Petsgram is a photo-sharing and social app, designed similarly to Instagram but entirely focused on pets. Users can create profiles for their pets, post images, and interact through likes, direct messages, while discovering new pets from around the world. This app gives pet lovers a platform to make new friends, get new ideas, and even find help with issues they face with their pets.

## Project Structure

The repository is organized as follows:
- **MyApp.xcodeproj**: The Xcode project file for building and managing the app.
- **MyApp.xcworkspace**: The Xcode workspace file used for managing the project with CocoaPods.
- **MyApp/**: The main directory containing the app's source code.
- **Pods/**: Directory containing third-party dependencies managed by CocoaPods.
- **Podfile**: Defines the dependencies used in the project.
- **README.md**: The current documentation for the repository.

## Features

- **Pet Profiles**: Users can create individual profiles for their pets.
- **Photo Sharing**: Post and share images of your pets.
- **Social Interactions**: Interact with other users through likes, comments, and direct messages.
- **Discovery**: Find and follow new pets from around the world.
- **CocoaPods Integration**: Manages dependencies for Firebase, SDWebImage, and more.
- **Firebase**: Provides authentication, database, analytics, crash reporting, and storage features.
- **SDWebImage**: Handles efficient image loading and caching.
- **Appirater**: Prompts users to rate the app based on usage milestones.

## Installation

### Prerequisites
- Xcode installed on your machine.
- CocoaPods installed. If not, install CocoaPods using:
  ```bash
  sudo gem install cocoapods
