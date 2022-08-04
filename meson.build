project('testmesoninterdep', 'c', version: '0')

proj1 = subproject('proj1')
libproj1_dep = proj1.get_variable('libproj1_dep')
meson.override_dependency('proj1', libproj1_dep)
proj2 = subproject('proj2')
libproj2_dep = proj2.get_variable('libproj2_dep')

executable('testmesoninterdep',
    'testmesoninterdep.c',
    dependencies: [libproj1_dep, libproj2_dep],
)
