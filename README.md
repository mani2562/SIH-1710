# Smart India Hackathon Workshop

**Date:** 26/10/2026

**Register Number:** 212225040224

**Name:** Manikandan G

## Problem Title

**SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations**

## 1. Idea

The idea is to develop a **Smart Railway Station Navigation System** that helps passengers easily find platforms, ticket counters, restrooms, food courts, waiting halls, enquiry counters, lifts, escalators, and other facilities inside railway stations.

The system will provide interactive 2D/3D maps, step-by-step directions, voice-guided navigation, and accessibility options for elderly passengers and people with disabilities. Passengers can use a mobile application or digital kiosks installed at railway stations to find the shortest and most convenient route to their destination.

The system will also provide information about platform changes and facility locations through regular updates. The main objective is to reduce passenger confusion, save time, improve accessibility, and make railway station navigation simple and efficient.

## 2. Proposed Solution / Architecture Diagram

### Proposed Solution

The proposed solution is a multi-platform navigation system that combines digital maps, GPS where available, indoor positioning, and route-finding algorithms to guide passengers inside railway stations.

The application will allow passengers to select their current location and desired destination. The system will calculate a suitable route and display step-by-step directions on an interactive map.

### Key Features

* **Interactive Maps:** Display station layouts, platforms, ticket counters, restrooms, food courts, waiting halls, and other facilities.
* **Smart Route Finding:** Calculate suitable routes using a pathfinding algorithm such as Dijkstra's algorithm or A*.
* **Indoor Navigation:** Use QR codes, Bluetooth beacons, or other indoor positioning methods to identify a passenger's approximate location.
* **Voice-Guided Navigation:** Provide spoken directions for visually impaired passengers.
* **Accessibility Support:** Offer wheelchair-friendly routes that avoid stairs and prioritize ramps and lifts.
* **Real-Time Updates:** Display verified updates about platform changes, closed passages, and relocated facilities.
* **Digital Kiosks:** Provide touch-screen navigation for passengers who do not have smartphones.
* **Multilingual Support:** Offer directions in English, Tamil, Hindi, and other supported languages.
* **Search Facility:** Allow passengers to search for destinations such as platforms, ticket counters, and restrooms.

### Architecture Diagram
![Uploading image.png…]()

### Working Process

1. The passenger opens the mobile application or uses a digital kiosk.
2. The passenger selects a destination, such as Platform 3 or the ticket counter.
3. The system identifies the passenger's approximate location using available indoor positioning methods or a manually selected location.
4. The navigation engine calculates a suitable route using the station map.
5. The application displays the route and provides step-by-step directions.
6. Voice instructions are provided when enabled, and accessible routes are prioritized according to passenger requirements.
7. The system uses verified updates to adjust routes when a passage is closed or a destination changes location.

## 3. Use Cases

### Use Case 1: Finding Railway Platforms

Passengers can search for their platform number and receive directions from the station entrance or their current location.

**Benefit:** Reduces confusion and helps passengers reach their platforms on time.

### Use Case 2: Locating Station Facilities

Passengers can find ticket counters, enquiry desks, restrooms, drinking water, food courts, waiting halls, and other facilities.

**Benefit:** Saves time and improves the passenger experience.

### Use Case 3: Navigation for Visually Impaired Passengers

The application provides voice-guided directions and spoken information about nearby facilities and navigation instructions.

**Benefit:** Improves accessibility and helps visually impaired passengers navigate the station more independently.

### Use Case 4: Wheelchair-Friendly Navigation

The system identifies accessible routes that prioritize ramps, lifts, and step-free passages.

**Benefit:** Helps wheelchair users and passengers with mobility difficulties travel more conveniently.

### Use Case 5: Digital Kiosk Navigation

Passengers can select their destination using a touch-screen kiosk and view directions on a station map.

**Benefit:** Supports passengers who do not have smartphones or internet access.

### Use Case 6: Real-Time Platform and Route Updates

When authorized railway staff update platform assignments or report a closed passage, the system can display the latest verified information and recalculate affected routes.

**Benefit:** Helps passengers respond to changes and avoid unavailable routes.

### Use Case 7: Multilingual Navigation

