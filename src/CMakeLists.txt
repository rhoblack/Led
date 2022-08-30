add_executable(${PROJECT_NAME}
    main.cpp
    ./hw/Led/Led.cpp
)

target_include_directories(${PROJECT_NAME} PUBLIC
    ./
    ./ap
    ./hw
    ./hw/Led
)

target_compile_options(${PROJECT_NAME} PUBLIC
    -Wall
)

target_link_libraries(${PROJECT_NAME} PUBLIC
    -lwiringPi
)