# calcurse 
## chatgpt 
Calcurse is a command-line calendar and scheduling application that can help you keep track of your daily tasks, appointments, and meetings. It allows you to manage your schedule and set reminders for important events. Here are some of the tasks you can perform with Calcurse:

1. View your schedule using the built-in calendar: You can view your daily, weekly, or monthly schedule using the built-in calendar. This allows you to see what tasks and events are coming up and plan accordingly.

2. Add new appointments and events: You can add new appointments or events to your calendar using the "a" command. You can specify the date, time, and description of the appointment or event.

3. Set reminders: You can set reminders for upcoming appointments or events using the "r" command. This will notify you of the event at a specified time before it starts.

4. Manage to-do lists: You can create and manage to-do lists using the "t" command. This allows you to keep track of tasks you need to complete and mark them as done when finished.

5. Export and import data: You can export and import your calendar data using the "e" and "i" commands. This allows you to move your data between computers or backup your data.

Overall, Calcurse is a versatile tool that can help you stay organized and manage your time effectively. It is a free, open-source application that is available for Linux, BSD, and macOS. 

## tldr 
 
> A text-based calendar and scheduling application for the command-line.
> More information: <https://calcurse.org>.

- Start calcurse on interactive mode:

`calcurse`

- Print the appointments and events for the current day and exit:

`calcurse --appointment`

- Remove all local calcurse items and import remote objects:

`calcurse-caldav --init=keep-remote`

- Remove all remote objects and push local calcurse items:

`calcurse-caldav --init=keep-local`

- Copy local objects to the CalDAV server and vice versa:

`calcurse-caldav --init=two-way`
