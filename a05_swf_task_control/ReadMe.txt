timestamp -> string 
this step is needed because timestamps are not json serializable and cannot be returned
so for timestamp comparison from an unpstream task to a downstream task we needed

UPSTREAM TASK
timestamp->string 

DOWNSTREAM TASK
string->timestamp