set(LLVM_LINK_COMPONENTS
  Support
  )

add_clang_executable(clang-llvm-rename
  ClangLLVMRename.cpp
  )

target_link_libraries(clang-llvm-rename
  PRIVATE
  clangAST
  clangASTMatchers
  clangBasic
  clangFrontend
  clangTooling
  clangToolingRefactoring
  clangToolingCore
  clangLex
  clangSerialization
  )
set(LLVM_LINK_COMPONENTS
  support
  )
