SET(SCEVENT_REGIONCHECKPLUGIN_SOURCES regioncheck.cpp)
SC_ADD_PLUGIN_LIBRARY(SCEVENT_REGIONCHECKPLUGIN evrc scevent)
SC_LINK_LIBRARIES_INTERNAL(evrc evplugin)

FILE(GLOB descs "${CMAKE_CURRENT_SOURCE_DIR}/descriptions/*.xml")
INSTALL(FILES ${descs} DESTINATION ${SC3_PACKAGE_APP_DESC_DIR})
