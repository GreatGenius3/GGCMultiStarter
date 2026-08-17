# Sätt målet för den körbara filen
add_executable(Exampel01 main.c)

# Skickar vidare Debug/Release-flaggor till källkoden i alla miljöer (CLion, VS Code & Visual Studio)
target_compile_definitions(Exampel01 PRIVATE
        $<$<CONFIG:Debug>:BUILD_MODE_DEBUG>
        $<$<CONFIG:Release>:BUILD_MODE_RELEASE>
)
