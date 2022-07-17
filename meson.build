project('ultimatepp',
        'cpp',
        version: '2022.2',
        license: 'BSD',
        default_options: ['cpp_std=c++14', 'default_library=static'])

# add_project_link_arguments(['-Wl,-no-undefined'], language: 'cpp', native: false)


date_prog = find_program('date', native: false)
hostname_prog = find_program('hostname', native: false)
whoami_prog = find_program('whoami', native: false)

date_output = run_command(date_prog, '+%Y-%m-%d-%H-%M-%S', check: true, capture: true).stdout().strip()
hostname_output = run_command(hostname_prog, check: true, capture: true).stdout().strip()
whoami_output = run_command(whoami_prog, check: true, capture: true).stdout().strip()

date_pieces = date_output.split('-')
the_time = '"@0@:@1@:@2@"'.format(date_pieces[3], date_pieces[4], date_pieces[5])

ide_configuration_data = configuration_data({
'bmYEAR': date_pieces[0],
'bmMONTH': date_pieces[1],
'bmDAY': date_pieces[2],
'bmHOUR': date_pieces[3],
'bmMINUTE': date_pieces[4],
'bmSECOND': date_pieces[5],
'bmTIME': the_time
})

configure_file(output: 'build_info.h', configuration: ide_configuration_data)

root_inc = include_directories('.')

subdir('uppsrc')
