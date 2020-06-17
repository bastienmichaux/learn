# Computers

## Computer components

Major hardware components of a computer system:
- Processor
- Main memory
- Secondary memory
- Input devices
- Output devices

Most components are connected to the main circuit board of the computer, the motherboard.

The power supply supplies power for most of the components.

Input/output devices are attached through connectors. Input and output devices allow the computer system to interact with the outside world by moving data into and out of the system.

A bus is a group of wires on the main circuit board of the computer. It is a pathway for data flowing between components.

Most devices are connected to the bus through a controller which coordinates the activities of the device with the bus.

A network interface acts as both input and output. Data flows from the network into the computer, and out of the computer into the network.

### Processor

The processor does the fundamental computing within the system, and directly or indirectly controls all the other components.

The processor is sometimes called the Central Processing Unit or CPU. A particular computer will have a particular type of processor, such as a Pentium processor or a SPARC processor.

The processor performs all the fundamental computation of the computer system. Other components contribute to the computation by doing such things as storing data or moving data into and out of the processor. But the processor is where the fundamental action takes place.

A processor chip has relatively little memory. It has only enough memory to hold a few instructions of a program and the data they process. Complete programs and data sets are held in memory external to the processor. This memory is of two fundamental types: main memory, and secondary memory.

### Memory

Main memory is sometimes called volatile because it looses its information when power is removed.

Secondary memory is usually nonvolatile because it retains its information when power is removed. (However, it needs power when information is stored into memory or retrieved from it.)

Main memory is sometimes called main storage and secondary memory is sometimes called secondary storage or mass storage.

Main memory:
- closely connected to the processor.
- stored data are quickly and easily changed.
- holds the programs and data that the processor is actively working with.
- interacts with the processor millions of times per second.
- needs constant electric power to keep its information.

Secondary memory:
- connected to main memory through the bus and a controller.
- stored data are easily changed, but changes are slow compared to main memory.
- used for long-term storage of programs and data.
- before data and programs can be used, they must be copied from secondary memory into main memory.
- does not need electric power to keep its information.

### Main memory

Main memory is where programs and data are kept when the processor is actively using them. When programs and data become active, they are copied from secondary memory into main memory where the processor can interact with them. A copy remains in secondary memory.

Main memory is intimately connected to the processor, so moving instructions and data into and out of the processor is very fast.

Main memory is sometimes called RAM. RAM stands for Random Access Memory. "Random" means that the memory cells can be accessed in any order. However, properly speaking, "RAM" means the type of silicon chip used to implement main memory.

When people say that a computer has "512 megabytes of RAM" they are talking about how big its main memory is. One megabyte of memory is enough to hold approximately one million (106) characters of a word processing document. (There will be more about bytes and megabytes later on in these notes.)

Nothing permanent is kept in main memory. Sometimes data are placed in main memory for just a few seconds, only as long as they are needed.

### Secondary memory

Secondary memory is where programs and data are kept on a long-term basis. Common secondary storage devices are the hard disk and optical disks.

The hard disk has enormous storage capacity compared to main memory.
The hard disk is usually contained inside the case of a computer.
The hard disk is used for long-term storage of programs and data.
Data and programs on the hard disk are organized into files.
A file is a collection of data on the disk that has a name.
A hard disk might have a storage capacity of 500 gigabytes (room for about 500 x 109 characters). This is about 100 times the capacity of main memory. A hard disk is slow compared to main memory. If the disk were the only type of memory the computer system would slow down to a crawl. The reason for having two types of storage is this difference in speed and capacity.

Large blocks of data are copied from disk into main memory. The operation is slow, but lots of data is copied. Then the processor can quickly read and write small sections of that data in main memory. When it is done, a large block of data is written to disk.

Often, while the processor is computing with one block of data in main memory, the next block of data from disk is read into another section of main memory and made ready for the processor. One of the jobs of an operating system is to manage main storage and disks this way.

### I/O

