Definition 2:
Write a PL/SQL block that explains the use of ZERO_DIVIDE exception.
set serveroutput on;
declare num1
number := &a; num2
number := &b;
answer number;

Marwadi University
Faculty of Computer Applications

begin dbms_output.put_line('Value of num1: ' ||
num1); dbms_output.put_line('Value of num2: ' ||
num2);
answer := num1 / num2;
dbms_output.put_line('Answer: ' || answer);
exception
when ZERO_DIVIDE then
dbms_output.put_line('num2 must not be zero');
end;
/
