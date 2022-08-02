# Specify the name of the executable.
add_executable(SupplementalAssignment)

# Specify the source files to be compiled.
target_sources(SupplementalAssignment PRIVATE(SupplementalAssignment.c(SupplementalAssignment.S)

# Pull in commonly used features.
target_link_libraries(SupplementalAssignment PRIVATE pico_stdlib)

# Create map/bin/hex file etc.
pico_add_extra_outputs(SupplementalAssignment)

# Add the URL via pico_set_program_url.
apps_auto_set_url(SupplementalAssignment)
