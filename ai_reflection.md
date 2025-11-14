# AI Reflection

This project was a fun learning experience. I am confident I would be ablte to explain or modify the project code without assistance -- but I did use AI to learn how to do some of this. Below you'll find some reflections on my AI use.

# How I used AI in this project

For this assignment, I used ChatGPT (and occasionally Google's AI mode) as a **technical reference and learning tool**, similar to using documentation, MDN or StackOverflow. AI helped me with:

- Planning my approach and breaking the task into manageable subtasks
- Exploring different ways to normalize the JSON data
- Asking *"What's wrong with this code?"* when debugging
- Clarifying specific CSS or JavaScript behaviors that I didn't understand

Crucially, I did **not** copy-paste any code into my project. Instead, I used AI answers as a personalized tutorial. I only used code I understood and then wrote myself.

---

## Which parts of the project were influenced by AI

- Calendar layout generation using CSS grids
- Styling of event detail and event creation pages as modals
- Understanding why certain CSS layout behaviors occurred. For example, I could not figure out why the calendar didn't stretch to fill the screen on mobile

In all these cases, I validated the AI suggestions by checking them against MDN or other documentation, testing them and modifying them to integrate with my goals.

## Which parts I wrote myself

All application logic, including

- sorting and normalizing event data,
- event rendering
- month navigation,
- modal open/close behavior,
- pre-filling datetime input when event creation is triggered by clicking on a day,
- input form and displaying the appropriate input fields for different sports,
- all CSS layout structure and styling,
- overflow and responsive behavior and
- final code architecture and naming

was written by me.

## Why I made certain techical decisions

### Using vanilla Javascript

This keeps the project lightweight and easy to evaluate. It demonstrates my ability to work with the core language without relying on functionality provided by frameworks. It's also just more satisfying to work out stuff myself.

### Normalizing incoming data

The provided dataset had inconsistent fields (e. g. missing values) and information I didn't deem relevant for displaying in the app. Normalizing it early created a stable, known structure for me to work with without being surprised down the line.

### Sorting by date immediately after normalization

This ensures events render consistently regardless of event order in the source data.

### Making users pick from a predetermined list of sports

This serves to functions: I can vary the input fields depending on the sport (two teams for team sports, one title for all else), and it ensures user-created data is consistent enough to be used for filtering later (I did, however, not get to this step).

### Not storing user-created events

This would've been the next big thing on my to-do list -- but I believe event storage should be added in tandem with the option to edit (or at least delete) user-created events. I decided I don't have enough time left to add these features in a clean, systematic way.

## One improvement I would make with more time

I would add **local storage with full support for editing and deleting events**. This would include:

- persisting events on page reload
- an *edit* button when viewing event details
- an *edit event* modal with the option to change various event attributes and delete the event altogether
- perhaps the ability to drag and drop events within the calendar to change their date (although I would need to think how to make this work with event times)