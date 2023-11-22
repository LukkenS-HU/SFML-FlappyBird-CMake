cmake_minimum_required(VERSION 3.26)
project(SFMLFlappyBird)

set(CMAKE_CXX_STANDARD 23)

add_subdirectory(SFML-2.6.1)

add_executable(SFMLFlappyBird main.cpp AssetManager.cpp Bird.cpp Collision.cpp Flash.cpp Game.cpp GameOverState.cpp GameState.cpp HUD.cpp InputManager.cpp Land.cpp MainMenuState.cpp Pipe.cpp SplashState.cpp StateMachine.cpp)
target_link_libraries(SFMLFlappyBird sfml-system sfml-window sfml-graphics sfml-audio)