# plantuml 
## chatgpt 
PlantUML is a tool used to create UML diagrams through text. It is very popular because of its simplicity and the ability to create diagrams without using complex graphical interfaces. The command "plantuml" refers to the software itself, which should be installed on your computer to use this tool.

When you run the "plantuml" command, it opens the PlantUML Console. From here, you can create different types of UML diagrams using simple text commands. PlantUML supports various types of diagrams like class, activity, use case, sequence, and more.

Here's an example of how to use the PlantUML command to create a class diagram:

```
@startuml
class Car {
  +make: string
  +model: string
  +year: int
  +getMake(): string
  +getModel(): string
  +getYear(): int
}
@enduml
```

When you save this code as a file with the ".uml" extension, you can pass it as an argument to the "plantuml" command. PlantUML will then generate a visual representation of the class diagram in a format of your choice (such as PNG, SVG, or PDF).

In summary, the "plantuml" command is a tool used to create UML diagrams from simple text commands. It is a popular and straightforward tool that is widely used in the software development industry. 

## tldr 
 
> Create UML diagrams from a plain text language and render them in different formats.
> More information: <https://plantuml.com/en/command-line>.

- Render diagrams to default format (PNG):

`plantuml {{diagram1.puml}} {{diagram2.puml}}`

- Render a diagram in given format (e.g. `png`, `pdf`, `svg`, `txt`):

`plantuml -t {{format}} {{diagram.puml}}`

- Render all diagrams of a directory:

`plantuml {{path/to/diagrams}}`

- Render a diagram to the output directory:

`plantuml -o {{path/to/output}} {{diagram.puml}}`

- Render a diagram with the configuration file:

`plantuml -config {{config.cfg}} {{diagram.puml}}`

- Display help:

`plantuml -help`
