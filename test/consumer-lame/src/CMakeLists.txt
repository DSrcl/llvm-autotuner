set(PROG consumer-lame)
set(CPPFLAGS -DHAVEMPGLIB -DLAMEPARSE -DNDEBUG -D__NO_MATH_INLINES -O -DLAMESNDFILE)
set(LDFLAGS -lm)
set(RUN_OPTIONS -S ${CMAKE_CURRENT_SOURCE_DIR}/large.wav Output/output_large.mp3)
set(USE_REFERENCE_OUTPUT 1)
llvm_multisource()
