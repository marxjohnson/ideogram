icon_sizes = ['16', '24', '32', '48', '64', '128']

foreach i : icon_sizes
    install_data (
        join_paths ('icons', i + '.svg'),
        install_dir: join_paths (get_option ('datadir'), 'icons', 'hicolor', i + 'x' + i, 'apps'),
        rename: meson.project_name () + '.svg'
    )
    install_data (
        join_paths ('icons', i + '.svg'),
        install_dir: join_paths(get_option ('datadir'), 'icons', 'hicolor', i + 'x' + i + '@2', 'apps'),
        rename: meson.project_name () + '.svg'
    )
endforeach

install_data (
    'launcher.desktop',
    install_dir: join_paths (get_option ('datadir'), 'applications'),
    rename: meson.project_name () + '.desktop'
)

install_data (
    'appdata.xml',
    install_dir: join_paths (get_option ('datadir'), 'metainfo'),
    rename: meson.project_name () + '.appdata.xml'
)

