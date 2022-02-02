# Academy
php project


<?php


function validateFloat($value): string
{
    if (!filter_var($value, filter:FILTER_VALIDATE_FLOAT)) {
        return "type is not float!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!";
    }else{
        return  "TYPE IS OK!!";
    }
}
function validatemin($value, $min_value) : string
{
    if ($value <= $min_value) {
        return "ERROR: Too few characters ";
    }
    return "OK";
}
