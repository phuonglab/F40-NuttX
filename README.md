F40-NuttX
=========

Build Nuttx for stm32f4:
C1:
+Build toolchains: 
  Downlaod: https://github.com/MikeSmith/summon-arm-toolchain.git
  git clone git://github.com/esden/summon-arm-toolchain
  cd summon-arm-toolchain
  ./summon-arm-toolchain
+Build kconfig-frontends
  download :
  cd kconfig-frontends-3.3.0-1
  ./configure --prefix to /sal folder 
  make install
+Build Nuutx:
  get source code: apps nuttx misc
  cd nuttx/tools
  ./configure.sh stm32f4discovery/nsh( depend on board bsp surppose)
  cd ..
  make
  
