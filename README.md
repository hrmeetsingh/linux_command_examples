# Linux Command Examples
## cURL - for quick API performance test

As per the curl man page, *"Make curl display information on stdout after a completed transfer. The format is a string that may contain  plain  text  mixed with  any  number of variables. The format can be specified as a literal "string", or you can have curl read the  format  from  a file  with  "@filename" and to tell curl to read the format from stdin you write "@-"."*

Run the following command fron inside the "curl" folder to get quick performance numbers for an API -

`curl -w "@curl-format.txt" -s -k -o /dev/null <URL>`

Example -

`curl -w "@curl-format.txt" -s -k -o /dev/null "https://www.google.com"`

Result -

`      response_code: 200`

`    time_namelookup:  0.005137`

`       time_connect:  0.009728`

`    time_appconnect:  0.133735`   
`   time_pretransfer:  0.134052`  
`      time_redirect:  0.000000`     
` time_starttransfer:  0.250884`

`                  ----------- ` 

`         time_total:  0.263603`
