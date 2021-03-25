m4_define([RAM], [2G])
m4_define([ACCELERATOR], [kvm])
m4_define([CORES], [2])
m4_define([CPU], [Penryn])
m4_define([CPU_VENDOR], [GeniuneIntel])
m4_define([CPU_FLAGS], [+sse3,+sse4.2,+aes,+xsave,+avx,+xsaveopt,+xsavec,+xgetbv1,+avx2,+bmi2,+smep,+bmi1,+fma,+movbe,+invtsc])
m4_define([CPU_NOT_HIDDEN], [on])
m4_define([VGA_TYPE], [none])
m4_define([DEVICES], [])
m4_define([DRIVES], [])
m4_define([EXTRA_FLAGS], [])
echo "qemu-system-x86_64 -enable-kvm -m RAM -machine q35,accel=ACCELERATOR -smp 4,cores=CORES -cpu CPU,vendor=CPU_VENDOR,kvm=CPU_NOT_HIDDEN,CPU_FLAGS -vga VGA_TYPE" > start.sh
python3 add_extra_flags devs="DEVICES" drives="DRIVES"
echo EXTRA_FLAGS >> start.sh
