include_defs('//BUCKAROO_DEPS')

cxx_library(
  name = 'boost-container',
  header_namespace = 'boost/container',
  exported_headers = subdir_glob([
    ('include/boost/container', '**/*.hpp'),
  ], 
  excludes = [
    'include/boost/container/detail/**/*.hpp',
  ]),
  headers = subdir_glob([
    ('include/boost/container', 'detail/**/*.hpp'),
    ('include/boost/container', 'detail/**/*.h'),
  ]),
  srcs = glob([
    'src/**/*.cpp',
  ]),
  visibility = [
    'PUBLIC',
  ],
  deps = BUCKAROO_DEPS,
)
