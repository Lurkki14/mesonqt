project('qt_test',
        'cpp',
	default_options : ['cpp_std=c++11'])

qt5 = import('qt5')
qt5_dep = dependency('qt5', modules: ['Widgets'])
# inc = include_directories('includes')

moc_files = qt5.preprocess(moc_headers : 'MainWindow.h',
                           dependencies : qt5_dep)

executable('qt_test', 'main.cpp', 'MainWindow.cpp', moc_files, dependencies : qt5_dep)
