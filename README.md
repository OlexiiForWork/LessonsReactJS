# LessonsReactJS
Мои уроки по React JS

## Сылка на неплохую теорию (Metanit)
-  [Metanit] https://metanit.com/web/react/;
  
## Сылка Обучающие видео в YouTube:
-  https://www.youtube.com/watch?v=lzICzoqlJgc&list=PL9mlH9etz6DyxCwks1tdVzlYhSxrsrjJ4;
-  https://www.youtube.com/watch?v=xJZa2_aldDs&list=RDQMVAcV6YX3oNs&start_radio=1;
-  https://www.youtube.com/watch?v=NDPiaUfsnLA&list=PL6NCtzCz-4pR_xzjVY6wpSTppLdJJmUqF;
-  https://www.youtube.com/watch?v=w4oNcyFhqzw&list=PL_Ff6C61NLImA9pRrkFXp8yaWz1_RtFdQ;
-  https://www.youtube.com/watch?v=tfn-59fbNMQ&list=PLDyJYA6aTY1lpbNh66kFpF62QpJyzliT2;
## Настройка Visual Studio Code для програмирования .Net:
-  Настройка Visual Studio и Visual Studio Code под C#: https://www.youtube.com/watch?v=9XYwm2GOQtk;
## React + .Net Core:  
-  ASP.NET Core + React веб-приложение | Как связать Бэкенд и Фронтенд?: https://www.youtube.com/watch?v=csD_-3Gdk5k;
-  Аутентификация в ASP.NET Core 8 с помощью JWT и Cookies + Хеширование: https://www.youtube.com/watch?v=sMe3T6rFkXo&list=PLBf3IyPz_J6WdTX3XYGajf8Z_2mZg5_xI;

## Офицыальнные сайты
-  [GitHub] https://github.com/facebook/react
-  [React] https://react.dev/



\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/

It is expected that developers will host a local version of a Postgres database for development. Development against the database in DevQA can be done by using the LocalDevqa configuration mentioned above, however it is usually not neccessary. Migrations should always be tested locally before deploying. _Migrations should **never** be tested against DevQA._

The postgres instance is now part of the OPF shared development stack for RefArch applications. You will need to clone the [ordermanagement.shared.refarch-dev-stack](https://github.com/EBSCOIS/ordermanagement.shared.refarch-dev-stack) repository and execute the `setup-stack.ps1` script to install the needed postgres container.

Once the shared development stack is running use the following script located in the src directory to setup the database:

```
powershell .\reset-db.ps1
```

> Once this is done you can reset the database back to the default state by re-running the reset-db script.

This database will be running in a postgres container with the following values:

-   Server: `localhost:12695`
-   Username: `app`
-   Password: `verysecure`
-   Database: orders
