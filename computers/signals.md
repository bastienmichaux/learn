# Computers

## Signals

## Binary

A binary device (e.g. a light switch) can be in just one of two possible states: a bit. A bit is a single on/off value.

Some devices are  discrete — have definite states — but there are usually more than two states (off, running, start, accessories ) A button on a electronic calculator is a binary device. It is either on or off. Ordinarily it is off. When you push it, it is on. It springs back to off when you release it, which is different from a toggle switch, but it still is a binary device.

Four important reasons for using binary:
- Binary devices are Simple and easy to build.
- Binary signals are Unambiguous (which gives them noise immunity).
- Flawless copies can be made of binary data.
- Anything that can be represented with some sort of pattern can be represented with patterns of bits.

These characteristics of binary were realized by Claude Shannon, a mathematician at Bell Telephone Laboratories. His 1948 paper A Mathematical Theory of Communication is the foundation of information theory and much of computer science.

## Analog

An analog signal may continuously change in value. Its values can be anything within a range of values, and its exact value at any time is important. The graph represents an audio signal. The exact value at each time is part of the information it contains. For example, the value at time "T2" must be measured exactly.

Now say that you are observing the voltage of a wire. It has been agreed that any voltage below a threshold will be counted as an "off" signal, and that any value above the threshold will be counted as an "on" signal.

## Binary signal

Analog signals usually continuously change their value. The information they convey is contained in the exact value at any instant.

However, by using a threshold, a signal can represent binary data ("on/off" data). Such a signal is called binary signal.

It is easy and fast to determine if a voltage is above or below a threshold. The signal in the figure is "off" at time T1 and then "on" at time T2.

### Imperfect transmission

The "ons" and "offs" of previous signal are clear. But what if the signal is sent down a long wire and someone nearby turns on a vacuum cleaner? The graph shows the signal at the other end of the wire.

Even though the signal is noisy (at the analog level), the binary values are transmitted perfectly. You (and the electronics) can still tell that at time T1 the signal represents "off" and that at time T2 the signal represents "on" The receiving end just needs to get the binary values.

Since only the "on" "off" information matters, the analog noise is irrelevant, and the original signal is received perfectly (so far as the binary information goes.)

### Flawless copies

Flawless copies can be made: The receiving end of the signal is only interested in the binary values. All it has to do it check if the signal is above or below the threshold. This can be done perfectly (as long as the noise is not too great.) For example, the picture shows the noisy signal with the on/off values recovered from it.

The original signal has been recovered flawlessly. This process can occur as many times as needed with a perfect copy made each time. This is essential in a computer system, where bit patterns (patterns of one and zero, or on and off) are copied back and forth between the processor and memory millions of times a second. The copies have to be perfect.

### Representing data
Since data of all kinds is stored in computer memory (main and secondary) using the same electronic methods, this means that endless perfect copies can be made of any type of data or program.

This idea is that any system of symbols can be translated into bit patterns. An example is how English characters are represented as eight-bit patterns. The agreement about what patterns represent what characters is called ASCII. The hardware and the software of a computer system (usually) follow this agreement when the data is "text". (You will learn more about this later). Other types of data (non-character data) are represented using other methods.

## Clocks
Digital systems are built so that the on/off (binary) value is tested only at certain points in time, giving the wire (or other device) time to change. This is why computer systems have a clock. The clock keeps all these time points synchronized. Faster clocks mean wires can be tested more times per second, and the whole system runs faster.

Processor chips are often described in terms of their clock speed. Clock speed is measured in Hertz, where one Hertz is one clock tick per second. The symbol MHz means megahertz, a million (106) clock ticks per second. The symbol GHz means gigahertz, a billion (109) clock ticks per second.

A 2 GHz processor checks binary values two billion times in each second. In between these times values are allowed to change and settle down. The faster a processor chip is, the more times per second values can be tested, and the more decisions per second can be made.