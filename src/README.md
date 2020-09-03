# Banxster
sofar Banxster project

Sequence of exec files for autonomous navigation (SLAM)

Create a map

- run_gazebo.sh ( or roslaunch mybot_gazebo mybot_world.launch)

- run_gmapping.sh ( or roslaunch mybot_navigation gmapping_demo.launch )

- run_gmapping_rviz.sh ( or roslaunch mybot_description mybot_rviz_gmapping.launch )

Move the Robot 

- run_teleop.sh ( the same of the turtlebot used during lessons, NON TUTTI I PULSANTI VANNO PROVARNE DIVERSI PER FARLO MUOVERE UN PO ('i' ed 'u' funzionano) ---> DA RISOLVERE)

Saving the Map 

- rosrun map_server map_saver -f ~/mybot_ws/src/mybot_navigation/maps/test_map

UNA VOLTA SALVATA LA MAPPA CHIUDERE I TERMINALI

Loading the Map (load a previous map for SLAM) 

- run_gazebo.sh

- run_nav.sh

- run_rviz.sh ( far navigare il robot usando 2D NAV GOAL )

BISOGNA SISTEMARE LE MASSE E LE DIMENSIONI DELL ORTHOPILLAR PERCHÈ È UNA CALESSINO e NON RISPONDE BENE AI COMANDI, CREDO GLI MANCHINO QUALCHE JOINT (?) ----> DA RISOLVERE
LA NAVIGAZIONE FA UN PO CAGARE MA PER ADESSO L IMPORTANTE FUNZIONI la sistemiamo direttamente su rOS2


