# Test

-- Select Nth highest Salary
With CTE as (
      Select *
      ,Row_number() over( order by Salary desc) R_Sal
      from emp
      )
Delete from CTE where R_Sal = 2

Select * from emp
      
Update table emp
set ename = 'Jane'
where id = 5
this is new one 9.20
