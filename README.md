#Enclustra Build Environment

Enclustra Build Environment is a tool which allows the user to quickly setup and run all of the Enclustra Zynq and Altera Soc boards.
It allows the user to choose the desired target, and downloads all the required binaries like the bitstream and fsbl. It downloads and compiles software such as U-Boot, Linux, and BusyBox based root file system. 

To run the build script a Python interpreter is required. The system is compatible both with Python 2 and Python 3.

Running the build.py script without any arguments starts the Build Environment in GUI mode. At this stage the user is prompted to select the family of the processor, the module model, the base board model, the boot mode and software for later use.

For automating the build process, command line interface is available.

The following arguments are supported:

    usage: tool [-h] [-L] [--list-devices-raw] [-d device] [-l]
                [--list-targets-raw] [-x target] [-f target] [-b target]
                [--custom-build target steps] [--fetch-history target]
                [--list-dev-options] [-o index] [-c] [-v]

    Enclustra Build Environment

    optional arguments:
      -h, --help                    show this help message and exit
      -L, --list-devices            list all available devices
      --list-devices-raw            list all available devices in a script
                                    friendly way
      -d device, --device device    specify device as follows:
                                    <family>/<module>/<base_board>/<boot_device>
      -l, --list-targets            list all targets for chosen device
      --list-targets-raw            list all targets for chosen device in a script
                                    friendly way
      -x target                     fetch and build specific target
      -f target, --fetch target     fetch specific target
      -b target, --build target     build specific target
      --custom-build target steps   build specific target with specific steps
                                    (comma separated)
      --fetch-history target        fetch specific target with history
      --list-dev-options            list all available device options for chosen
                                    device
      -o index, --dev-option index  set device option by index, the default one
                                    will be used if not specified
      -c, --clean-all               delete all downloaded code, binaries, tools
                                    and built files
      -v, --version                 print version


Please refer to the user documentation located inside this repository for more information about the usage of the build system.

Copyright (c) 2015, Enclustra GmbH, Switzerland
