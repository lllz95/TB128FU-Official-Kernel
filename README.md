官方公开源码中未包含快充相关内容，所以引入[Eddie07/android_kernel_tb128fu](https://github.com/Eddie07/android_kernel_tb128fu)的充电驱动修复联想的超级闪充

由于[Eddie07/android_kernel_tb128fu](https://github.com/Eddie07/android_kernel_tb128fu)的充电驱动无法显示联想充电时的“超级闪充”动画，强制将get_charge_type映射为1（PPS类）即可显示（charge_type=2是USB_FLOAT / TwinTurbo双引擎闪充）
