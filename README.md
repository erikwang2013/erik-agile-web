# erik-agile-web

https://github.com/tuteng/Best-websites-a-programmer-should-visit-zh

https://github.com/1c7/chinese-independent-developer


https://github.com/Wechat-ggGitHub/Awesome-GitHub-Repo

https://github.com/yuenov/reader-api



``
function marriedDeal($arr,$change_number){
    $i=0;
    $finsh=[];
    $default_total=count($arr);
    arsort($arr);
    $blance=0;
    while($default_total>=1){
        $i+=1;
        if($i>$default_total || $change_number<=0) break;
        $head=array_shift($arr);
        if($head>$change_number){
            array_push($arr,$head);continue;
        }
        $finsh[]=$head;
        $change_number-=$head;
        $blance=$change_number;
    }
    return [$finsh,$blance,$arr];
}
$get_number=marriedDeal([120,200,220,400,20,320,180],311);
print_r($get_number);
``
