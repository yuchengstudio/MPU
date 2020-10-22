# 1.参考链接
https://github.com/atmelcorp/atmel-software-package/tree/master/examples/low_power_mode

# 2.在Linux（ubuntu）下操作步骤
). Install cross compiler:
$ sudo apt install gcc-arm-none-eabi
<br/>
2). Download softpack source codes:
$ git clone https://github.com/atmelcorp/atmel-software-package.git
<br/>
3). Cross compile getting_started application in softpack:
<br/>$ cd atmel-software-package/examples/low_power_mode
<br/>$ make TARGET=sama5d27-som1-ek CROSS_COMPILE=arm-none-eabi-
<br/>（备注：如果是对SAM9X60 demo的测试，请将sama5d27-som1-ek 替换成 sam9x60-ek）
<br/>（备注：如果希望从SRAM启动VARIANT=sram）
<br/>After compiling successful, binary file getting-started.bin should be found in atmel-software-package/examples/getting_started/build/sama5d27-som1-ek/sram/


