# Python + Django sample

This sample contains the basic program with routes and rendering templates in response of calls. Also has a simple database interaction with sqlite3. Attention: no controls. 

It also contains the Dockerfile and uwsgi.ini files necessary to build a container with a production server. The resulting image works both locally and when deployed to some cloud service. 


## Installation

You need Docker installed first. Then, go to the root folder and run: 

```bash
$ docker build -t your_name/your_app_name .
$ docker run -p 49160:8000 -d your_name/your_app_name
```

## Usage

On browser, go to 127.0.0.1/49160

Possible routes: 

```bash
127.0.0.1/49160/ (shows the last 5 messages logged)
127.0.0.1/49160/about/
127.0.0.1/49160/contact/
127.0.0.1/49160/log/ (allow you to input a simple message to test)

```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)