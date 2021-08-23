# Movies-app

### Overview
Movies-App lets you create and manage movies, actors and directors (using React.js and Django Rest Framework). To see full functionality register after running app.

### Requirements
- Docker
- Code editor (for API keys)

### How to run project?
1. Clone repository `git clone --recurse-submodules git@github.com:szym0nplaza/movies-app.git`
2. If you want to use celery functionality see [this](#celery)
<a name="conf"></a>
3. Run app `docker-compose up --build`
4. Run migrations: 
    - In terminal type: `docker ps`
    - Copy <em>movies-app-backend</em> container id
    - Run command: `docker exet -it <container_id> bash`
    - In bash type: `python manage.py migrate`

<a name="celery"></a>
### Using Celery
1. First you need to gain API key. To get it follow the rules on this website https://developers.themoviedb.org/3/getting-started/introduction
2. Paste your API key in `.env` file in <em>movies-app-backend</em> directory and [finish configuartion](#conf)

## Screenshot

![alt text](https://github.com/szym0nplaza/movies-app/blob/main/screens/screen1.png)
### More screenshots
- https://github.com/szym0nplaza/movies-app/tree/main/screens
