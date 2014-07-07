This relatively compact, cheap, simple FMCW radar operates in the spectrum around 5.8-6.0 GHz and is aimed at lowering the barrier to entry for experiments with radar and general education around RF and microwave electronics. It is capable of speed measurement,
rangefinding and SAR imaging (with appropriate moving antennas or a moving vehicle.) It is potentially applicable to experiments with autonomous aircraft (or spacecraft) altitude-finding, SAR imaging/mapping or navigation as an alternative to (or in addition to)
other sensing techniques such as GPS, ultrasonics, LIDAR or barometry, without some of the limitations applicable to those technologies.

This is still an early prototype, a rough quick work that is still very much in progress and evolving as bits are designed and built and redesigned.

Frequency-modulated RF is generated by the HMC431 VCO, at about 5.8-6.0 GHz, amplified by a HMC476 MMIC gain block, and split in half by the Wilkinson divider. Half the RF output from the divider is amplified again and sent to the transmit antenna connector.
The local oscillator, from the other side of the splitter, is amplified again and applied to the LO port of the HMC219 double-balanced mixer. The reflected RF from the receive antenna comes in at bottom right, where it is amplified by the HMC717 6 GHz LNA and the
amplified output is applied to the mixer.

A couple of pi attenuators are used, after the VCO, before the mixer LO port and after the mixer's IF output, to "tune" optimal mixer LO level and overall performance. Although I haven't fixed certain values for these attenuators yet, space for them is left on
the board.

IF filtering, amplification and signal processing, along with generation of the 0-10V modulation signal for the VCO, are done on a separate board.

License information: Open Hardware as per the CERN Open Hardware License; please see license.txt