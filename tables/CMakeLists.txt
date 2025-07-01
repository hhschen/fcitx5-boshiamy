fcitx5_translate_desktop_file("boshiamy.conf.in" "boshiamy.conf")

add_custom_command(OUTPUT "boshiamy.main.dict"
  DEPENDS "boshiamy.txt"
  COMMAND LibIME::tabledict ARGS "${CMAKE_CURRENT_SOURCE_DIR}/boshiamy.txt"
  "${CMAKE_CURRENT_BINARY_DIR}/boshiamy.main.dict")

add_custom_target(table_data ALL DEPENDS boshiamy.main.dict)

install(FILES
  "${CMAKE_CURRENT_BINARY_DIR}/boshiamy.conf"
  DESTINATION "${FCITX_INSTALL_PKGDATADIR}/inputmethod")

install(FILES
  "${CMAKE_CURRENT_BINARY_DIR}/boshiamy.main.dict"
  DESTINATION "${FCITX_INSTALL_PKGDATADIR}/table")
