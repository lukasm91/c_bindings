cpp_bindgen_add_library(gen_regression_array_gt_legacy SOURCES implementation.cpp)

add_executable(gen_regression_array_gt_legacy_driver_fortran driver.f90)
target_link_libraries(gen_regression_array_gt_legacy_driver_fortran gen_regression_array_gt_legacy_fortran)
add_test(NAME gen_regression_array_gt_legacy_driver_fortran COMMAND gen_regression_array_gt_legacy_driver_fortran)
