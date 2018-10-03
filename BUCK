# cxx_genrule(
genrule(
  name = 'config-h', 
  out = 'config.h', 
  srcs = [
    'CMakeLists.txt', 
    'config.h.in', 
  ], 
  cmd = ' && '.join([
    'cp -r $SRCDIR/. $TMP', 
    'cd $TMP', 
    'cmake . ', 
    # 'cmake -DCMAKE_C_COMPILER="$(cc)" -DCMAKE_CXX_COMPILER="$(cxx)" -DCMAKE_C_FLAGS="$(cflags)" -DCMAKE_CXX_FLAGS="$(cxxflags)" . ', 
    'cp ./config.h $OUT', 
  ]), 
)