Input/output devices are usually called I/O devices. They are directly connected to an electronic module attached to the motherboard called a device controller. For example, the speakers of a multimedia computer system are directly connected to a device controller called an audio card, which in turn is plugged into a bus on the motherboard.

With many recent computers, the functions of a device controller are integerated with the motherboard. Some motherboards have audio, graphics, and network controllers built in.

Sometimes secondary memory devices like the hard disk are called I/O devices (because they move data in and out of main memory). What counts as an I/O device depends on context. To a user, an I/O device is something outside of the computer case. To a programmer, anything outside of the processor and main memory is an I/O device. To an engineer working on the design of a processor everything outside of the processor is an I/O device.

### Embedded systems

An embedded system is a computer system that is part of a larger machine and which controls how that machine operates.

Usually the processor constantly runs a single control program which is permanently kept in ROM (Read Only Memory).

ROM is used to make a section of main memory read-only. Main memory looks the same as before to the processor, except a section of it permanently contains the program the processor is running. This section of memory retains its data even when power is off.

Cell phones, cars (e.g. airbags) have embedded systems. Digital cameras, DVD players, medical equipment, and even home appliances contain dedicated processors.

Most processor chips are used in embedded systems. Less than 1% of processor chips are used for desktop computers.

### Types of Programs

There are two categories of programs. Application programs (usually called just "applications") are programs that people use to get their work done. Computers exist because people want to run these programs. Systems programs keep the hardware and software running together smoothly. The difference between "application program" and "system program" is fuzzy. Often it is more a matter of marketing than of logic.

The most important systems program is the operating system. The operating system is always present when a computer is running. It coordinates the operation of the other hardware and software components of the computer system. The operating system is responsible for starting up application programs, running them, and managing the resources that they need. When an application program is running, the operating system manages the details of the hardware for it. For example, when you type characters on the keyboard, the operating system determines which application program they are intended for and does the work of getting them there.

Some embedded systems do not use an operating system, but run their programs directly on the processor.

Modern operating systems for desktop computers come with a user interface that enables users to easily interact with application programs (and with the operating system itself) by using windows, buttons, menus, icons, the mouse, and the keyboard. Examples of operating systems are Unix, Linux, Android, Mac OS, and Windows.

### Operating Systems

An operating system is a complex program that keeps the hardware and software components of a computer system coordinated and functioning. It is like the owner of a small shop, who keeps everything in order by attending to customers, accepting deliveries, stocking the shelves, doing the bookkeeping, and so on. The shopkeeper must promptly attend to tasks as they arise. Without the shopkeeper the shop could not function.

Most computer systems can potentially run any of several operating systems. For example, most Pentium-based computers can run either Linux or a Windows operating systems. Usually only one operating system is installed on a computer system, although some computers have several. In any case, only one operating system at a time can be in control of the computer system. The computer user makes a choice when the computer is turned on, and that operating system remains in control until the computer is turned off.

### Starting a Program

When a computer is first started, the hardware automatically loads the operating system and starts it running. This process is called booting. The reason for this odd term is that the operating system is itself involved in getting itself running—a process that is like someone "pulling themselves up by their bootstraps". Once the operating system is running, it is used to start up application programs.

Here is a (simplified) list of what happens when the user (you) starts up an application. Assume that the operating system (OS) is already running.

The user asks to run an application.
This is done by clicking on an icon, making a menu choice, or by other means.
The OS determines the name of the application.
The OS finds the files on the hard disk where the application and its data are stored.
The OS finds an unused section of main memory that is large enough for the application.
The OS makes a copy of the application and its data in that section of main memory.
The software on the hard disk is unchanged; main memory holds a copy of what is on disk.
The OS sets up resources for the application.
Finally, the OS starts the application running.
As the application runs, the OS is there in the background managing resources, doing input and output for the application, and keeping everything else running.

### Networks
A computer network consists of two or more computers connected so that they can exchange data and programs. When a computer is a member of a network, the programs it runs and the data it uses can be on the hard disk of some other computer on the network. In business and industrial settings, most computers are on a network. The operating system that runs on a networked computer must manage its share of the network (along with managing all its other responsibilities). The operating system is able to find programs and data that are stored on other network computers, and copy them into its own main memory.

