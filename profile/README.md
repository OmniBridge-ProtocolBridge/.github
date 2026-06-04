# Welcome to OmniBridge

OmniBridge is a Universal Adapter targeted for embedded developers. 
It allows interacting with embedded protocols such as GPIO (not a protocol, I know), and will soon be supporting I2C and SPI as a minimum.
OmniBridge is built around an open specification, allowing anyone to implement their own devices (and even define their own protocols!), 
and have it work with existing software.

## What can I use it for?

Since OmniBridge gives such fine-grained control, it's intended for developers to use for testing.
Whether that be Hardware-In-The-Loop Embedded tests, or integration testing, If you can imagine it you can [hopefully] do it!

Since the host software is primarily provided in Python, it integrates easily with testing frameworks such as Pytest as well!

## Which bits can I use?

OmniBridge is comprised of 3 main components.

### Spec

The specification contains XML definitions of data communicated between the Bridge device, and the Host computer.

### Core

OmniBridge's Core contains the main logic for the firmware, as well as the Core Python libraries.

### Modules

OmniBridge "Modules" contain the end-to-end GPIO/SPI/I2C Logic. They have matching C++ (Firmware) and Python (Host Software) components. 
While the Spec may be provided, an open implementation may not exist, so feel free to do it yourself!

## Why have you provided Specs for some Modules, but the Module doesn't exist?

Unfortunately I have finite time and implementing things takes time. 
Part of this project is creating a framework for others build on.
By providing a Spec, I'm hoping that there's enough structure for anyone to come along and create something, 
and minimise the effort it takes to be compatible with other implementations.

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
