# azurite 
## chatgpt 
Azurite is not a command. It is a mineral that is often used as a decorative stone or as a pigment in blue paint. 

However, there is a software tool called Azurite that can be used in conjunction with Microsoft's Azure platform. Azurite is a lightweight emulator for Azure services that allows developers to build and test their applications locally before deploying them to the cloud.

Using Azurite, developers can simulate various Azure services, including Azure Blob Storage, Azure Table Storage, and Azure Queue Storage. This helps to identify and resolve any issues or bugs in the application before it goes live.

To use Azurite, developers need to download and install the emulator on their local machines. Once installed, they can start the emulator and connect their application to the simulated Azure services using the local connection string.

Overall, Azurite simplifies the development and testing process for Azure applications, making it easier for developers to create scalable and reliable cloud-based solutions. 

## tldr 
 
> Azure Storage API compatible server (emulator) in local environment.
> More information: <https://www.npmjs.com/package/azurite>.

- Use an existing [l]ocation as workspace path:

`azurite {{-l|--location}} {{path/to/directory}}`

- Disable access log displayed in console:

`azurite {{-s|--silent}}`

- Enable [d]ebug log by providing a file path as log destination:

`azurite {{-d|--debug}} {{path/to/debug.log}}`

- Customize the listening address of Blob/Queue/Table service:

`azurite {{--blobHost|--queueHost|--tableHost}} {{0.0.0.0}}`

- Customize the listening port of Blob/Queue/Table service:

`azurite {{--blobPort|--queuePort|--tablePort}} {{8888}}`
