set(LLVM_LINK_COMPONENTS
  BitReader
  BitWriter
  Core
  IRReader
  Linker
  Object
  Support
  TransformUtils
  IPO
  )

add_llvm_tool(llvm-link-cudafe
  llvm-link-cudafe.cpp

  DEPENDS
  intrinsics_gen
  )
