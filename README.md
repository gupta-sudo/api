# api


https://github.com/gupta-sudo/api


+--------+-----------+-----------------------+---------------+------------------------------------------------------------+------------------------------------------+
| Domain | Method    | URI                   | Name          | Action                                                     | Middleware                               |
+--------+-----------+-----------------------+---------------+------------------------------------------------------------+------------------------------------------+
|        | GET|HEAD  | /                     |               | Closure                                                    | web                                      |
|        | GET|HEAD  | api/tasks             | tasks.index   | App\Http\Controllers\TaskController@index                  | api                                      |
|        | POST      | api/tasks             | tasks.store   | App\Http\Controllers\TaskController@store                  | api                                      |
|        | GET|HEAD  | api/tasks/create      | tasks.create  | App\Http\Controllers\TaskController@create                 | api                                      |
|        | GET|HEAD  | api/tasks/{task}      | tasks.show    | App\Http\Controllers\TaskController@show                   | api                                      |
|        | PUT|PATCH | api/tasks/{task}      | tasks.update  | App\Http\Controllers\TaskController@update                 | api                                      |
|        | DELETE    | api/tasks/{task}      | tasks.destroy | App\Http\Controllers\TaskController@destroy                | api                                      |
|        | GET|HEAD  | api/tasks/{task}/edit | tasks.edit    | App\Http\Controllers\TaskController@edit                   | api                                      |
|        | GET|HEAD  | api/user              |               | Closure                                                    | api                                      |
|        |           |                       |               |                                                            | App\Http\Middleware\Authenticate:sanctum |
|        | GET|HEAD  | sanctum/csrf-cookie   |               | Laravel\Sanctum\Http\Controllers\CsrfCookieController@show | web                                      |
+--------+-----------+-----------------------+---------------+------------------------------------------------------------+------------------------------------------+
