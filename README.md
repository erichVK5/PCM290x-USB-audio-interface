# PCM290x-USB-audio-interface

An  open source hardware USB audio interface board for amateur radio and other applications.

The June 2014 edition of Amateur Radio magazine published a design for a USB sound card based
on the PCM290x family of CODECs. The depicted prototype used the PCM2904.

The board has optional connectors for the 3 switches supported by the CODEC, an SPDIF header
for the codec models that support it, as well as space for 2 optional input and 2 optional
output level adjustment potentiometers (Jumpered with 4 small wire links in the published photo).

The board is 50mm x 50mm and has been designed for easy mounting in existing commercial rigs
or homebrew rigs, or as a standalone unit. Input and output 3.5mm stereo sockets are supported
to make connections simpler, as well as simple headers for those not using 3.5mm audio leads,
and a Type B USB socket mounts directly to the board.

The option of an external regulated power supply for the ADC/DAC section of the CODEC is also
supported.

Soldering was quick and easy, in fact three boards were done at once, using a hotplate (aka skillet)
liftoff jig technique.

SDR homebrewers need to be aware of the one sample audio packet misalignment issue in some of
the PCM290x revisions, and must either

1) choose unaffected revisions by studying the errata, or
2) empirically determine if the codec used does it, or
3) adjust their software to avoid phasing errors if using an affected codec

The design has been released under the TAPR open hardware licence, see http://www.tapr.org/OHL

Radio amateurs are encouraged to modify and experiment and include the board in homebrew or
commercial rigs needing USB audio for I/Q or digimodes.

VK5HSE-PCM2904-v1.0.zip contains gerber files which can be sent to a PCB manufacturer to have boards made. The boards shown in AR magazine were made by hackvana.com and are eligible for preferential pricing due to the board dimensions being 50mmx50mm. 

The gerber files are industry standard and can be used by any PCB manufacturer that accepts gerber files, with at most minor changes to the file endings for the PCB layers.

The schematic simply implements the reference design in the data sheet for the PCM290x family.
