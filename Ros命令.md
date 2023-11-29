\#Ros命令

\#\# 召唤海龟三步🐢

\`roscore\`

\`rosrun turtlesim turtlesim_node\`

\`rosrun turtlesim turtle_telop_key\`

\#\# 工具

\#\#\# 检索工具

\* 查看一个系列的__\*\*可执行命令\*\*__的输出该系列的命令行工具

\`rosnode\`

\`rostopic\`

\`rossevice\`

\* 查看该系列的__\*\*在执行单位\*\*__在后面加\`list\`

\* 查看该系列的__\*\*详细运行信息\*\*__在后面加\`info \__name__\`

\* 可视化查看连接信息工具

\`rqt_graph\`

\#\#\# 记录工具

\* 记录(record)

\-a是all的意思 -O是打包的意思

\`rosbag record -a -O \__bag_name__\`

\* 复现(play)

\`rosbag play \__bag_name__\`

\#\# 话题(topic)

\* 发送指令(pub)

\`rostopic pub -r \__rate_\_ \__subscriber_\_ \__cmd__\`

\* 让海龟动🐢

\`rostopic pub \__turtle_\_ geometry_msgs/Twist "__msgs_detail__"\`

\#\# 服务(service)

\* 召唤海龟

\`rosservice call /spawn "__msgs_of_turtle__"\`
