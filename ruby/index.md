# Ruby

> Question taken from http://rubyquiz.com/quiz126.html
> Write a program that prints the numbers from 1 to 100.
> But for multiples of three print “Fizz” instead of the
> number and for the multiples of five print “Buzz”. For
> numbers which are multiples of both three and five
> print “FizzBuzz”.

Questions taken from http://www.toptal.com/ruby/interview-questions

- What will `val1` and `val2` equal after the code below is executed? Explain your answer.
```ruby
val1 = true and false  # hint: output of this statement in IRB is NOT value of val1!
val2 = true && false
```
- Which of the expressions listed below will result in `"false"`?
```ruby
true    ? "true" : "false"
false   ? "true" : "false"
nil     ? "true" : "false"
1       ? "true" : "false"
0       ? "true" : "false"
"false" ? "true" : "false"
""      ? "true" : "false"
[]      ? "true" : "false"
```
- Write a function that sorts the keys in a hash by the length of the key as a string. For instance, the hash:
```ruby
{ abc: 'hello', 'another_key' => 123, 4567 => 'third' }
```
should result in:
```ruby
["abc", "4567", "another_key"]
```
- Consider the following two methods:
```ruby
def times_two(arg1);
  puts arg1 * 2;
end

def sum(arg1, arg2);
  puts arg1 + arg2;
end
```
What will be the result of each of the following lines of code:
```ruby
times_two 5
times_two(5)
times_two (5)
sum 1, 2
sum(1, 2)
sum (1, 2)
```
- Consider the following code:
```ruby
VAL = 'Global'
 
module Foo
  VAL = 'Foo Local'
 
  class Bar
    def value1
      VAL
    end
  end
end
 
class Foo::Bar
  def value2
    VAL
  end
end
```
What will be the value of each of the following:
```ruby
Foo::Bar.new.value1
Foo::Bar.new.value2
```
Explain your answer.
- Is the line of code below valid Ruby code? If so, what does it do? Explain your answer.
```ruby
-> (a) {p a}["Hello world"]
```
- What is the difference between calling `super` and calling `super()`?
- Explain each of the following **operators** and how and when they should be used: `==`, `===`, `eql?`, `equal?`.
- Given:
```ruby
x = "hello"
```
Explain the difference between:
```ruby
x += " world"
```
and
```ruby
x.concat " world"
```
- In Ruby code, you quite often see the trick of using an expression like `array.map(&:method_name)` as a shorthand form of `array.map { |element| element.method_name }`. How exactly does it work?
- Write a single line of Ruby code that prints the Fibonacci sequence of any length as an array. (Hint: use `inject`)



# [Back to readme](../readme.md)