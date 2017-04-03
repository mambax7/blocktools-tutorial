# 8.0 Other

There were other solutions similar to this one:

1\) **Blocks Anywhere** developed by [**Trabis**](https://www.xuups.com/modules/publisher/item.php?itemid=10)

On his Website he describes the module this way: 

Here is an easy way to place a block in a theme or template.

Just upload this smarty plugin to class/smarty/xoops\_plugins folder and you will be able to add a block using the following method

\`\`\`php

&lt;{block id=1}&gt;

\`\`\`



Replace '1' by the id of the block you want to display.



You can find id of block in blocks admin, just hover the mouse over block edit link and you will see something like this:



yoursite/modules/system/admin.php?fct=blocksadmin&op=edit&bid=3



This plugin respect XOOPS permissions. It will only display the block for users that are allowed to see it\(as set in groups permissions\).



This plugin also takes in consideration cached blocks.



Version 1.1 brings you some new cool options such as:



display = 'title' -&gt; shows just title

display = 'none' -&gt; renders the block but does not display it

options = 'enter\|block\|options' -&gt; overwrites block default options

groups = 'enter\|allowed\|groups' -&gt; overwrites block default group view permissions

cache = 3600 -&gt; overwrite cache time\(in seconds\)



Code examples:

&lt;{block id=1 display="title"}&gt;   displays just the block title 

&lt;{block id=1}&gt;                   displays just the block content 

&lt;{block id=7 display="none"}&gt;    does not display nothing but executes the block, this can go for online block or to trigger some cron block

&lt;{block id=600 groups="0\|1" cache=20}&gt;  display block just for this 2 groups and sets a cache of 20 seconds

&lt;{block id=600 options="100\|100\|s\_poweredby.gif\|0"}&gt; displays block with diferent options





Usage example:

Place your 'multimenu' block in your theme. 

Invisible online block that updates online users table.

Add an image gallery block inside article category page.

Add users online block into yogurt profile page

Etc... way to place a block in a theme or template.



Just upload this smarty plugin to class/smarty/xoops\_plugins folder and you will be able to add a block using the following method:

&lt;{block id=1}&gt;





Replace '1' by the id of the block you want to display.



You can find id of block in blocks admin, just hover the mouse over block edit link and you will see something like this:



yoursite/modules/system/admin.php?fct=blocksadmin&op=edit&bid=3



This plugin respect XOOPS permissions. It will only display the block for users that are allowed to see it\(as set in groups permissions\).



This plugin also takes in consideration cached blocks.



Version 1.1 brings you some new cool options such as:



display = 'title' -&gt; shows just title

display = 'none' -&gt; renders the block but does not display it

options = 'enter\|block\|options' -&gt; overwrites block default options

groups = 'enter\|allowed\|groups' -&gt; overwrites block default group view permissions

cache = 3600 -&gt; overwrite cache time\(in seconds\)



Code examples:

&lt;{block id=1 display="title"}&gt;   displays just the block title 

&lt;{block id=1}&gt;                   displays just the block content 

&lt;{block id=7 display="none"}&gt;    does not display nothing but executes the block, this can go for online block or to trigger some cron block

&lt;{block id=600 groups="0\|1" cache=20}&gt;  display block just for this 2 groups and sets a cache of 20 seconds

&lt;{block id=600 options="100\|100\|s\_poweredby.gif\|0"}&gt; displays block with diferent options





Usage example:

Place your 'multimenu' block in your theme. 

Invisible online block that updates online users table.

Add an image gallery block inside article category page.

Add users online block into yogurt profile page

Etc...

2\) A solution developed by Catzwolf

