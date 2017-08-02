#
# project: fips-libjpeg
#
cmake_minimum_required(VERSION 2.8)

# include the fips main cmake file
get_filename_component(FIPS_ROOT_DIR "../fips" ABSOLUTE)
include("${FIPS_ROOT_DIR}/cmake/fips.cmake")

fips_setup()
fips_project(fips-libjpeg)

fips_begin_lib(libjpeg)
fips_src(libjpeg/ NO_RECURSE)
fips_end_lib()

fips_finish()


