# arm_typed_robot
gazebo files for an arm typed robot on ROS2.

Gazebo用のアームロボットのファイルです．
簡単なリンク構造で作成しているので，アームの変更が簡単にできます．

# How to Use
Run Docker and access "http://localhost:6080" with your browser.

Docker で起動して，ブラウザ経由で「http://localhost:6080 」にアクセスすると接続できます．
> docker compose up

Run the desktop icon "Gazebo(Arm Typed Robot)".
You can control the robot with the following command:

デスクトップの「Gazebo(Arm Typed Robot)」というアイコンをダブルクリックするとGazeboが立ち上がります．
以下のコマンドで関節を制御できます．
> gz topic -t /joint2_position_cmd -m gz.msgs.Double -p "data: 0"

Joint number is from 1 to 4. 
関節番号（jointX）は，1から4です．

<a href="https://github.com/wadaru/arm_typed_robot/blob/main/Screen%20Recording%202025-12-11%20at%2018.30.59.mov">movie</a>
