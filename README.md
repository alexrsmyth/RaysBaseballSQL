# RaysBaseballSQL

This is my SQL analytics of Tamp Bay Rays baseball as I learn and test my SQL skills.
My focus on this analysis is on home game attendance and different factors affecting attendance.

* Using Google Cloud BigQuery

SELECT homeTeamName, attendance, FORMAT_DATE('%A', startTime) AS DayOfWeek, awayTeamName
FROM `bigquery-public-data.baseball.schedules` 
Where homeTeamName = 'Rays'
Order By attendance DESC

| Results form the above query |
| ----------- | ----------- |
| Row | homeTeamName | attendance | DayOfWeek | awayTeamName |
|  1  |     Rays     |    40135   | Friday    | Giants       |
|  2  |     Rays     |    31042   | Sunday    | BlueJays     |
|  3  |     Rays     |    30451   | Saturday  | White Sox    |
|  4  |     Rays     |    28158   | Saturday  | Athletics    |
|  5  |     Rays     |    27217   | Sunday    | BlueJays     |

*Results from query are for 81 home games during the 2016 season.



