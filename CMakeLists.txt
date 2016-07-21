cmake_minimum_required(VERSION 3.0)
project(appstreamrunner)

find_package(ECM 1.7.0 REQUIRED NO_MODULE)
set(CMAKE_MODULE_PATH ${ECM_MODULE_PATH})

find_package(Qt5 REQUIRED COMPONENTS Gui)
find_package(KF5 REQUIRED COMPONENTS I18n Runner)
find_package(AppstreamQt REQUIRED 0.9.2)

include(KDEInstallDirs)
include(KDECompilerSettings NO_POLICY_SCOPE)
include(KDECMakeSettings)
include(ECMInstallIcons)
include(FeatureSummary)
include(ECMAddAppIcon)

add_subdirectory(src)
