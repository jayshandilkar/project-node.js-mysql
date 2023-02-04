# project-nodejs-mysql
# I follow this docs for following project --> https://varsubham.medium.com/nodejs-mysql-docker-compose-ad156cd0c885
# when some error occure i follow this docs --> https://sebhastian.com/npm-err-missing-script-start/ERROR: for ubuntu_web_1  Cannot start service web: driver failed programming external connectivity on endpoint ubuntu_web_1 (79ea4a8129a1de8f729eb8f6ac9a074592b6e243d130c73e11389b178116d15d): Error starting userland proxy: listen tcp4 0.0.0.0:5000: bind: address already in use

If we getting that one error :-
ERROR: for web  Cannot start service web: driver failed programming external connectivity on endpoint ubuntu_web_1 (79ea4a8129a1de8f729eb8f6ac9a074592b6e243d130c73e11389b178116d15d): Error starting userland proxy: listen tcp4 0.0.0.0:5000: bind: address already in use
ERROR: Encountered errors while bringing up the project.

For solution if we need to kill running process by using " kill -9 with process id " .



ERROR :-------
throw er; // Unhandled 'error' event
      ^

Error: listen EADDRINUSE: address already in use :::5000

solution :- we need to kill docker compose process id " kill -9 process id ".
