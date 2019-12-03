project(DSTools)

add_compile_options(
	-nostdinc
)

#add_darling_executable(dsmemberutil dsmbrutil/dsmbrutil.c)

# Disabling in favor of stub
#install(TARGETS dsmemberutil DESTINATION libexec/darling/usr/bin)

install(FILES
	dirt/dirt.1
	dscacheutil/dscacheutil.1
	dscacheutil/lookupd.1
	dscl/dscl.1
	dsconfigldap/dsconfigldap.1
	dsmbrutil/dsmemberutil.1
	dsmbrutil/memberd.1

	DESTINATION libexec/darling/usr/share/man/man1
)

install(FILES
	dsenableroot/dsenableroot.8
	dserr/dserr.8
	pwpolicy/pwpolicy.8
	ugtools/dseditgroup.8

	DESTINATION libexec/darling/usr/share/man/man8
)
