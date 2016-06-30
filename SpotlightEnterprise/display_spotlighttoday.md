---
title: Spotlight today
keywords: spotlight today
summary: "Spotlight Today is a display of recent alarms and alarms requiring acknowledgment."
sidebar: p_enterprise_sidebar
permalink: /enterprise_spotlighttoday/
---

## About the Spotlight today grid
The Spotlight today grid is made up of rows and columns where each row represents an alarm and each column information about that alarm.

Column | Description
-------|------------
Severity | The degree of urgency of the alarm. The color used depends on the severity of the alarm.
Alarm | The name of the alarm. This column is unavailable when the Group By action is set to Alarm.
Connection | The connection the alarm was raised on. This column is unavailable when the Group By action is set to Connection.
Raised | The time the alarm was raised.
Message | More information on the alarm.
Snoozed By | The user who requested the alarm be snoozed.
Snoozed Until | The time the alarm is snoozed until.
Condition Cleared | The time the alarm severity returned to normal. This is relevant to alarms that require acknowledgment.
Connection type | The type of connection the alarm was raised on (for example, SQL Server). The connection type is available only when the Group By action is set to Connection.

{% include tip.html content="The Spotlight Today grid is a Spotlight grid which may be saved to a file or the clipboard. To show / hide columns on the grid, right-click the grid headings and select Organize Columns. Refer to the help for more information on Spotlight grids." %}

## Filter the Spotlight today grid

![Filter]({{ "/imagesClient/tb_action_changefilter.png" | prepend: site.baseurl }})
Filter the Spotlight today grid from the Filter ribbon group.

Ribbon Select | Description
--------------|------------
Filter by Severity | Show alarms of a certain severity.
Hide Snoozed Alarms | Remove snoozed alarms from the grid.


## Actions on the Spotlight today grid

These actions are selectable from the Action ribbon group. Some actions are enabled only when an alarm is selected.

*  To select an alarm, highlight it on the Spotlight today grid.
*  Use SHIFT to select (or deselect) a range of alarms.
*  Use CTRL to select (or deselect) non sequential alarms.

Icon | Ribbon Select | Description
-----|---------------|-------------
![Diagnose]({{ "/imagesClient/tb_action_diagnose.png" | prepend: site.baseurl }}) | Diagnose | Show the drilldown relevant to the selected alarm.
![Acknowledge]({{ "/imagesClient/tb_alarms_acknowledge.png" | prepend: site.baseurl }}) | Acknowledge | Acknowledge the selected alarm(s). This is appropriate for alarms that are configured to require acknowledgment.
![Show in Alarms by Time]({{ "/imagesClient/tb_alarms_alarmhistory.png" | prepend: site.baseurl }}) |  Alarm History | Show the selected alarm in alarms by time.
![Snooze]({{ "/imagesClient/tb_action_snooze.png" | prepend: site.baseurl }}) | Snooze Alarm | Temporarily remove the visual alert associated with the alarm.
![Ignore this Alarm]({{ "/imagesClient/tb_action_ignorealarm.png" | prepend: site.baseurl }}) | Ignore this Alarm | Configure Spotlight to ignore this alarm and future cases of this alarm. Select the rule by which you want Spotlight to ignore future cases of this alarm: ignore this alarm for the current value or for the current connection. The choices are dependent on the type of alarm. This is a simplified interface for Configure \| Alarms \| Do not alarm for certain values.
![Alarm Settings]({{ "/imagesClient/tb_action_settings.png" | prepend: site.baseurl }}) | Alarm Settings | Configure the selected alarm.
![Find]({{ "/imagesClient/tb_grid_find.png" | prepend: site.baseurl }}) | Find | Find text in the list of alarms.
![Collapse all]({{ "/imagesClient/tb_action_collapseall.png" | prepend: site.baseurl }}) | Collapse All | Collapse the tree view of the list of alarms.
![Group by]({{ "/imagesClient/tb_action_groupby.png" | prepend: site.baseurl }}) | Group By | Group the alarms according to: <br> *Alarm* The name of the alarm. <br> *Connection* The name of the connection. <br> *Ungrouped (top 50 only)* Show the alarms in order of severity. Limit the display to 50 alarms.


## Configure Spotlight today
Spotlight today can be configured to be the first page you see when you open Spotlight. For more information, see Spotlight startup location.