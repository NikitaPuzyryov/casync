libshared_sources = files('''
	cachunk.c
	cachunk.h
	cachunker.c
	cachunker.h
	cachunkid.c
	cachunkid.h
	cacommon.h
	cadecoder.c
	cadecoder.h
	caencoder.c
	caencoder.h
	cafileroot.c
	cafileroot.h
	caformat-util.c
	caformat-util.h
	caformat.h
	caindex.c
	caindex.h
	calocation.c
	calocation.h
	camakebst.c
	camakebst.h
	canbd.c
	canbd.h
	caorigin.c
	caorigin.h
	caprotocol-util.c
	caprotocol-util.h
	caprotocol.h
	caremote.c
	caremote.h
	caseed.c
	caseed.h
	castore.c
	castore.h
	casync.c
	casync.h
	cautil.c
	cautil.h
	def.h
	fssize.c
	fssize.h
	gcrypt-util.c
	gcrypt-util.h
	parse-util.c
	parse-util.h
	realloc-buffer.c
	realloc-buffer.h
	reflink.c
	reflink.h
	rm-rf.c
	rm-rf.h
	siphash24.c
	siphash24.h
	util.c
	util.h
'''.split())

libshared = static_library(
	      'shared',
	      libshared_sources)

casync_sources = files('''
	casync-tool.c
	canbd.c
	canbd.h
	cafuse.h
	signal-handler.c
	signal-handler.h
'''.split())

if conf.get('HAVE_FUSE') == 1
        casync_sources += files('cafuse.c')
endif

casync_http_sources = files('casync-http.c')
