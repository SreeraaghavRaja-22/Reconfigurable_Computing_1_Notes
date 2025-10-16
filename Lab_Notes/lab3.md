# Lab 3 notes

## Part 1

- **wrapper:** *Top-level entity* for the entire project
  - Entity that will be instantiated from within the AXI peripheral code
  - Instantiates the *user_app* entity
- **user_app:** a simple, *memory-map* interface that is much more modular / portable than the *AXI interface*
- **config_pkg.vhd:** contains constants and types that are used for configuring the virtual board interface
- **user_pkg.vhd:** provides contraints used throughout the application
  - similar to a *Header File* in C
- **user_app_tb.vhd:** shows how to send inputs and read outputs to/from the memory map
- **memory_map.vhd:** implements the memory map entity that enables application-specific communication with FPGA resources
