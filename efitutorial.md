# Working Intel HD 530 graphics on macOS Mojave on a Dell Optiplex 7040.

1. In order to get graphics working on macOS Mojave with the Intel HD 530 graphics, you will need to boot into the Clover boot menu, and then press "Start UEFI Shell 64". 

2. Then run setup_var 0x350 0x4, which will make sure 128MB+ of memory is allocated to your iGPU.

Please note that the "0x350" variable only works on the Dell Optiplex 7040, and differs on other Dell Optiplex models.