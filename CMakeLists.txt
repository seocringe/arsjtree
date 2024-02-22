cmake_minimum_required(VERSION 3.0)
project(MyProject VERSION 1.0.0)

# Установка стандарта C++
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Добавление исполняемого файла
add_executable(MyExecutable main.cpp)

# Если вам нужно добавить поддиректории, используйте add_subdirectory(имя_поддиректории)
# Если вам нужно линковать библиотеки, то используйте target_link_libraries(MyExecutable имя_библиотеки)

# Инсталляция (опционально)
install(TARGETS MyExecutable DESTINATION bin)
