# circup 
## chatgpt 
As an AI language model, I don't have the full context of where 'circup' command is used. However, here is some explanation about it. 

CircUp is a Python package used for managing and updating CircuitPython libraries on devices. To run the 'circup' command, first, you need to install CircUp via pip by running the command:

```
pip install circup
```

Once installed, CircUp helps you to install, update or remove the CircuitPython libraries on your device. Here are some examples of what you can do with the 'circup' command:

- To install a library, run:

  ```
  circup install adafruit_bus_device
  ```

- To update all installed libraries, run:

  ```
  circup update
  ```

- To remove a library, run:

  ```
  circup remove adafruit_bus_device
  ```

CircUp also has other options such as checking the installed library version, modifying CircuitPython bundle files, etc. You can check the CircUp documentation for the full list of commands and options. 

## tldr 
 
> The CircuitPython library updater.
> More information: <https://github.com/adafruit/circup>.

- Interactively update modules on a device:

`circup update`

- Install a new library:

`circup install {{library_name}}`

- Search for a library:

`circup show {{partial_name}}`

- List all libraries on a connected device in `requirements.txt` format:

`circup freeze`

- Save all libraries on a connected device in the current directory:

`circup freeze -r`
