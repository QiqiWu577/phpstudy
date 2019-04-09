[PHP](https://en.wikipedia.org/wiki/PHP), **Hypertext Preprocessor**, is the popular server scripting language designed for web development. The main reason why I want to talk about PHP in this blog is that It has been a long time that learning PHP exists in my to-do list but just do not have sufficient time to do some research about it. Recently, I got a interview chance last week and the potential company asked me to solve the PHP problem. After I completed the task, I am so impressed about the efficiency of this programming language because the simple syntax and the a variaty of useful functions of its liabray. From my opinoin, It is really worthy here to share what handy knowledge of PHP I have learned.

Another thing I want to mention before we start to explore is that the compiler I use. Since I have to finish the task in the limited time, I did not loading my php file in the specific [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment). What I use is the [online sandbox PHP](http://sandbox.onlinephpfunctions.com/), which I found it is very useful and easy to use to test the output of the codes. In this blog, I would use the output that sanbox PHP compiles.

### Syntax

To create a php file, writing `<?php` at the beginning of the file with file extension ".php" is enough.The simple basic syntax is using php tag to create a php script. We can use this php tag every where in no matter html file or jsp file, which is very similar the way how we use the script tag. 

```markdown
<?php
// PHP code goes here
?>
```

Also, if you want to display the other tags in those file using php tag, you can just simply create them inside the php tag with double quotes. `echo` means output the content.

```markdown
<!DOCTYPE html>
<html>
<body>
<?php
$color = "red";
echo "My car is " . $color . "<br>";
echo "My house is " . $COLOR . "<br>";
echo "My boat is " . $coLOR . "<br>";
?>
</body>
</html>
```

### Array

The second thing I really like in PHP is the object [Array](https://www.php.net/manual/en/language.types.array.php). The Array in PHP acts not only like the ArrayList in Java. More than that, we can treat `Array` as an array, list (vector), hash table (an implementation of a map), dictionary, collection, stack, queue, and so on. what amazing thing is that an array values can be other arrays, trees and multidimensional arrays are also possible.

One interesting thing I really love is that you can set any numbers of comma-separated key => value pairs as arguments, which is very useful to store some key values as a pair and not only using index position.

```markdown
<?php
$array = array(
    "foo" => "bar",
    "bar" => "foo",
);
```

The symbol `=>` is used as an access mechanism for arrays. This means that the key on the left side will match the value on the right side. Another symbol `$` is used for declaring every variable in PHP.

```markdown
foreach($array as &$detail){
    echo $detail;
    $detail = "developer";
}
```

Using `&` before the variable is going to reference the original location of that element in the array so that we can reset the value of the array. Otherwise, you cannot change the value. Also, from my research, `foreach` can be only used for loop the elements in the array.

Last important feature of array I want to talk about is the multidimensional arrays, which provides more effective way to access the array then using Java. Specifically, you can set arrays inside of the array, which acts more like a tree.

```markdown
<?php
$array = array(
    "foo" => "bar",
    42    => 24,
    "multi" => array(
         "dimensional" => array(
             "array" => "foo"
         )
    )
);

var_dump($array["foo"]);
var_dump($array[42]);
var_dump($array["multi"]["dimensional"]["array"]);
?>
```

### String functions

Last but not least, [string functions](https://www.php.net/ref.strings) is the third thing that helps me a lot when I was tring to solve the PHP problem. The problem is about how to mask sensitive data with different data format, including array, string, JSON and xml formats. How to deal with these data format is easy because PHP already has handy functions to convert them to each other. The tricky point is that after replace all the sensitive data for some specific fields the ouput they require must be the exacly same as the original one, which means it would be a little bit complicated to achieve that if I want to use those usefule function existing in the PHP library and almost every thing I have to hardcode it. 

After a few hours struggling, I realized that it would be easier to treat those format as string and combine different parts after spliting a string and masking the sensitive data. In this way, I do not worry too much about the data format and also can store the data in the original format. Right now I will introduce 3 most useful string functions I found.

## preg_split


## stripos


## implode


### Summary

