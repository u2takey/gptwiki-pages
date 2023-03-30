# amass viz 
## chatgpt 
The "amass viz" command is a feature provided by the "Amass" tool, which is an open-source network mapping and reconnaissance tool. It is designed for discovering exposed targets on the internet and collecting information about them. 

The "amass viz" command is specifically used to visualize the data collected by the Amass tool. It generates an HTML file with an interactive visual representation of the data. This HTML file can be viewed in a web browser and allows the user to explore and interact with the data in various ways, such as zooming in/out, panning, and filtering. 

The visualization includes different types of nodes and edges representing IPs, domains, subdomains, and connections between them. The nodes are color-coded based on importance and various other parameters such as the number of links to other nodes, website traffic, and the presence of web technologies.

In summary, the "amass viz" command serves as a powerful and useful visualization tool for understanding complex network data collected by the Amass tool. It provides a rich visual interface that makes it easy to explore and analyze the data in a user-friendly manner. 

## tldr 
 
> Visualize gathered information in a network graph.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-viz-subcommand>.

- Generate a D3.js visualization based on database data:

`amass viz -d3 -dir {{path/to/database_directory}}`

- Generate a DOT file based on database data:

`amass viz -dot -dir {{path/to/database_directory}}`

- Generate a Gephi Graph Exchange XML Format (GEXF) file based on database data:

`amass viz -gexf -dir {{path/to/database_directory}}`

- Generate a Graphistry JSON file based on database data:

`amass viz -graphistry -dir {{path/to/database_directory}}`

- Generate a Maltego CSV file based on database data:

`amass viz -maltego -dir {{path/to/database_directory}}`
