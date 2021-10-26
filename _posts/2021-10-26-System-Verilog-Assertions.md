---
published: true
---
###### Notes
 - Failures in antecedent are called vacous success.
 - Two ways to combine ancedent
	`ifdef M1
		sec == 0 && $past(min) != 59
	`endif
	`ifdef M2
		sec == 0
		##0 			// in the same cycle 
		$past(min) != 59
	`endif
    
 - Assertions are always overlapping. It can be avoided by $rose(). It is used to avoid multiple triggering of assertion.
 
 ```
	1)  x 
		|->
		##3
		y==20
	
	2)	//x==0 ##1 x==1
		$rose(x)
		|->
		##3
		y==20
 ```
 - After ##1 clock delay we can't use if statement but we can use ternary operator ? :
 - iff statement works only with disable block
 - Boolean operators `(|| &&)` are not allowed inside assert block for combining sequence. But we can use then in boolean expression.
 ```
		a && b 
		
		(a ##1 b) and (b ##2 c)
 ```
 - Add `-msgmode both` to vsim command to view assertion message (triangles) in the waveform (for Questasim).
 - Assertion doesn't have a right to change a variable. It can only do comparision check.
 - To use `local variable` inside assertion we have to use property block.
 - ```
	  Boolean Algebra
	  a    b
	  and  &
	  or   |
	  xor  ^
	  xnor !(a^b)  (a !^ b)
	  
	  not !(a) 
	  
	  // Sequence 
	  s1 or  s2 
	  s1 and s2 
	  not (s1)
	  
	  s1 intersect s2 
	  s1 within s2
	  s2 within s1
	  
  ```
 -
