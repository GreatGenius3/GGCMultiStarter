cmake_minimum_required(VERSION 3.10)
project(CMultiStarter C)

set(CMAKE_C_STANDARD 17)
set(CMAKE_C_STANDARD_REQUIRED ON)

# Sätter gemensam utdatakatalog för den färdiga .exe-filen
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}")

# Lägg till subdirektorn
add_subdirectory(Exampel01)
add_subdirectory(Exampel02)