<?php 
/*
分类函数
$line 进行分类的资源 
$pid  分类的pid
$lever 等级
 */
function Tree($line,$pid = 0,$lever = 0)
{
	//定义一个空数组
	static $arr = array();
	foreach ($line as  $value) {
		if($value['pid'] == $pid){
			$value['lever'] = $lever;
			$arr[] = $value;
			//函数自调
			Tree($line,$value['id'],$lever+1);
		}
	}
	return $arr;
}


 ?>