In a local-area network only a few dozen computers are connected together, usually all located within the same building. Each computer has a network address that the other computers use to access it. Usually the computers share a printer. There may be an especially powerful computer called a server whose hard disk holds application programs and data that the other computers are expected to need.

Each computer in a network has a network interface card. This is an input/output device that sends and receives data over cables. The network interface cards of computers on a network are connected together with cables.

### Wide-Area Networks
Large organizations need to connect many more computers than can be handled with a local area network. A wide-area network can connect thousands of computers together over great distances. The long distance connections are made by using optical fiber, telephone lines, microwave radio, and satellite communications. Each computer in the network has a network address (as with local-area networks) to uniquely identify it.

Wide-area networks use a variety of special hardware to manage the flow of data. When two computers share data, this hardware makes it appear that the two computers are connected together directly. In reality, there may be dozens of network devices between the two computers.

All these devices use the same method for dealing with data. Without a common method of dealing with data, a large network would become a hopeless muddle. An agreement about how to represent and transmit data over a network is called a protocol. Usually large networks use a protocol called TCP/IP (for transmission control protocol / internet protocol).

### Internet
The Internet consists of many networks that have been connected together to form one huge worldwide network. Even on this huge network, each computer must have a unique network address, called an IP address, much like each telephone in the world has a unique telephone number (including the country code and area code).

Typical IP address: `149.152.21.203`

IP addresses actually are 32-bit binary numbers. Networking equipment uses these addresses to route information over the network. The above example shows the standard way of writing these bits using decimal digits.

But even when written in decimal the address is not clear to humans. One of the features of the World Wide Web is that it allows humans to use computer names rather than numbers. Here is a typical computer name:

`chortle.ccsu.edu`

This computer name corresponds to the above IP address. When you use it in a Web browser it is converted into the 32 binary digits of the computer's IP address.

As an experiment, enter the above IP address into the address field of your browser and hit return. Now do the same with the computer name. You will get to the same web page with each.

### World Wide Web

Remember that important idea (discussed several pages back):

Fundamental Idea: Both programs and data are saved in computer memory in the same way. The electronics of computer memory (both main memory and secondary memory) make no distinction between programs and data.

Picture of a package with a mailing label
Communications equipment makes no distinction between programs and data, either. It is all information as far as it is concerned, and all information is transmitted the same way. The Internet is like a worldwide package delivery service. It is concerned with moving packages from one address to another, without concern about what is in the packages.

The Internet provides the hardware and the information transmission protocols for the World-Wide Web. Data intended for the Web is transmitted over the Internet just like any data. What makes Web data special is that it is intended for Web browsers (such as the one you are probably looking at). A browser is a program that can read Web pages and display them in a nicely formatted way.

A Web page is a package of data that contains information on how it is to be displayed on a monitor. This information is given using a language called Hypertext Markup Language (HTML). If you want to see the HTML that describes this page, look at the menu at the top of your Web browser, and select Tools/Web Developer/Page Source. For older browsers, select View in the menu then left-click on Source. This will bring up a new window with the HTML of this page in it. After you are done viewing, close the window by clicking on the close button in its upper right corner (the button marked with X).

## Hyperlinks

Hyperlinks connect web pages. Clicking an hyperlink asks the operating system to get a particular Web page from another computer connected to the Internet.

The Web page to get is specified with a uniform resource locator URL. A URL specifies the exact computer (among all the Internet computers in the world) and the exact Web page on that computer.

To see some examples of URLs, keep watching the box at the top of your browser labeled "Address".

## More

### BIOS

Software code built into the computer that handle sending data from one part of the computer to another.

### Boot (boot-up)

Process happening when a computer is turned on. Checks all the components function properly and that the operating system is loaded. Term comes from the expression "lifting yourself by your bootstraps".

### Circuit board

A board with metallic wires printed into it that connect components. Eliminates the need for separate wiring of the componants. Its creation can be automated. It also reduces the physical space needed.
