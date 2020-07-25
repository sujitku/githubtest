Write a program in PHP to find the sum of the array of numbers defined
<?php
$sum = 0;
for($x=1; $x<=30; $x++)
{
$sum +=$x;
}
echo "The sum of the numbers 0 to 30 is $sum"."\n";
?>

Write a php code to find the repeated number.
<?php 

function printRepeating($arr, $size) 
{ 
    $i; 
    $j; 
    echo " Repeating elements are "; 
  
    for($i = 0; $i < $size; $i++) 
        for($j = $i + 1; $j < $size; $j++) 
            if($arr[$i] == $arr[$j]) 
                echo $arr[$i], " "; 
}  
   
$arr = array(4, 2, 4, 5, 2, 3, 1); 
$arr_size = sizeof($arr, 0); 
printRepeating($arr, $arr_size); 
?>

Find the maximum consecutive 1's in an array of 0's and 1's.
<?php 
function getMaxLength($arr, $n) 
{ 
    
    $count = 0;  
      

    $result = 0;  
  
    for ($i = 0; $i < $n; $i++) 
    { 
     
        if ($arr[$i] == 0) 
            $count = 0; 
  
     
        else
        {
            $count++; 
            $result = max($result, $count); 
        } 
    } 
  
    return $result; 
} 
$arr = array(1, 1, 0, 0, 1, 0,  
             1, 0, 1, 1, 1, 1); 
$n = sizeof($arr) / sizeof($arr[0]); 
echo getMaxLength($arr, $n); 
?> 
