# api


https://github.com/gupta-sudo/api




-----------+-----------------------+------------------------------------------------------------
 Method    | URI                   | Action
-----------+-----------------------+------------------------------------------------------------
 GET|HEAD  | /                     | Closure
 GET|HEAD  | api/tasks             | App\Http\Controllers\TaskController@index
 POST      | api/tasks             | App\Http\Controllers\TaskController@store
 GET|HEAD  | api/tasks/create      | App\Http\Controllers\TaskController@create
 GET|HEAD  | api/tasks/{task}      | App\Http\Controllers\TaskController@show
 PUT|PATCH | api/tasks/{task}      | App\Http\Controllers\TaskController@update
 DELETE    | api/tasks/{task}      | App\Http\Controllers\TaskController@destroy
 GET|HEAD  | api/tasks/{task}/edit | App\Http\Controllers\TaskController@edit
 GET|HEAD  | api/user              | Closure
           |                       |
 GET|HEAD  | sanctum/csrf-cookie   | Laravel\Sanctum\Http\Controllers\CsrfCookieController@show
+--------+-----------+-----------------------+---------------------------------------------------

