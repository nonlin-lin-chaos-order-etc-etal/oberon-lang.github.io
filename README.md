## Work in progress

Check back later.

### Code Examples

```linenos
module Fibonacci
  proc calc( n : integer ): integer
    var a,b: integer
  begin
    if n > 1 then 
      a := calc( n - 1 )
      b := calc( n - 2 )
      return ( a + b )
    elsif n = 0 then 
      return 0
    else 
      return 1
    end
  end calc
  var res: integer
begin
  res := calc(21)
  assert( res = 10946 )
  println("Fibonacci done")
end Fibonacci
```
