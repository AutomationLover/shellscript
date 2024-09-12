

Save selected env var to file
(printenv | grep 'API_ARTIFACT_PATH\|API_GATEWAY_SWAGGER_FILE') > environment.txt



Save selected env var to file
(printenv | grep 'API_ARTIFACT_PATH\|API_GATEWAY_SWAGGER_FILE') > environment.txt

Export to env var
export $(cat environment.txt | xargs)

xargs is a command line tool that allows you to use STDIN as the argument to another program.

xargs: STDIN --> args to other program

https://remysharp.com/2016/12/16/tricks-with-xargs

