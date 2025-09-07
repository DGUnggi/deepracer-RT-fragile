## Parameters that we have to consider in the process of defining reward function
`speed` : 0 ~ 4 m/s  
`distance_from_center` : Distance between center of car and track's center line  
`track_width` : Width of track  
`all_wheels_on_track` : 바퀴 하나라도 밖에 있으면 `False`  
`heading` : -180 ~ +180 -> 차의 진행 방향(각도)  
`steering_angle` : 이게 **차의 진행 방향** 에 대한 앞바퀴의 각도이기 때문에, **차의 진행 방향** 을 상대적인 기준으로 둬서 이제 어느 방향으로 이동할 것인지를 의미함  
`steps, progress, track_length, is_offtrack` : 이건 에피소드가 하나 끝날 때마다 reward를 어떻게 줄 지 결정하는 용도로 사용할 수 있을듯  
`is_left_of_center` : 직선 주행 구간에서 이후에 있을 코너 부분에서의 코너링을 빠르게 하기 위해 차선 유지하거나?, 쨌든 용도는 있을듯  
`is_reversed` : 이건 reward를 음수로 주거나 낮게 주면 될듯  
`waypoints, closest_waypoints` : 이건 waypoint들의 구간별 rep time을 재는 용도로 사용이 가능한가? 아니면 두 waypoint를 보고서 대충 어느 위치에 있는지 알아내는 용도인데, 사실 (x,y) 좌표가 더 직관적이긴 한데..  
> 이외의 parameter들은 예선전에서는 필요 없을듯