Passengers can select their preferred supported language to receive directions and facility information.

**Benefit:** Makes the system easier to use for passengers from different regions.

### Use Case 8: Emergency and Accessible Exit Navigation

The system can display verified emergency exits and accessible evacuation routes based on authorized station safety information.

**Benefit:** Helps passengers identify appropriate exits and supports safer movement during emergencies.

## 4. Technology Stack

The following technologies can be used to develop the proposed system.

| Component            | Suggested Technology                           | Purpose                                                            |
| -------------------- | ---------------------------------------------- | ------------------------------------------------------------------ |
| Frontend             | React.js                                       | Develop the web interface and digital kiosk application            |
| Mobile Application   | React Native or Flutter                        | Build the passenger navigation app                                 |
| UI Design            | HTML, CSS, JavaScript                          | Create an interactive and user-friendly interface                  |
| Interactive Maps     | Leaflet.js or Mapbox                           | Display station maps and navigation routes                         |
| 3D Maps              | Three.js                                       | Display interactive 3D station layouts                             |
| Backend              | Python with FastAPI or Node.js with Express    | Handle requests and navigation services                            |
| Database             | PostgreSQL with PostGIS                        | Store station locations, maps, facilities, and spatial information |
| Navigation Algorithm | Dijkstra's algorithm or A*                     | Calculate suitable routes between locations                        |
| Indoor Positioning   | QR codes or Bluetooth Low Energy (BLE) beacons | Estimate the passenger's location inside the station               |
| Voice Navigation     | Web Speech API or a text-to-speech service     | Convert navigation instructions into speech                        |
| Real-Time Updates    | WebSockets or REST APIs                        | Deliver verified station and route updates                         |
| Authentication       | Role-based access control                      | Restrict station map and update management to authorized staff     |
| Cloud Hosting        | AWS, Microsoft Azure, or Google Cloud          | Host the application and backend services                          |
| Version Control      | Git and GitHub                                 | Manage source code and team collaboration                          |

**Recommended prototype stack:** React.js, Python FastAPI, PostgreSQL, Leaflet.js, and QR-code-based indoor location identification. These technologies can support an initial demonstration without requiring expensive indoor positioning hardware.

## 5. Dependencies

The system requires the following software, data, infrastructure, and services.

### A. Software Dependencies

* Node.js and npm for installing and running the frontend.
* React.js for building the user interface.
* Python and FastAPI for developing backend APIs.
* PostgreSQL with PostGIS for storing station and spatial data.
* Leaflet.js or another mapping library for displaying maps.
* A compatible QR-code scanning library for identifying marked station locations.
* A text-to-speech service or browser speech API for voice instructions.
* Git and GitHub for version control and team collaboration.

### B. Data Dependencies

* Accurate railway station floor plans and layouts.
* Platform numbers and locations.
* Locations of ticket counters, restrooms, lifts, escalators, food courts, and waiting areas.
* Information about accessible paths, ramps, and step-free entrances.
* Verified platform assignments and station announcements, where available through authorized sources.
* Information about closed passages and relocated facilities.
* Multilingual facility names and navigation instructions.

### C. Hardware Dependencies

* A smartphone, tablet, laptop, or desktop computer for development and testing.
* A touchscreen display or kiosk device for the kiosk prototype.
* QR-code labels placed at selected station locations for the prototype.
* Internet or local network connectivity, depending on deployment.
* Optional Bluetooth beacons or other indoor positioning equipment for more advanced navigation.
* A microphone or speaker where voice input or audio output is required.

### D. API and Service Dependencies

* Mapping libraries or services.
* Text-to-speech services, if the browser's built-in speech features are insufficient.
* Railway information APIs, if officially available and authorized.
* Cloud hosting and database services for deployment.
* Authentication and authorization services for staff who maintain station information.

### E. Operational Dependencies

* Permission to access and use railway station maps and facility information.
* Coordination with railway authorities to verify station layouts and platform data.
* Authorized staff or an approved process to update facility locations and report closures.
* Regular checks to ensure route information remains accurate.
* Privacy and security measures to protect passenger information.
* Accessibility testing with users who have different mobility, vision, and language needs.


