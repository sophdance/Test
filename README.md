# Test

-- Select Nth highest Salary
With CTE as (
      Select *
      ,Row_number() over( order by Salary desc) R_Sal
      from emp
      )
Delete from CTE where R_Sal = 2
      
