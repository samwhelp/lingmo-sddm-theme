cmake_minimum_required(VERSION 3.5)

project(yoyo-sddm-theme)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTORCC ON)

install(FILES Main.qml DESTINATION /usr/share/sddm/themes/yoyo)
install(FILES SessionMenu.qml DESTINATION /usr/share/sddm/themes/yoyo)
install(FILES UserView.qml DESTINATION /usr/share/sddm/themes/yoyo)
install(FILES FishUIMenu.qml DESTINATION /usr/share/sddm/themes/yoyo)
install(FILES FishUIMenuItem.qml DESTINATION /usr/share/sddm/themes/yoyo)
install(FILES system-shutdown-symbolic.svg DESTINATION /usr/share/sddm/themes/yoyo)

install(FILES theme.conf DESTINATION /usr/share/sddm/themes/yoyo)
install(FILES hidpi.conf DESTINATION /etc/sddm.conf.d/)
install(FILES sddm.conf DESTINATION /etc/)

# install(FILES "faces/.face.icon" DESTINATION /usr/share/sddm/faces/)
