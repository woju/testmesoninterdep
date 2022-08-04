project('proj2', 'c')

proj1_dep = dependency('proj1')

libproj2 = both_libraries('proj2',
    'proj2.c',
    dependencies: proj1_dep,
)

libproj2_dep = declare_dependency(
    link_with: libproj2,
    include_directories: include_directories('.'),
)
