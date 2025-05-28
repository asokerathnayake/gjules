# Real-Time Themed Clock

This project is a simple, single-page web application that displays the current date and time, with a background theme that automatically adjusts based on whether it's day or night. It can also display local sunrise and sunset times if location access is granted.

## Features

- **Real-Time Clock**: Displays the current date and time, updating every second.
- **Automatic Day/Night Theme**:
    - Switches to a light theme during the day and a dark theme during the night.
    - If browser geolocation is permitted and sunrise/sunset times are successfully fetched, these times are used to determine day/night for more accuracy.
    - Falls back to a 6:00 AM / 6:00 PM schedule if geolocation is denied, fails, or if sunrise/sunset data cannot be retrieved.
- **Sunrise and Sunset Times**:
    - If the user grants location permission, the application will attempt to fetch and display the local sunrise and sunset times using the `api.sunrise-sunset.org` service.
    - Displays user-friendly messages if location access is denied or if data fetching fails.
- **Pure HTML/CSS/JavaScript**: No external libraries or frameworks are used for the core functionality.

## How to Use

1.  Clone or download the repository.
2.  Open the `index.html` file in a modern web browser.
3.  The browser may ask for permission to access your location.
    - **Allowing** will enable the display of sunrise/sunset times and theme changes based on them.
    - **Denying** will cause the application to use a fixed 6 AM/6 PM schedule for theme changes, and sunrise/sunset times will not be displayed.
