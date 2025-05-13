# task_reuseall 
# Rider Route & Navigation App (Flutter)

A Flutter-based screen designed for delivery riders to easily visualize their pickup route, navigate through each stop, and reach the final warehouse location.

---

## Overview

This app screen allows riders to:
- View their *current location* on a map.
- See *pickup points* and a *warehouse location* via markers.
- Follow a *complete route* connecting all pickups and ending at the warehouse.
- Use a *"Navigate"* button to:
  - Open the route in Map, or
  - Trigger *in-app navigation*.

---

## Features

- Display Map with:
  - *Markers* for all pickup locations
  - *Marker* for the warehouse
- Route drawing using polyline:
  - From current location
  - Through all pickup points (in given order)
  - Ending at the warehouse
- 'Navigate' button functionality:
  - Opens *Maps* with route using url_launcher
  - Supports *in-app navigation*
- Show *distance/time to warehouse*

---

### Prerequisites
- Install Flutter
- Install VS Code or Android Studio
- Enable Developer Mode on your physical device if using wireless debugging

### Clone the Repository
- bash
  git clone https://github.com/shubhnesh/Task-Pragati.git

### Install Dependencies
- bash
  pub get

### Run the App
- bash
  flutter run

### Check if the device is recognized:
- bash
  flutter devices

---

## Sample Data

```dart
final pickups = [
  {
    "id": 1,
    "location": LatLng(12.971598, 77.594566),
    "time_slot": "9AM-10AM",
    "inventory": 5,
  },
  {
    "id": 2,
    "location": LatLng(12.972819, 77.595212),
    "time_slot": "9AM-10AM",
    "inventory": 3,
  },
  {
    "id": 3,
    "location": LatLng(12.963842, 77.609043),
    "time_slot": "10AM-11AM",
    "inventory": 7,
  },
];

final warehouseLocation = LatLng(12.961115, 77.600000);
