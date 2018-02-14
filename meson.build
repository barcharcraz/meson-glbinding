project('glbinding',
	languages: ['c++'],
	version: '3.0.0',
	default_options: ['cpp_std=c++11'])

# python_prog = find_program('python')
# message('Command update')
# message('Command generate')


#if get_option('update_gl_spec')
#	update_target = custom_target('update',
#		command: [python_prog, '-f', '@INPUT@'],
#		input: ['source/codegeneration/gl.xml'])
#endif

#generate_target = run_target('generate',
#	command: [python_prog, '

feature_sets = [
'gl',
'gl10',
'gl10ext',
'gl11',
'gl11ext',
'gl12',
'gl12ext',
'gl13',
'gl13ext',
'gl14',
'gl14ext',
'gl15',
'gl15ext',
'gl20',
'gl20ext',
'gl21',
'gl21ext',
'gl30',
'gl30ext',
'gl31',
'gl31ext',
'gl32',
'gl32core',
'gl32ext',
'gl33',
'gl33core',
'gl33ext',
'gl40',
'gl40core',
'gl40ext',
'gl41',
'gl41core',
'gl41ext',
'gl42',
'gl42core',
'gl42ext',
'gl43',
'gl43core',
'gl43ext',
'gl44',
'gl44core',
'gl44ext',
'gl45',
'gl45core',
'gl45ext',
'gl46',
'gl46core',
'gl46ext'
]
header_dir =  'source/glbinding/include/glbinding/'
headers = files(
	header_dir + '/glbinding/callbacks.h',
	header_dir + '/glbinding/nogl.h',
	header_dir + '/glbinding/AbstractFunction.h',
	header_dir + '/glbinding/AbstractValue.h',
	header_dir + '/glbinding/CallbackMask.h',
	header_dir + '/glbinding/CallbackMask.inl',
	header_dir + '/glbinding/Function.h',
	header_dir + '/glbinding/Function.inl',
	header_dir + '/glbinding/FunctionCall.h',
	header_dir + '/glbinding/Binding.h',
	header_dir + '/glbinding/Meta.h',
	header_dir + '/glbinding/ProcAddress.h',
	header_dir + '/glbinding/ContextHandle.h',
	header_dir + '/glbinding/ContextInfo.h',
	header_dir + '/glbinding/Value.h',
	header_dir + '/glbinding/Value.inl',
	header_dir + '/glbinding/Version.h',
	header_dir + '/glbinding/Version.inl',
	header_dir + '/glbinding/SharedBitfield.h',
	header_dir + '/glbinding/SharedBitfield.inl',
	header_dir + '/glbinding/logging.h'
)
sources = files(

foreach feature : feature_sets
	headers += files(
		header_dir + feature + '/bitfield.h',
		header_dir + feature + '/boolean.h',
		header_dir + feature + '/enum.h',
		header_dir + feature + '/functions.h',
		header_dir + feature + '/gl.h',
		header_dir + feature + '/types.h',
		header_dir + feature + '/values.h'
	)
endforeach