# gcalcli 
## chatgpt 
gcalcli is a command line interface (CLI) application that allows you to access and manage your Google Calendar from your terminal or command prompt. It can be used to view your calendar events, create new events, edit existing events, delete events, and perform other calendar-related tasks. 

Some of the features of gcalcli include:

- The ability to show your calendar in various formats including month, week, and agenda view.
- The ability to search for events and filter them based on various criteria.
- The ability to create new events with options such as title, start time, end time, location, and description.
- The ability to edit existing events, including changing their start or end times, location, or description.
- The ability to delete events.
- The ability to import or export events to or from other calendar applications.

gcalcli can be a useful tool for anyone who wants to manage their Google Calendar using the command line interface. It is particularly useful for users who prefer to use the terminal or command prompt for tasks like scheduling appointments or setting reminders. 

## tldr 
 
> Command-line tool to interact with Google Calendar.
> Requests Google API authorization upon first launch.
> More information: <https://github.com/insanum/gcalcli>.

- List your events for all your calendars over the next 7 days:

`gcalcli agenda`

- Show events starting from or between specific dates (also takes relative dates e.g. "tomorrow"):

`gcalcli agenda {{mm/dd}} [{{mm/dd}}]`

- List events from a specific calendar:

`gcalcli --calendar {{calendar_name}} agenda`

- Display an ASCII calendar of events by week:

`gcalcli calw`

- Display an ASCII calendar of events for a month:

`gcalcli calm`

- Quick-add an event to your calendar:

`gcalcli --calendar {{calendar_name}} quick "{{mm/dd}} {{HH:MM}} {{event_name}}"`

- Add an event to calendar. Triggers interactive prompt:

`gcalcli --calendar "{{calendar_name}}" add`
