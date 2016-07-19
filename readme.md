prereq:
Docker


Open the Docker terminal

download the latest Ubuntu, Erlang, Elixir, Phoenix

``` docker pull marcelocg/phoenix ```



``` docker run -it --rm -v "$PWD":/code -w /phoenix marcelocg/phoenix mix phoenix.new /code/my_new_app ```

- creates a folder called my_new_app


cd my_new_app

docker run -it --rm -v "$PWD":/code marcelocg/phoenix /bin/bash

``` mix deps.get ```


``` mix phoenix.new hello_world ```


``` cd hello_world ```

``` mix ecto.create ```
- create our database
- give it a couple minutes

``` mix phoenix.server ```



``` npm i ```
- I ran npm i from docker prompt, instead of from inside the container
- so exit the container first



run the docker container, exposing a port for dev http
``` docker run -it --rm -v "$PWD":/code -p 4000:4000 marcelocg/phoenix /bin/bash ```



browse to....
``` 192.168.99.100:4000 ```



#### ref:
mnk->comp->phoenix install: