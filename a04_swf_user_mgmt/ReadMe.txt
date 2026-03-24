this is an example on how Xcoms can work within a Snowflake Operator.
you have to create a xcom reader function outside the dag, for some reasons it does not work directly in the Operator
like in hte traditional syntax you needed a python operator to read xcoms, here you use a function 