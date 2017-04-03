# 4.0 Operating Instructions

There are two methods to add the blocks with coding:

The first is simple call like following with [**Smarty**](http://www.smarty.net/):

```smarty
<{xoBlk module="system" file="system_blocks.php" show_func="b_system_search_show"  template="system_block_search.html"}>
```

The second way is to format the Smarty template as following:

```smarty
<{xoBlkTpl module="system" file="system_blocks.php" show_func="b_system_search_show" }> 
<form style="margin-top: 0px;" action="<{$xoops_url}>/search.php" method="get"> 
  <input type="text" name="query" size="14" /><input type="hidden" name="action" value="results" /><br /><input type="submit" value="<{$block.lang_search}>" /> 
</form> 
<a href="<{$xoops_url}>/search.php" title="<{$block.lang_advsearch}>"><{$block.lang_advsearch}></a> 
<{/xoBlkTpl}>
```



