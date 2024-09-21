# OpenJBOD

OpenJBOD is a project that aims to make it easier to build disk shelves or "Just a Bunch Of Disks" units.

Traditionally, JBODs are sold as part of Enterprise storage systems and are made up of relatively few components:
- A case
- Power supplies
- A control plane for managing the power status
- One (or more) SAS expanders.

These components all work together to allow the JBOD to host a number of disks while allowing only a server connected via the SAS expander (often referred to as a head unit) to access and manage the disks themselves.

Have an idea for a project? Wanna talk about how to use these components or share new ideas? Check out our [discussions!](https://github.com/orgs/OpenJBOD/discussions)

## OpenJBOD Projects

OpenJBOD aims to make it easier to build JBODs out of commodity hardware by providing some of the more niche or rare to come by components.

### OpenJBOD RP2040

The [OpenJBOD RP2040](https://github.com/OpenJBOD/rp2040) is an open source control plane that allows users to remotely control a JBOD chassis, its features include:

- Network management over ethernet
- ATX power supply control
- PCI-e slot for a standalone SAS expander
- Fan controller with five fan headers
- On-board temperature probe for accurate fan curve responses
- Option for an external temperature probe for more accurate readings near disks

### OpenJBOD Software

The [OpenJBOD Software](https://github.com/OpenJBOD/software) is a MicroPython-based software package that provides the network-based management of the OpenJBOD RP2040 board. Its features includes:

- Configurable networking (DHCP or Static IP assignment)
- BASIC authentication with unique users
- Customizable power-on behavior (Power up immediately, follow USB port power)
- Customizable fan curve
- Free-form notes
