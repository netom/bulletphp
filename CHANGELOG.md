# 2.0

* run() only accepts Request instances
* ->path(array('...', ...)) paths are not supported
* If we get no response, but managed to parse an url without an error, return an 501 Not Implemented status (?)
* Every URI part MUST have a path callback (?)
* $app->request() is not supported, you have to pass around the \Bullet\Request object manually
* Param callbacks receive Closure objects, no strings allowed.
* $app->response() receives the response data as the first parameter, and the response code as the second.