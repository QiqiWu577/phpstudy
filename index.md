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

The second thing I really like in PHP is the object `Array`

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
