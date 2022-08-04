project('proj1', 'c')

libproj1 = both_libraries('proj1',
    'proj1.c',
)

libproj1_dep = declare_dependency(
    link_with: libproj1,
    include_directories: include_directories('.'),
)
