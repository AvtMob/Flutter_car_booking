# Flutter Cars

A simple Car Rental application using [Flutter](https://flutter.dev/) and the [CarTrawler](https://www.cartrawler.com) API. This project/app was built as a means to learn Dart & Flutter. I have no intention of releasing.

![alt text](https://simondarcyonline.com/cartrawler/flutter-cars-screens.png "Screenshot of app")

You can watch a demo video [here](https://www.youtube.com/watch?v=_8MyyqRhc1g)

## Getting Started

This app is built using Flutter, Google's open-source UI SDK. If you are not familiar with Dart/Flutter, here are a few resources to get you started:

- [Official documentation](https://flutter.dev/docs) 
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

### Prerequisites 

This project requires 2 keys: 

1. A CarTrawler Client ID. Required to communicate with [CarTrawler's API](https://docs.cartrawler.com/docs/xml/overview.html). 
2. A Google Maps API key. Needed for location autocomplete and map widget. Follow [these](https://developers.google.com/places/web-service/get-api-key) steps to acquire one.

Once you have these 2 keys. Add them to `"lib/settings_example.dart"` and rename this file to simply `"settings.dart"`.

Note: The CarTrawler API comes with a locations endpoint. A !todo is to use this instead than Google for the location autocomplete.   

### Dependencies  

Once your keys are ready, run `Pub get` to add the following dependencies:

- http: Used to communicate with APIs.
- flutter_google_places: Used for locations autocomplete.
- google_maps_webservice:  Used for locations autocomplete.
- google_maps_flutter: Used for map widget.
- intl: Used for localisation (dates mostly).
- webview_flutter: Used to load e-voucher.
- sqflite: Used to store booked cars.
- path_provider: Used to create DB.
- cached_network_image: Used to cache and lazy load images.
- progress_dialog: Used to show progress modal when making booking.

## App screens / Flow

- Home screen/search screen: Form to allow users to input their search criteria.
- Search Results screen: Displays cars at selected location/dates/times.
- Car details screen: Show full details of the selected car.
- Driver details screen: Form to allow users to input their details (Name, email and phone).
- Confirmation screen: Show details of booked car.
- Voucher screen: Load webview containing e-voucher. 
- My bookings screen: Show cars booked through app.
- Terms screen: Show car/supplier terms & conditions.
