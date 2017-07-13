## kernel-patches
Miscellaneous patches for the Linux kernel

# CPUFreq Interactive Governor patches for the Linux kernel
The Interactive governor must be set to built-in (not module) in your kernel config for the build to succeed.
Swapping to and from Interactive on a running system can be problematic, so if you want to try this governor it's suggested to set it as the default in your kernel config.

# 600Hz timer interrupt rate patch for the Linux kernel
All common video framerates (24, 25, 30, 50, 60) are evenly divisible by 600, so it's a good interrupt rate for those working with realtime video.
It's also nicely halfway between in the "1000Hz vs 300/250Hz" debate.
