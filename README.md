# Raspberry Pi Codec Zero (and IQaudIO Pi-Codec+ / Pi-CodecZero)

These are ALSA configuration ("state") files for the Raspberry Pi Codec Zero
and IQaudIO Pi-Codec+ / Pi-CodecZero soundcards. Although functionally
equivalent, the Raspberry Pi and IQaudIO versions appear with different names
for the cards, requiring different configuration files, and the boards
themselves differ in colour - Raspberry Pi boards are green, IQaudIO boards
are black.

To load a state file, from the command line use:

    sudo alsactl restore -f <filename>

where `<filename>` is one of the following:

    # Raspberry Pi branded:
    Codec_Zero_AUXIN_record_and_HP_playback.state
    Codec_Zero_OnboardMIC_record_and_SPK_playback.state
    Codec_Zero_Playback_only.state
    Codec_Zero_StereoMIC_record_and_HP_playback.state

    # IQaudIO branded:
    IQaudIO_Codec_AUXIN_record_and_HP_playback.state
    IQaudIO_Codec_OnboardMIC_record_and_SPK_playback.state
    IQaudIO_Codec_Playback_only.state
    IQaudIO_Codec_StereoMIC_record_and_HP_playback.state
