Updated Dec 14 2021

- Fix ping rate
- Fix Hash display
- Updated config.joson file
- sample binary file.

Miner fee reduced by 0.25% while mining on Flockpool.com

Remember that you can reuse the tune_config files from version 1.2.X by copying it into the 1.2.4.1 main folder.
Alder Lake (12th gen intel) users are highly recommended to retune the miner.
Make sure E cores number was detected properly.


General:

    Update startup scripts to accommodate changes in Windows 11.
    Use new avx2-sha-vaes on Alder Lake.
    Correct some output inconsistencies while tuning.

Improvements:

    Add improvements for Alder Lake tuning. ~6% (12900k) increase in hashrate.
    Retuning of the system is REQUIRED to get improved performance.

Flags:

    Add --ecores=N - Specify the number of E cores of the CPU. Miner will try to
    autodetect. It will show the predicted number. Specifying it incorrectly or on the
    platform that does NOT support E cores (Intel Alder Lake) can lead to
    reduced performance.
    Add --disable-rot=LIST - Comma separated list of rotations to not be used
    while mining. For testing purposes only! Using this for normal mining WILL
    reduce your overall average hashrate!! Does not apply to the tuning process.


This project is a fork form cpuminer-gr-1.2.4.1-x86_64.
