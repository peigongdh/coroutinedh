project(coroutinedh)

set(SRC_LIST test_ctx.cpp contextu.c)
message(STATUS ${SRC_LIST})
message(STATUS "This is Binary dir" ${PROJECT_BINARY_DIR})
message(STATUS "This is Source dir" ${PROJECT_SOURCE_DIR})
add_executable(test_ctx.bin ${SRC_LIST})

set(SRC_LIST test_swap.cpp contextu.c)
message(STATUS ${SRC_LIST})
message(STATUS "This is Binary dir" ${PROJECT_BINARY_DIR})
message(STATUS "This is Source dir" ${PROJECT_SOURCE_DIR})
add_executable(test_swap.bin ${SRC_LIST})

set(SRC_LIST main.c coroutine.c contextu.c)
message(STATUS ${SRC_LIST})
message(STATUS "This is Binary dir" ${PROJECT_BINARY_DIR})
message(STATUS "This is Source dir" ${PROJECT_SOURCE_DIR})
add_executable(coroutine.bin ${SRC_LIST})

set(SRC_LIST producer_consumer.c coroutine.c contextu.c)
message(STATUS ${SRC_LIST})
message(STATUS "This is Binary dir" ${PROJECT_BINARY_DIR})
message(STATUS "This is Source dir" ${PROJECT_SOURCE_DIR})
add_executable(producer_consumer.bin ${SRC_LIST})