# Event Calendar – Coding Task Submission

An interactive calendar for sports events, built as part of an application. Displays a set of events in a monthly calendar view, allows users to view event details, and create their own events.

The project is fully client-side and built with **HTML, CSS and JavaScript**.

---

## Live Demo

View the deployed version here:
**https://jonathanthul-sr-event-calendar.statichost.eu/**

---

## Tech Stack

- **HTML** for structure
- **CSS** for layout and styling, using grids and flexboxes for the calendar
- **Vanilla JavaScript** for all functionality - no frameworks!
- **Static hosting** via statichost.eu

---

## How to Run the Project Locally

Because of cross-origin restrictions in modern browsers, the project has to be served through a local web server.

1. Clone the repository:
    ```console
    git clone https://github.com/jonathanthul/sr-event-calendar.git
    ```
2. Navigate into the project folder:
    ```console
    cd sr-event-calendar
    ```
3. Run a local server (example using Python):
    ```console
    python -m http.server
    ````
4. Open http://localhost:8000/ in your browser of choice.

## Design Decisions

The application is intentionally framework-free to emphasize clear JavaScript logic.

Events provided by the JSON dataset are normalized into a unified structure to simplify rendering. 

The calendar is rendered via JavaScript so new months and user-created events integrate seamlessly.

## Current Limitations
- Within any day, user-created events are rendered in order of creation, not in chronological order
- User events reset on page reload

## Planned Improvements

If I had more time, I would add:

- Local storage for persistence of user-created events
- Edit & Delete functionality
- Filtering by sport
- Automatic winner highlighting for matches with known results
- Notifications for upcoming events
- Dark mode
- Smoother mobile-specific modal layout