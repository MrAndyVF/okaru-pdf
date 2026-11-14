# okaru-pdf: document viewer de OKARU. Se compila contra el núcleo instalado (paquete okaru-core).
project('okaru-pdf', 'cpp',
  version: files('VERSION'),
  meson_version: '>=1.1',
  default_options: ['cpp_std=c++23', 'cpp_extensions=false', 'warning_level=0', 'b_ndebug=if-release'],
)

# El núcleo y sus bibliotecas son privados (/usr/lib/okaru): se enlazan con su ruta en el binario.
_okaru_libdir = get_option('prefix') / get_option('libdir') / 'okaru'
_deps = [dependency('okaru-apps')]
_inc = include_directories('src')
_args = ['-Wall', '-Wextra', '-Wno-missing-field-initializers', '-Wpedantic', '-Wconversion', '-Wshadow']

executable('okaru-pdf',
  sources: files('src/apps/pdf/main.cpp', 'src/apps/pdf/pdf_sidebar.cpp', 'src/apps/pdf/pdf_window.cpp'),
  include_directories: _inc,
  dependencies: _deps,
  cpp_args: _args,
  install_rpath: _okaru_libdir,
  install: true,
)

# Sus textos, que el núcleo busca en /usr/share/okaru/apps/pdf/translations.
install_subdir('apps/pdf/translations', install_dir: get_option('datadir') / 'okaru' / 'apps' / 'pdf')
install_data('assets/dev.okaru.Pdf.desktop', install_dir: get_option('datadir') / 'applications')
