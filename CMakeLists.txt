cmake_minimum_required(VERSION 3.6)

project(test-project-a 
	VERSION 1.0.0
	LANGUAGES CXX
	DESCRIPTION "Test Project A."
	)

include(GNUInstallDirs)
install(DIRECTORY include/ CONFIGURATIONS Release DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}/test-project-a" FILES_MATCHING PATTERN "*")
