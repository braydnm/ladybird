set(SOURCES
    BackgroundAction.cpp
    Thread.cpp
./public/TracyClient.cpp
)

serenity_lib(LibThreading threading)
add_compile_definitions(TRACY_ENABLE)
target_link_libraries(LibThreading PRIVATE LibCore)
