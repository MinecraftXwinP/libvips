add_library(
	conversion
	autorot.c
	insert.c
	flip.c
	pconversion.h
	falsecolour.c
	recomb.c
	smartcrop.c
	flatten.c
	msb.c
	replicate.c
	bandfold.c
	bandunfold.c
	tilecache.c
	premultiply.c
	unpremultiply.c
	grid.c
	zoom.c
	cast.c
	transpose3d.c
	join.c
	cache.c
	bandbool.c
	sequential.c
	subsample.c
	bandmean.c
	bandary.h
	arrayjoin.c
	scale.c
	copy.c
	bandary.c
	embed.c
	conversion.c
	wrap.c
	rot45.c
	ifthenelse.c
	byteswap.c
	gamma.c
	bandjoin.c
	bandrank.c
	rot.c
	extract.c
)
target_include_directories(conversion PUBLIC ${VIPS_INCLUDE_DIR})

target_link_libraries(conversion PkgConfig::glib-2.0)