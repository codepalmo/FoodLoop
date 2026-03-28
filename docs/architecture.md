# FoodLoop Architectural Guidelines

The FoodLoop mobile platform follows a layered architectural pattern to ensure modularity and scalability. The system is divided into four primary structural layers:

## 1. Presentation Layer
- **Technology**: `Flutter`, `Material 3`
- **Responsibility**: Manages the graphical interface and user interactions.
- **Components**: Interactive map viewport, Giver/Taker dashboards, and NGO interface.

## 2. Application Layer
- **Technology**: `Dart`, `Google Maps SDK`
- **Responsibility**: Core processing logic and community engagement.
- **Components**:
    - **Discovery Engine**: Filters food items within a 5km radius.
    - **Verification**: Generates secure claim tokens for handover.

## 3. Data Layer
- **Technology**: `Cloud Firestore`, `Firebase Storage`, `Firebase Auth`
- **Responsibility**: Persistent storage and secure retrieval of data.
- **Components**:
    - `Users` Collection: Tracks reputation and account types.
    - `Postings` Collection: Tracks location and expiry timestamps.

## 4. Hardware Interface Layer
- **Technology**: `Google Location Services` (Android) / `CoreLocation` (iOS)
- **Responsibility**: Bridges physical device sensors with the software.
