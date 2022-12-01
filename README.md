- 👋 Hi, I’m @ggpaeist888
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
ggpaeist888/ggpaeist888 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Merge tag 'char-misc-6.1-rc7' of git://git.kernel.org/pub/scm/linux/k…
…ernel/git/gregkh/char-misc
Pull char/misc driver fixes from Greg KH:
 "Here are some small driver fixes for 6.1-rc7, they include:

   - build warning fix for the vdso when using new versions of grep

   - iio driver fixes for reported issues

   - small nvmem driver fixes

   - fpga Kconfig fix

   - interconnect dt binding fix

  All of these have been in linux-next with no reported issues"

* tag 'char-misc-6.1-rc7' of git://git.kernel.org/pub/scm/linux/kernel/git/gregkh/char-misc:
  lib/vdso: use "grep -E" instead of "egrep"
  nvmem: lan9662-otp: Change return type of lan9662_otp_wait_flag_clear()
  nvmem: rmem: Fix return value check in rmem_read()
  fpga: m10bmc-sec: Fix kconfig dependencies
  dt-bindings: iio: adc: Remove the property "aspeed,trim-data-valid"
  iio: adc: aspeed: Remove the trim valid dts property.
  iio: core: Fix entry not deleted when iio_register_sw_trigger_type() fails
  iio: accel: bma400: Fix memory leak in bma400_get_steps_reg()
  iio: light: rpr0521: add missing Kconfig dependencies
  iio: health: afe4404: Fix oob read in afe4404_[read|write]_raw
  iio: health: afe4403: Fix oob read in afe4403_read_raw
  iio: light: apds9960: fix wrong register for gesture gain
  dt-bindings: interconnect: qcom,msm8998-bwmon: Correct SC7280 CPU compatible
