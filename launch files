<launch>
  <arg name="model" default="$(find owl_robot_description)/urdf/owl_robot.urdf" />
  <param name="robot_description" command="cat $(arg model)" />
  <node name="robot_state_publisher" pkg="robot_state_publisher" type="robot_state_publisher" output="screen">
    <param name="publish_frequency" type="double" value="50.0" />
    <param name="tf_prefix" type="string" value="" />
  </node>
  <node name="joint_state_publisher" pkg="joint_state_publisher" type="joint_state_publisher" output="screen"/>
  <node name="rviz" pkg="rviz" type="rviz" args="-d $(find owl_robot_description)/rviz/owl_robot.rviz" />
</launch>
