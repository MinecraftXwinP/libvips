add_library(
	histogram
	phistogram.h
	hist_cum.c
	hist_entropy.c
	hist_equal.c
	hist_ismonotonic.c
	hist_local.c
	hist_match.c
	hist_norm.c
	hist_plot.c
	hist_unary.c
	histogram.c
	maplut.c
	percent.c
	stdif.c
)
target_include_directories(histogram PUBLIC ${VIPS_INCLUDE_DIR})

target_link_libraries(histogram PkgConfig::glib-2.0)
